---
title: "TextOptions.FarEastName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextOptions özelliği. FarEast adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textoptions/fareastname/
---
## TextOptions.FarEastName property

FarEast adını alır ve ayarlar.

```csharp
public string FarEastName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyFarEastNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir şekil ekleyin ve FarEastName yazı tipini ayarlayın
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            shape.Text = "Sample Text";
            shape.TextOptions.FarEastName = "宋体";

            // Doğrulamak için kaydedin ve yeniden yükleyin
            string outputPath = "output_FarEastName.xlsx";
            workbook.Save(outputPath);

            // Doğrulamak için yeniden yükle
            Workbook verifyWorkbook = new Workbook(outputPath);
            Aspose.Cells.Drawing.Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("FarEastName: " + verifyShape.TextOptions.FarEastName);
        }
    }
}
```

### Ayrıca Bakınız

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


