##ControlPictureSizeMode Enum
'ControlPictureSizeMode enum. Encapsulates the object that represents controlpicturesizemode in Go.'
## ControlPictureSizeMode Enum
Represents how to display the picture.
```go
type ControlPictureSizeMode int32
```
## Fields
| Field | Description |
| --- | --- |
|[Clip](./clip/) | Crops any part of the picture that is larger than the control's boundaries. |
|[Stretch](./stretch/) | Stretches the picture to fill the control's area.This setting distorts the picture in either the horizontal or vertical direction. |
|[Zoom](./zoom/) | Enlarges the picture, but does not distort the picture in either the horizontal or vertical direction. |
