##TilePicOption Class
'TilePicOption class. Encapsulates the object that represents tilepicoption in Go.'
## TilePicOption class
Represents tile picture as texture.
```go
type TilePicOption struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewTilePicOption](./newtilepicoption/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetOffsetX](./getoffsetx/) | Gets or sets the X offset for tiling picture. |
|[SetOffsetX](./setoffsetx/) | Gets or sets the X offset for tiling picture. |
|[GetOffsetY](./getoffsety/) | Gets or sets the Y offset for tiling picture. |
|[SetOffsetY](./setoffsety/) | Gets or sets the Y offset for tiling picture. |
|[GetScaleX](./getscalex/) | Gets or sets the X scale for tiling picture. |
|[SetScaleX](./setscalex/) | Gets or sets the X scale for tiling picture. |
|[GetScaleY](./getscaley/) | Gets or sets the Y scale for tiling picture. |
|[SetScaleY](./setscaley/) | Gets or sets the Y scale for tiling picture. |
|[GetMirrorType](./getmirrortype/) | Gets or sets the mirror type for tiling. |
|[SetMirrorType](./setmirrortype/) | Gets or sets the mirror type for tiling. |
|[GetAlignmentType](./getalignmenttype/) | Gets or sets the alignment for tiling. |
|[SetAlignmentType](./setalignmenttype/) | Gets or sets the alignment for tiling. |
