---
title: "Enum MsoDrawingType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.MsoDrawingType enum. Ofis çizim nesneleri türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/msodrawingtype/
---
## MsoDrawingType enumeration

Office çizim nesneleri türünü temsil eder.

```csharp
public enum MsoDrawingType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Group | `0` | Grup |
| Line | `1` | Çizgi |
| Rectangle | `2` | Dikdörtgen |
| Oval | `3` | Oval |
| Arc | `4` | Yay |
| Chart | `5` | Grafik |
| TextBox | `6` | TextBox |
| Button | `7` | Düğme |
| Picture | `8` | Resim |
| Polygon | `9` | Poligon |
| CheckBox | `11` | CheckBox |
| RadioButton | `12` | RadioButton |
| Label | `14` | Etiket |
| DialogBox | `15` | DialogBox |
| Spinner | `16` | Spinner |
| ScrollBar | `17` | ScrollBar |
| ListBox | `18` | ListBox |
| GroupBox | `19` | GroupBox |
| ComboBox | `20` | ComboBox |
| Comment | `25` | Yorum |
| OleObject | `24` | OleObject |
| CellsDrawing | `30` | Yalnızca şablon dosyasında çizim nesnesini korumak için. |
| Unknown | `29` | Yalnızca xlsx dosyasında çizim nesnesini korumak için. |
| Slicer | `31` | Slicer |
| WebExtension | `32` | Web uzantısı |
| SmartArt | `33` | Smart Art |
| CustomXml | `34` | Özel xml şekli, örneğin Ink. |
| Timeline | `35` | Zaman Çizelgesi |
| Model3D | `36` | 3D Modeli |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoDrawingTypeDemo
    {
        public static void MsoDrawingTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir dikdörtgen şekli ekle
            Shape rectangle = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 200);
            rectangle.Name = "MyRectangle";
            rectangle.AlternativeText = "This is a rectangle shape";

            // Çalışma sayfasına bir oval şekil ekle
            Shape oval = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 5, 0, 5, 0, 100, 200);
            oval.Name = "MyOval";
            oval.AlternativeText = "This is an oval shape";

            // Çalışma sayfasına bir çizgi şekli ekle
            Shape line = worksheet.Shapes.AddShape(MsoDrawingType.Line, 8, 0, 8, 0, 100, 200);
            line.Name = "MyLine";
            line.AlternativeText = "This is a line shape";

            // Çalışma sayfasına bir metin kutusu şekli ekle
            Shape textBox = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 11, 0, 11, 0, 100, 200);
            textBox.Name = "MyTextBox";
            textBox.AlternativeText = "This is a textbox shape";
            textBox.Text = "Hello, Aspose.Cells!";

            // Şekillerin adlarını ve türlerini çıktı olarak ver
            foreach (Shape shape in worksheet.Shapes)
            {
                Console.WriteLine($"Shape Name: {shape.Name}, Shape Type: {shape.MsoDrawingType}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("MsoDrawingTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


