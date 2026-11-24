---
title: "Klasse ExternalLink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalLink-Klasse. Repräsentiert einen externen Link in einer Arbeitsmappe"
type: docs
url: /de/net/aspose.cells/externallink/
---
## ExternalLink class

Stellt einen externen Link in einem Arbeitsblatt dar.

```csharp
public class ExternalLink
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DataSource](../../aspose.cells/externallink/datasource/) { get; set; } | Repräsentiert die Datenquelle des externen Links. |
| [IsReferred](../../aspose.cells/externallink/isreferred/) { get; } | Gibt an, ob dieser externe Link von anderen referenziert wird. |
| [IsVisible](../../aspose.cells/externallink/isvisible/) { get; } | Gibt an, ob dieser externe Link in MS Excel sichtbar ist. |
| [OriginalDataSource](../../aspose.cells/externallink/originaldatasource/) { get; set; } | Repräsentiert die gespeicherte Datenquelle des externen Links. |
| [PathType](../../aspose.cells/externallink/pathtype/) { get; } | Erhalte den Pfadtyp dieses externen Links |
| [Type](../../aspose.cells/externallink/type/) { get; } | Ermittelt den Typ des externen Links. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddExternalName](../../aspose.cells/externallink/addexternalname/)(string, string) | Fügt einen externen Namen hinzu. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkDemo
    {
        public static void ExternalLinkExample()
        {
            // Öffnen Sie eine Datei mit externen Links
            Workbook workbook = new Workbook("UpdatedExternalLinkExample_original.xlsx");

            // Abrufen des externen Links 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Eigenschaften des externen Links anzeigen
            Console.WriteLine("External Link Type: " + externalLink.Type);
            Console.WriteLine("Path Type: " + externalLink.PathType);
            Console.WriteLine("Original Data Source: " + externalLink.OriginalDataSource);
            Console.WriteLine("Data Source: " + externalLink.DataSource);
            Console.WriteLine("Is Referred: " + externalLink.IsReferred);
            Console.WriteLine("Is Visible: " + externalLink.IsVisible);

            // Ändern Sie die Datenquelle des externen Links
            externalLink.DataSource = "d:\\linktest.xls";

            // Füge einen externen Namen zum externen Link hinzu
            externalLink.AddExternalName("ExternalName", "Sheet1!A1");

            // Speichere die Arbeitsmappe
            workbook.Save("UpdatedExternalLinkExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


