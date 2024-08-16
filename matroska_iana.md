


## Matroska Compression Algorithms Registry

IANA has created a new registry called the "Matroska Compression Algorithms" registry.
The values correspond to the unsigned integer `ContentCompAlgo` value described in (#contentcompalgo-element).

To register a new Compression Algorithm in this registry, one needs a Compression Algorithm value,
a description, a Change Controller, and
a Reference to a document describing the Compression Algorithm.

The Compression Algorithms are to be allocated according to the "Specification Required" policy [@!RFC8126]. Available values range from 4-18446744073709551615.

(#compression-algorithm-registry-table) shows the initial contents of the "Matroska Compression Algorithms" registry.
The Change Controller for the initial entries is the IETF.

Compression Algorithm | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0 | zlib | RFC 9559, (#contentcompalgo-element)
1 | bzlib | RFC 9559, (#contentcompalgo-element)
2 | lzo1x | RFC 9559, (#contentcompalgo-element)
3 | Header Stripping | RFC 9559, (#contentcompalgo-element)
Table: Initial Contents of "Matroska Compression Algorithms" Registry{#compression-algorithm-registry-table}


## Matroska Encryption Algorithms Registry

IANA has created a new registry called the "Matroska Encryption Algorithms" registry.
The values correspond to the unsigned integer `ContentEncAlgo` value described in (#contentencalgo-element).

To register a new Encryption Algorithm in this registry, one needs an Encryption Algorithm value,
a description, a Change Controller, and
an optional Reference to a document describing the Encryption Algorithm.

The Encryption Algorithms are to be allocated according to the "First Come First Served" policy [@!RFC8126]. Available values range from 6-18446744073709551615.

(#encryption-algorithm-registry-table) shows the initial contents of the "Matroska Encryption Algorithms" registry.
The Change Controller for the initial entries is the IETF.

Encryption Algorithm | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0 | Not encrypted | RFC 9559, (#contentencalgo-element)
1 | DES | RFC 9559, (#contentencalgo-element)
2 | 3DES | RFC 9559, (#contentencalgo-element)
3 | Twofish | RFC 9559, (#contentencalgo-element)
4 | Blowfish | RFC 9559, (#contentencalgo-element)
5 | AES | RFC 9559, (#contentencalgo-element)
Table: Initial Contents of "Matroska Encryption Algorithms" Registry{#encryption-algorithm-registry-table}


## Matroska AES Cipher Modes Registry

IANA has created a new registry called the "Matroska AES Cipher Modes" registry.
The values correspond to the unsigned integer `AESSettingsCipherMode` value described in (#aessettingsciphermode-element).

To register a new AES Cipher Mode in this registry, one needs an AES Cipher Mode value,
a description, a Change Controller, and
an optional Reference to a document describing the AES Cipher Mode.

The AES Cipher Modes are to be allocated according to the "First Come First Served" policy [@!RFC8126]. Available values range from 3-18446744073709551615.

The value 0 is not valid for use as an AES Cipher Mode.

(#aes-cipher-mode-registry-table) shows the initial contents of the "Matroska AES Cipher Modes" registry.
The Change Controller for the initial entries is the IETF.

AES Cipher Mode | Description            | Reference
----------:|:------------------------|:-------------------------------------------
1 | AES-CTR | RFC 9559, (#aessettingsciphermode-element)
2 | AES-CBC | RFC 9559, (#aessettingsciphermode-element)
Table: Initial Contents of "Matroska AES Cipher Modes" Registry{#aes-cipher-mode-registry-table}


## Matroska Content Encoding Scopes Registry

IANA has created a new registry called the "Matroska Content Encoding Scopes" registry.
The values correspond to the unsigned integer `ContentEncodingScope` value described in (#contentencodingscope-element).

To register a new Content Encoding Scope in this registry, one needs a Content Encoding Scope value,
a description, a Change Controller, and
a Reference to a document describing the Content Encoding Scope.

The Content Encoding Scopes are to be allocated according to the "Specification Required" policy [@!RFC8126]. Available values range from 0x8-0x8000000000000000.

The Content Encoding Scope is a bit-field value so only power of 2 value can be registered.

The value 0 is not valid for use as a Content Encoding Scope.

(#content-encoding-scope-registry-table) shows the initial contents of the "Matroska Content Encoding Scopes" registry.
The Change Controller for the initial entries is the IETF.

Content Encoding Scope | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0x1 | Block | RFC 9559, (#contentencodingscope-element)
0x2 | Private | RFC 9559, (#contentencodingscope-element)
0x4 | Next | RFC 9559, (#contentencodingscope-element)
Table: Initial Contents of "Matroska Content Encoding Scopes" Registry{#content-encoding-scope-registry-table}


## Matroska Content Encoding Types Registry

IANA has created a new registry called the "Matroska Content Encoding Types" registry.
The values correspond to the unsigned integer `ContentEncodingType` value described in (#contentencodingtype-element).

To register a new Content Encoding Type in this registry, one needs a Content Encoding Type value,
a description, a Change Controller, and
a Reference to a document describing the Content Encoding Type.

The Content Encoding Types are to be allocated according to the "Specification Required" policy [@!RFC8126]. Available values range from 2-18446744073709551615.

(#content-encoding-type-registry-table) shows the initial contents of the "Matroska Content Encoding Types" registry.
The Change Controller for the initial entries is the IETF.

Content Encoding Type | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0 | Compression | RFC 9559, (#contentencodingtype-element)
1 | Encryption | RFC 9559, (#contentencodingtype-element)
Table: Initial Contents of "Matroska Content Encoding Types" Registry{#content-encoding-type-registry-table}


## Matroska Stereo Modes Registry

IANA has created a new registry called the "Matroska Stereo Modes" registry.
The values correspond to the unsigned integer `StereoMode` value described in (#stereomode-element).

To register a new Stereo Mode in this registry, one needs a Stereo Mode value,
a description, a Change Controller, and
a Reference to a document describing the Stereo Mode.

The Stereo Modes are to be allocated according to the "Specification Required" policy [@!RFC8126]. Available values range from 15-18446744073709551615.

(#stereo-mode-registry-table) shows the initial contents of the "Matroska Stereo Modes" registry.
The Change Controller for the initial entries is the IETF.

Stereo Mode | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0 | mono | RFC 9559, (#stereomode-element)
1 | side by side (left eye first) | RFC 9559, (#stereomode-element)
2 | top - bottom (right eye is first) | RFC 9559, (#stereomode-element)
3 | top - bottom (left eye is first) | RFC 9559, (#stereomode-element)
4 | checkboard (right eye is first) | RFC 9559, (#stereomode-element)
5 | checkboard (left eye is first) | RFC 9559, (#stereomode-element)
6 | row interleaved (right eye is first) | RFC 9559, (#stereomode-element)
7 | row interleaved (left eye is first) | RFC 9559, (#stereomode-element)
8 | column interleaved (right eye is first) | RFC 9559, (#stereomode-element)
9 | column interleaved (left eye is first) | RFC 9559, (#stereomode-element)
10 | anaglyph (cyan/red) | RFC 9559, (#stereomode-element)
11 | side by side (right eye first) | RFC 9559, (#stereomode-element)
12 | anaglyph (green/magenta) | RFC 9559, (#stereomode-element)
13 | both eyes laced in one Block (left eye is first) | RFC 9559, (#stereomode-element)
14 | both eyes laced in one Block (right eye is first) | RFC 9559, (#stereomode-element)
Table: Initial Contents of "Matroska Stereo Modes" Registry{#stereo-mode-registry-table}


## Matroska Alpha Modes Registry

IANA has created a new registry called the "Matroska Alpha Modes" registry.
The values correspond to the unsigned integer `AlphaMode` value described in (#alphamode-element).

To register a new Alpha Mode in this registry, one needs an Alpha Mode value,
a description, a Change Controller, and
an optional Reference to a document describing the Alpha Mode.

The Alpha Modes are to be allocated according to the "First Come First Served" policy [@!RFC8126]. Available values range from 2-18446744073709551615.

(#alpha-mode-registry-table) shows the initial contents of the "Matroska Alpha Modes" registry.
The Change Controller for the initial entries is the IETF.

Alpha Mode | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0 | none | RFC 9559, (#alphamode-element)
1 | present | RFC 9559, (#alphamode-element)
Table: Initial Contents of "Matroska Alpha Modes" Registry{#alpha-mode-registry-table}


## Matroska Display Units Registry

IANA has created a new registry called the "Matroska Display Units" registry.
The values correspond to the unsigned integer `DisplayUnit` value described in (#displayunit-element).

To register a new Display Unit in this registry, one needs a Display Unit value,
a description, a Change Controller, and
a Reference to a document describing the Display Unit.

The Display Units are to be allocated according to the "Specification Required" policy [@!RFC8126]. Available values range from 5-18446744073709551615.

(#display-unit-registry-table) shows the initial contents of the "Matroska Display Units" registry.
The Change Controller for the initial entries is the IETF.

Display Unit | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0 | pixels | RFC 9559, (#displayunit-element)
1 | centimeters | RFC 9559, (#displayunit-element)
2 | inches | RFC 9559, (#displayunit-element)
3 | display aspect ratio | RFC 9559, (#displayunit-element)
4 | unknown | RFC 9559, (#displayunit-element)
Table: Initial Contents of "Matroska Display Units" Registry{#display-unit-registry-table}


## Matroska Horizontal Chroma Sitings Registry

IANA has created a new registry called the "Matroska Horizontal Chroma Sitings" registry.
The values correspond to the unsigned integer `ChromaSitingHorz` value described in (#chromasitinghorz-element).

To register a new Horizontal Chroma Siting in this registry, one needs a Horizontal Chroma Siting value,
a description, a Change Controller, and
an optional Reference to a document describing the Horizontal Chroma Siting.

The Horizontal Chroma Sitings are to be allocated according to the "First Come First Served" policy [@!RFC8126]. Available values range from 3-18446744073709551615.

(#horizontal-chroma-siting-registry-table) shows the initial contents of the "Matroska Horizontal Chroma Sitings" registry.
The Change Controller for the initial entries is the IETF.

Horizontal Chroma Siting | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0 | unspecified | RFC 9559, (#chromasitinghorz-element)
1 | left collocated | RFC 9559, (#chromasitinghorz-element)
2 | half | RFC 9559, (#chromasitinghorz-element)
Table: Initial Contents of "Matroska Horizontal Chroma Sitings" Registry{#horizontal-chroma-siting-registry-table}


## Matroska Vertical Chroma Sitings Registry

IANA has created a new registry called the "Matroska Vertical Chroma Sitings" registry.
The values correspond to the unsigned integer `ChromaSitingVert` value described in (#chromasitingvert-element).

To register a new Vertical Chroma Siting in this registry, one needs a Vertical Chroma Siting value,
a description, a Change Controller, and
an optional Reference to a document describing the Vertical Chroma Siting.

The Vertical Chroma Sitings are to be allocated according to the "First Come First Served" policy [@!RFC8126]. Available values range from 3-18446744073709551615.

(#vertical-chroma-siting-registry-table) shows the initial contents of the "Matroska Vertical Chroma Sitings" registry.
The Change Controller for the initial entries is the IETF.

Vertical Chroma Siting | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0 | unspecified | RFC 9559, (#chromasitingvert-element)
1 | top collocated | RFC 9559, (#chromasitingvert-element)
2 | half | RFC 9559, (#chromasitingvert-element)
Table: Initial Contents of "Matroska Vertical Chroma Sitings" Registry{#vertical-chroma-siting-registry-table}


## Matroska Color Ranges Registry

IANA has created a new registry called the "Matroska Color Ranges" registry.
The values correspond to the unsigned integer `Range` value described in (#color-range-element).

To register a new Color Range in this registry, one needs a Color Range value,
a description, a Change Controller, and
a Reference to a document describing the Color Range.

The Color Ranges are to be allocated according to the "Specification Required" policy [@!RFC8126]. Available values range from 4-18446744073709551615.

(#color-range-registry-table) shows the initial contents of the "Matroska Color Ranges" registry.
The Change Controller for the initial entries is the IETF.

Color Range | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0 | unspecified | RFC 9559, (#color-range-element)
1 | broadcast range | RFC 9559, (#color-range-element)
2 | full range (no clipping) | RFC 9559, (#color-range-element)
3 | defined by MatrixCoefficients / TransferCharacteristics | RFC 9559, (#color-range-element)
Table: Initial Contents of "Matroska Color Ranges" Registry{#color-range-registry-table}


## Matroska Tags Target Types Registry

IANA has created a new registry called the "Matroska Tags Target Types" registry.
The values correspond to the unsigned integer `TargetTypeValue` value described in (#targettypevalue-element).

To register a new Tags Target Type in this registry, one needs a Tags Target Type value,
a description, a Change Controller, and
a Reference to a document describing the Tags Target Type.

The Tags Target Types are to be allocated according to the "Specification Required" policy [@!RFC8126]. Available values range from 71-18446744073709551615.

The value 0 is not valid for use as a Tags Target Type.

(#tags-target-type-registry-table) shows the initial contents of the "Matroska Tags Target Types" registry.
The Change Controller for the initial entries is the IETF.

Tags Target Type | Description            | Reference
----------:|:------------------------|:-------------------------------------------
70 | COLLECTION | RFC 9559, (#targettypevalue-element)
60 | EDITION / ISSUE / VOLUME / OPUS / SEASON / SEQUEL | RFC 9559, (#targettypevalue-element)
50 | ALBUM / OPERA / CONCERT / MOVIE / EPISODE | RFC 9559, (#targettypevalue-element)
40 | PART / SESSION | RFC 9559, (#targettypevalue-element)
30 | TRACK / SONG / CHAPTER | RFC 9559, (#targettypevalue-element)
20 | SUBTRACK / MOVEMENT / SCENE | RFC 9559, (#targettypevalue-element)
10 | SHOT | RFC 9559, (#targettypevalue-element)
Table: Initial Contents of "Matroska Tags Target Types" Registry{#tags-target-type-registry-table}


## Matroska Chapter Codec IDs Registry

IANA has created a new registry called the "Matroska Chapter Codec IDs" registry.
The values correspond to the unsigned integer `ChapProcessCodecID`, `ChapterTranslateCodec`, and `TrackTranslateCodec` values described in (#chapprocesscodecid-element).

To register a new Chapter Codec ID in this registry, one needs a Chapter Codec ID value,
a description, a Change Controller, and
a Reference to a document describing the Chapter Codec ID.

The Chapter Codec IDs are to be allocated according to the "Specification Required" policy [@!RFC8126]. Available values range from 2-18446744073709551615.

(#chapter-codec-id-registry-table) shows the initial contents of the "Matroska Chapter Codec IDs" registry.
The Change Controller for the initial entries is the IETF.

Chapter Codec ID | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0 | Matroska Script | RFC 9559, (#chapprocesscodecid-element)
1 | DVD-menu | RFC 9559, (#chapprocesscodecid-element)
Table: Initial Contents of "Matroska Chapter Codec IDs" Registry{#chapter-codec-id-registry-table}


## Matroska Projection Types Registry

IANA has created a new registry called the "Matroska Projection Types" registry.
The values correspond to the unsigned integer `ProjectionType` value described in (#projectiontype-element).

To register a new Projection Type in this registry, one needs a Projection Type value,
a description, a Change Controller, and
an optional Reference to a document describing the Projection Type.

The Projection Types are to be allocated according to the "First Come First Served" policy [@!RFC8126]. Available values range from 4-18446744073709551615.

(#projection-type-registry-table) shows the initial contents of the "Matroska Projection Types" registry.
The Change Controller for the initial entries is the IETF.

Projection Type | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0 | rectangular | RFC 9559, (#projectiontype-element)
1 | equirectangular | RFC 9559, (#projectiontype-element)
2 | cubemap | RFC 9559, (#projectiontype-element)
3 | mesh | RFC 9559, (#projectiontype-element)
Table: Initial Contents of "Matroska Projection Types" Registry{#projection-type-registry-table}


## Matroska Track Types Registry

IANA has created a new registry called the "Matroska Track Types" registry.
The values correspond to the unsigned integer `TrackType` value described in (#tracktype-element).

To register a new Track Type in this registry, one needs a Track Type value,
a description, a Change Controller, and
a Reference to a document describing the Track Type.

The Track Types are to be allocated according to the "Specification Required" policy [@!RFC8126]. Available values range from 34-18446744073709551615.

The value 0 is not valid for use as a Track Type.

(#track-type-registry-table) shows the initial contents of the "Matroska Track Types" registry.
The Change Controller for the initial entries is the IETF.

Track Type | Description            | Reference
----------:|:------------------------|:-------------------------------------------
1 | video | RFC 9559, (#tracktype-element)
2 | audio | RFC 9559, (#tracktype-element)
3 | complex | RFC 9559, (#tracktype-element)
16 | logo | RFC 9559, (#tracktype-element)
17 | subtitle | RFC 9559, (#tracktype-element)
18 | buttons | RFC 9559, (#tracktype-element)
32 | control | RFC 9559, (#tracktype-element)
33 | metadata | RFC 9559, (#tracktype-element)
Table: Initial Contents of "Matroska Track Types" Registry{#track-type-registry-table}


## Matroska Track Plane Types Registry

IANA has created a new registry called the "Matroska Track Plane Types" registry.
The values correspond to the unsigned integer `TrackPlaneType` value described in (#trackplanetype-element).

To register a new Track Plane Type in this registry, one needs a Track Plane Type value,
a description, a Change Controller, and
an optional Reference to a document describing the Track Plane Type.

The Track Plane Types are to be allocated according to the "First Come First Served" policy [@!RFC8126]. Available values range from 3-18446744073709551615.

(#track-plane-type-registry-table) shows the initial contents of the "Matroska Track Plane Types" registry.
The Change Controller for the initial entries is the IETF.

Track Plane Type | Description            | Reference
----------:|:------------------------|:-------------------------------------------
0 | left eye | RFC 9559, (#trackplanetype-element)
1 | right eye | RFC 9559, (#trackplanetype-element)
2 | background | RFC 9559, (#trackplanetype-element)
Table: Initial Contents of "Matroska Track Plane Types" Registry{#track-plane-type-registry-table}

