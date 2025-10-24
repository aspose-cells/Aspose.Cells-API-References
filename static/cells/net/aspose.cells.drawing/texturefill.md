##Class TextureFill
Aspose.Cells.Drawing.TextureFill class. Encapsulates the object that represents texture fill format
## TextureFill class
Encapsulates the object that represents texture fill format
```csharp
public class TextureFill : Fill
```
## Properties
| Name | Description |
| --- | --- |
| [ImageData](../../aspose.cells.drawing/texturefill/imagedata/) { get; set; } | Gets and sets the image data of the fill. |
| [IsTiling](../../aspose.cells.drawing/texturefill/istiling/) { get; set; } | Indicates whether tile picture as texture. |
| [PicFormatOption](../../aspose.cells.drawing/texturefill/picformatoption/) { get; set; } | Gets or sets picture format option. |
| [PictureFormatType](../../aspose.cells.drawing/texturefill/pictureformattype/) { get; set; } | Gets and sets the picture format type. |
| [Scale](../../aspose.cells.drawing/texturefill/scale/) { get; set; } | Gets and sets the picture format scale. |
| [TilePicOption](../../aspose.cells.drawing/texturefill/tilepicoption/) { get; set; } | Gets or sets tile picture option. |
| [Transparency](../../aspose.cells.drawing/texturefill/transparency/) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [Type](../../aspose.cells.drawing/texturefill/type/) { get; set; } | Gets and sets the texture type |
## Methods
| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Inherited from [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Gets the hash code.(Inherited from [`Fill`](../fill/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class DrawingClassTextureFillDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to demonstrate texture fill
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 150, 300);
// Apply texture fill to the shape and get existing TextureFill instance
shape.Fill.FillType = FillType.Texture;
TextureFill textureFill = shape.Fill.TextureFill;
// Set built-in texture type
textureFill.Type = TextureType.BlueTissuePaper;
// Configure tiling options
textureFill.IsTiling = true;
TilePicOption tileOptions = new TilePicOption
{
ScaleX = 0.5,
ScaleY = 0.5,
OffsetX = 10,
OffsetY = 10
};
textureFill.TilePicOption = tileOptions;
// Set fill transparency and scaling
textureFill.Transparency = 0.2;
textureFill.Scale = 0.8;
// Save the workbook with texture fill applied
workbook.Save("TextureFillDemo.xlsx");
}
}
}
```
### See Also
* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
