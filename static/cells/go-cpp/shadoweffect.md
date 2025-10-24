##ShadowEffect Class
'ShadowEffect class. Encapsulates the object that represents shadoweffect in Go.'
## ShadowEffect class
This class specifies the shadow effect of the chart element or shape.
```go
type ShadowEffect struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetPresetType](./getpresettype/) | Gets and sets the preset shadow type of the shadow. |
|[SetPresetType](./setpresettype/) | Gets and sets the preset shadow type of the shadow. |
|[GetColor](./getcolor/) | Gets and sets the color of the shadow. |
|[SetColor](./setcolor/) | Gets and sets the color of the shadow. |
|[GetTransparency](./gettransparency/) | Gets and sets the degree of transparency of the shadow. Range from 0.0 (opaque) to 1.0 (clear). |
|[SetTransparency](./settransparency/) | Gets and sets the degree of transparency of the shadow. Range from 0.0 (opaque) to 1.0 (clear). |
|[GetSize](./getsize/) | Gets and sets the size of the shadow. Range from 0 to 2.0.Meaningless in inner shadow. |
|[SetSize](./setsize/) | Gets and sets the size of the shadow. Range from 0 to 2.0.Meaningless in inner shadow. |
|[GetBlur](./getblur/) | Gets and sets the blur of the shadow. Range from 0 to 100 points. |
|[SetBlur](./setblur/) | Gets and sets the blur of the shadow. Range from 0 to 100 points. |
|[GetAngle](./getangle/) | Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
|[SetAngle](./setangle/) | Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
|[GetDistance](./getdistance/) | Gets and sets the distance of the shadow. Range from 0 to 200 points. |
|[SetDistance](./setdistance/) | Gets and sets the distance of the shadow. Range from 0 to 200 points. |
