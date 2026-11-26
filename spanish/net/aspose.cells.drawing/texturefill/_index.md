---
title: "Clase TextureFill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.TextureFill. Encapsula el objeto que representa el formato de relleno de textura"
type: docs
url: /es/net/aspose.cells.drawing/texturefill/
---
## TextureFill class

Encapsula el objeto que representa el formato de relleno de textura.

```csharp
public class TextureFill : Fill
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ImageData](../../aspose.cells.drawing/texturefill/imagedata/) { get; set; } | Obtiene y establece los datos de imagen del relleno. |
| [IsTiling](../../aspose.cells.drawing/texturefill/istiling/) { get; set; } | Indica si la imagen se repite como textura. |
| [PicFormatOption](../../aspose.cells.drawing/texturefill/picformatoption/) { get; set; } | Obtiene o establece la opción de formato de imagen. |
| [PictureFormatType](../../aspose.cells.drawing/texturefill/pictureformattype/) { get; set; } | Obtiene y establece el tipo de formato de imagen. |
| [Scale](../../aspose.cells.drawing/texturefill/scale/) { get; set; } | Obtiene y establece la escala del formato de imagen. |
| [TilePicOption](../../aspose.cells.drawing/texturefill/tilepicoption/) { get; set; } | Obtiene o establece la opción de mosaico de imagen. |
| [Transparency](../../aspose.cells.drawing/texturefill/transparency/) { get; set; } | Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro). |
| [Type](../../aspose.cells.drawing/texturefill/type/) { get; set; } | Obtiene y establece el tipo de textura |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Hereda de [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Obtiene el código hash.(Hereda de [`Fill`](../fill/).) |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agrega una forma rectangular para demostrar el relleno de textura
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 150, 300);
            
            // Aplica el relleno de textura a la forma y obtén la instancia existente de TextureFill
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;
            
            // Establece el tipo de textura incorporado
            textureFill.Type = TextureType.BlueTissuePaper;
            
            // Configura las opciones de mosaico
            textureFill.IsTiling = true;
            TilePicOption tileOptions = new TilePicOption
            {
                ScaleX = 0.5,
                ScaleY = 0.5,
                OffsetX = 10,
                OffsetY = 10
            };
            textureFill.TilePicOption = tileOptions;
            
            // Establece la transparencia y el escalado del relleno
            textureFill.Transparency = 0.2;
            textureFill.Scale = 0.8;
            
            // Guarda el libro de trabajo con el relleno de textura aplicado
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


