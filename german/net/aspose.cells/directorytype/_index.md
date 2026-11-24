---
title: "Enum DirectoryType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DirectoryType Enum. Stellt den Verzeichnistyp des Dateinamens dar"
type: docs
url: /de/net/aspose.cells/directorytype/
---
## DirectoryType enumeration

Stellt den Verzeichnistyp des Dateinamens dar.

```csharp
public enum DirectoryType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Volume | `0` | Stellt einen MS-DOS-Laufwerksbuchstaben dar. Er wird vom Laufwerksbuchstaben gefolgt. Oder UNC-Dateinamen, wie \\server\share\myfile.xls |
| SameVolume | `1` | Gibt an, dass die Quellarbeitsmappe sich auf demselben Laufwerk wie die abhängige Arbeitsmappe befindet (der Laufwerksbuchstabe wird weggelassen) |
| DownDirectory | `2` | Gibt an, dass die Quellarbeitsmappe in einem Unterverzeichnis des aktuellen Verzeichnisses liegt. |
| UpDirectory | `3` | Gibt an, dass die Quellarbeitsmappe im übergeordneten Verzeichnis des aktuellen Verzeichnisses liegt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DirectoryTypeDemo
    {
        public static void DirectoryTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Fügen Sie dem Arbeitsbuch einen externen Link hinzu
            string externalFileName = "externalWorkbook.xlsx";
            string[] sheetNames = { "Sheet1" };

            // Fügen Sie einen externen Link mit DirectoryType.Volume hinzu
            int linkIndex = workbook.Worksheets.ExternalLinks.Add(DirectoryType.Volume, externalFileName, sheetNames);

            // Rufen Sie den hinzugefügten externen Link ab
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[linkIndex];

            // Geben Sie die Details des externen Links aus
            Console.WriteLine("External Link Details:");
            Console.WriteLine("File Name: " + externalLink.DataSource);

            // Speichere die Arbeitsmappe
            workbook.Save("DirectoryTypeExample.xlsx");
            workbook.Save("DirectoryTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


