---
title: "Enum DirectoryType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DirectoryType enum. Representerar katalogtypen för filnamnet"
type: docs
url: /sv/net/aspose.cells/directorytype/
---
## DirectoryType enumeration

Representerar katalogtypen för filnamnet.

```csharp
public enum DirectoryType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Volume | `0` | Representerar en MS-DOS-enhetsbokstav. Den följs av enhetsbokstaven. Eller UNC-filnamn, såsom \\server\share\myfile.xls |
| SameVolume | `1` | Indikerar att källarboken ligger på samma enhet som den beroende arbetsboken (enhetsbokstaven utelämnas) |
| DownDirectory | `2` | Indikerar att källarboken ligger i en underkatalog till den aktuella katalogen. |
| UpDirectory | `3` | Indikerar att källarboken ligger i den överordnade katalogen till den aktuella katalogen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DirectoryTypeDemo
    {
        public static void DirectoryTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Lägg till en extern länk till arbetsboken
            string externalFileName = "externalWorkbook.xlsx";
            string[] sheetNames = { "Sheet1" };

            // Lägg till extern länk med DirectoryType.Volume
            int linkIndex = workbook.Worksheets.ExternalLinks.Add(DirectoryType.Volume, externalFileName, sheetNames);

            // Hämta den tillagda externa länken
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[linkIndex];

            // Skriv ut detaljerna för den externa länken
            Console.WriteLine("External Link Details:");
            Console.WriteLine("File Name: " + externalLink.DataSource);

            // Spara arbetsboken
            workbook.Save("DirectoryTypeExample.xlsx");
            workbook.Save("DirectoryTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


