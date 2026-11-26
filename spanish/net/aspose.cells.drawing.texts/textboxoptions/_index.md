---
title: "Clase TextBoxOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Texts.TextBoxOptions class. Representa las opciones de texto de la forma"
type: docs
url: /es/net/aspose.cells.drawing.texts/textboxoptions/
---
## TextBoxOptions class

Representa las opciones de texto de la forma

```csharp
public class TextBoxOptions
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllowTextToOverflow](../../aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/) { get; set; } | Si permite que el texto desborde la forma. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/textboxoptions/bottommarginpt/) { get; set; } | Devuelve el margen inferior en unidades de puntos |
| [LeftMarginPt](../../aspose.cells.drawing.texts/textboxoptions/leftmarginpt/) { get; set; } | Obtiene y establece el margen izquierdo en unidades de Puntos. |
| [ResizeToFitText](../../aspose.cells.drawing.texts/textboxoptions/resizetofittext/) { get; set; } | Indica si redimensionar la forma para ajustarse al texto |
| [RightMarginPt](../../aspose.cells.drawing.texts/textboxoptions/rightmarginpt/) { get; set; } | Obtiene y establece el margen derecho en unidades de Puntos. |
| [ShapeTextDirection](../../aspose.cells.drawing.texts/textboxoptions/shapetextdirection/) { get; set; } | Obtiene o establece la dirección de visualización del texto dentro de un cuerpo de texto dado. Corresponde a "Formato de forma - Opciones de texto - Cuadro de texto - Dirección del texto" en Excel |
| [ShapeTextVerticalAlignment](../../aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/) { get; set; } | Corresponde a "Formato de forma - Opciones de texto - Cuadro de texto - Alineación vertical" en Excel. |
| [TopMarginPt](../../aspose.cells.drawing.texts/textboxoptions/topmarginpt/) { get; set; } | Obtiene y establece el margen superior en unidades de Puntos. |
| [WrapTextInShape](../../aspose.cells.drawing.texts/textboxoptions/wraptextinshape/) { get; set; } | Especifica el ajuste de texto dentro de una forma. False - No se producirá ajuste en el cuerpo del texto. True - Se producirá ajuste en el cuerpo del texto. |

### Ejemplos

```csharp

[C#]
//Instanciando un objeto Workbook
Workbook workbook = new Workbook();
int index = workbook.Worksheets[0].TextBoxes.Add(0, 0, 350, 350);
Shape shape = workbook.Worksheets[0].TextBoxes[index];
shape.Text = "This is test.";

//realiza tu negocio

//Guardar el archivo de Excel.
workbook.Save("exmaple.xlsx");
```

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


