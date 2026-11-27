---
title: "Klass FileFontSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FileFontSource-klass. Representerar den enda TrueType‑teckensnittsfilen som lagras i filsystemet"
type: docs
url: /sv/net/aspose.cells/filefontsource/
---
## FileFontSource class

Representerar den enskilda TrueType-typsnittsfilen som lagras i filsystemet.

```csharp
public class FileFontSource : FontSourceBase
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [FileFontSource](filefontsource/)(string) | Konstruktor. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FilePath](../../aspose.cells/filefontsource/filepath/) { get; } | Sökväg till teckensnittsfilen. |
| override [Type](../../aspose.cells/filefontsource/type/) { get; } | Returnerar typen av teckensnittskälla. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFontSourceDemo
    {
        public static void FileFontSourceExample()
        {
            // Ange sökvägen till TrueType‑teckensnittsfilen
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";

            // Skapa en FileFontSource‑instans
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            // Visa teckensnittskällans typ och filsökväg
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            // Skapa ett Workbook‑objekt
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ange ett cellvärde
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Hello, Aspose!");

            // Applicera det anpassade teckensnittet på cellen
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont"; // Use the name of the font
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("FileFontSourceExample.xlsx");
            workbook.Save("FileFontSourceExample.pdf");
        }
    }
}
```

### Se även

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


