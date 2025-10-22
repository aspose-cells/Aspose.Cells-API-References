##ReflectionEffect Class
'ReflectionEffect class. Encapsulates the object that represents reflectioneffect in Go.'
## ReflectionEffect class
This class specifies a reflection effect.
```go
type ReflectionEffect struct  {
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
|[GetType](./gettype/) | Gets and sets the preset reflection effect. |
|[SetType](./settype/) | Gets and sets the preset reflection effect. |
|[GetTransparency](./gettransparency/) | Gets and sets the degree of the starting reflection transparency as a value from 0.0 (opaque) through 1.0 (clear). |
|[SetTransparency](./settransparency/) | Gets and sets the degree of the starting reflection transparency as a value from 0.0 (opaque) through 1.0 (clear). |
|[GetSize](./getsize/) | Gets and sets the end position (along the alpha gradient ramp) of the end alpha value,in unit of percentage |
|[SetSize](./setsize/) | Gets and sets the end position (along the alpha gradient ramp) of the end alpha value,in unit of percentage |
|[GetBlur](./getblur/) | Gets and sets the blur radius,in unit of points. |
|[SetBlur](./setblur/) | Gets and sets the blur radius,in unit of points. |
|[GetDirection](./getdirection/) | Gets and sets the direction of the alpha gradient ramp relative to the shape itself. |
|[SetDirection](./setdirection/) | Gets and sets the direction of the alpha gradient ramp relative to the shape itself. |
|[GetDistance](./getdistance/) | Gets and sets how far to distance the shadow,in unit of points. |
|[SetDistance](./setdistance/) | Gets and sets how far to distance the shadow,in unit of points. |
|[GetFadeDirection](./getfadedirection/) | Gets and sets the direction to offset the reflection. |
|[SetFadeDirection](./setfadedirection/) | Gets and sets the direction to offset the reflection. |
|[GetRotWithShape](./getrotwithshape/) | Gets and sets if the reflection should rotate with the shape. |
|[SetRotWithShape](./setrotwithshape/) | Gets and sets if the reflection should rotate with the shape. |
