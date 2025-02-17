# Block Additional Mapping

Extra data or metadata can be added to each `Block` using `BlockAdditional` data.
Each `BlockAdditional` contains a `BlockAddID` that identifies the kind of data it contains.
When the `BlockAddID` is set to "1" the contents of the `BlockAdditional` element
are define by the Codec Mappings defines; see (#codec-blockadditions).
When the `BlockAddID` is set a value greater than "1", then the contents of the
`BlockAdditional` element are defined by the `BlockAdditionalMapping` element, within
the associated `Track` element, where the `BlockAddID` element of `BlockAdditional` element
equals the `BlockAddIDValue` of the associated `Track`'s `BlockAdditionalMapping` element.
That `BlockAdditionalMapping` element identifies a particular `Block Additional Mapping` by the `BlockAddIDType`.

The following XML depicts a use of a `Block Additional Mapping` to associate a timecode value with a `Block`:

```xml
<Segment>
  <!--Mandatory elements omitted for readability-->
  <Tracks>
    <TrackEntry>
      <TrackNumber>1</TrackNumber>
      <TrackUID>568001708</TrackUID>
      <TrackType>1</TrackType>
      <BlockAdditionalMapping>
        <BlockAddIDValue>2</BlockAddIDValue><!--arbitrary value
          used in BlockAddID-->
        <BlockAddIDName>timecode</BlockAddIDName>
        <BlockAddIDType>12</BlockAddIDType>
      </BlockAdditionalMapping>
      <CodecID>V_FFV1</CodecID>
      <Video>
        <PixelWidth>1920</PixelWidth>
        <PixelHeight>1080</PixelHeight>
      </Video>
    </TrackEntry>
  </Tracks>
  <Cluster>
    <Timestamp>3000</Timestamp>
    <BlockGroup>
      <Block>{binary video frame}</Block>
      <BlockAdditions>
        <BlockMore>
          <BlockAddID>2</BlockAddID><!--arbitrary value from
            BlockAdditionalMapping-->
          <BlockAdditional>01:00:00:00</BlockAdditional>
        </BlockMore>
      </BlockAdditions>
    </BlockGroup>
  </Cluster>
</Segment>
```

`Block Additional Mappings` detail how additional data **MAY** be stored in the `BlockMore` element
with a `BlockAdditionMapping` element, within the `Track` element, which identifies the `BlockAdditional` content.
`Block Additional Mappings` define the `BlockAddIDType` value reserved to identify that
type of data as well as providing an optional label stored within the `BlockAddIDName` element.
When the `Block Additional Mapping` is dependent on additional contextual information,
then the Mapping **SHOULD** describe how such additional contextual information is stored within the `BlockAddIDExtraData` element.
