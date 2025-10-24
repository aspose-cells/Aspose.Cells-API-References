##ShapePropertyCollection Class
'ShapePropertyCollection class. Encapsulates the object that represents shapepropertycollection in Go.'
## ShapePropertyCollection class
This class specifies the visual shape properties for a chart element or shape.
```go
type ShapePropertyCollection struct  {
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
|[GetGlowEffect](./getgloweffect/) | Represents a GlowEffect object that specifies glow effect for the chart element or shape. |
|[ClearGlowEffect](./cleargloweffect/) | Clears the glow effect of the shape. |
|[HasGlowEffect](./hasgloweffect/) | Indicates if the shape has glow effect data. |
|[GetFormat3D](./getformat3d/) | Represents a Format3D object that specifies 3D shape properties for the chart element or shape. |
|[HasFormat3D](./hasformat3d/) | Indicates if the shape has 3d format data. |
|[ClearFormat3D](./clearformat3d/) | Clears the 3D shape properties of the shape. |
|[GetSoftEdgeRadius](./getsoftedgeradius/) | Gets and sets the radius of blur to apply to the edges, in unit of points. |
|[SetSoftEdgeRadius](./setsoftedgeradius/) | Gets and sets the radius of blur to apply to the edges, in unit of points. |
|[GetShadowEffect](./getshadoweffect/) | Represents a ShadowEffect object that specifies shadow effect for the chart element or shape. |
|[ClearShadowEffect](./clearshadoweffect/) | Clears the shadow effect of the chart element or shape. |
|[HasShadowEffect](./hasshadoweffect/) | Indicates if the shape has shadow effect data. |
