---
title: "Klass FontFileDataInfo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FontFileDataInfo-klass. Representerar datainformation för teckensnittsfilens data"
type: docs
url: /sv/net/aspose.cells/fontfiledatainfo/
---
## FontFileDataInfo class

Representerar datainformation för teckensnittsfilens data.

```csharp
public class FontFileDataInfo
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Data](../../aspose.cells/fontfiledatainfo/data/) { get; } | Hämtar binärdata för teckensnittsfilen. |
| [FormatType](../../aspose.cells/fontfiledatainfo/formattype/) { get; } | Hämtar teckensnittets formattyp för teckensnittsfilen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassFontFileDataInfoDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempel: Laddar teckensnittsfilens data
            string fontFilePath = "arial.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Obs: FontFileDataInfo kan inte instansieras direkt eftersom den saknar offentlig konstruktor
            // och dess egenskaper är skrivskyddade. I ett verkligt scenario skulle du få en instans
            // från en annan API‑metod (t.ex. FontConfigs.GetFontFileDataInfo())
            FontFileDataInfo fontInfo = null; // Would be populated by API call in real scenario

            // Demonstrera hur egenskaper skulle användas om vi hade en instans
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
                Console.WriteLine("Font data length: " + (fontInfo.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            }

            // Demonstrera integration med Workbook
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Spara arbetsboken
            workbook.Save("FontFileDataInfoDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


