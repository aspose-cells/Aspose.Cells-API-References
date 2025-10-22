##OoxmlCompressionType Enum
'OoxmlCompressionType enum. Encapsulates the object that represents ooxmlcompressiontype in Go.'
## OoxmlCompressionType Enum
The Ooxml compression type
```go
type OoxmlCompressionType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Level1](./level1/) | The fastest but least effective compression. |
|[Level2](./level2/) | A little slower, but better, than level 1. |
|[Level3](./level3/) | A little slower, but better, than level 2. |
|[Level4](./level4/) | A little slower, but better, than level 3. |
|[Level5](./level5/) | A little slower than level 4, but with better compression. |
|[Level6](./level6/) | A good balance of speed and compression efficiency. |
|[Level7](./level7/) | Pretty good compression! |
|[Level8](./level8/) | Better compression than Level7! |
|[Level9](./level9/) | The "best" compression, where best means greatest reduction in size of the input data stream.This is also the slowest compression. |
