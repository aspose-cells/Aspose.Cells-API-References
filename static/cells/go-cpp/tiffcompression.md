##TiffCompression Enum
'TiffCompression enum. Encapsulates the object that represents tiffcompression in Go.'
## TiffCompression Enum
Specifies what type of compression to apply when saving images into TIFF format file.
```go
type TiffCompression int32
```
## Fields
| Field | Description |
| --- | --- |
|[CompressionNone](./compressionnone/) | Specifies no compression. |
|[CompressionRle](./compressionrle/) | Specifies the RLE compression scheme. |
|[CompressionLZW](./compressionlzw/) | Specifies the LZW compression scheme. |
|[CompressionCCITT3](./compressionccitt3/) | Specifies the CCITT3 compression scheme. |
|[CompressionCCITT4](./compressionccitt4/) | Specifies the CCITT4 compression scheme. |
