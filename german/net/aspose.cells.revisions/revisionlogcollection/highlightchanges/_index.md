---
title: "RevisionLogCollection.HighlightChanges"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionLogCollection-Methode. Hebt Änderungen des gemeinsamen Arbeitsbuchs hervor"
type: docs
url: /de/net/aspose.cells.revisions/revisionlogcollection/highlightchanges/
---
## RevisionLogCollection.HighlightChanges method

Hebt Änderungen der freigegebenen Arbeitsmappe hervor.

```csharp
public void HighlightChanges(HighlightChangesOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | HighlightChangesOptions | Legen Sie die Optionen zum Filtern fest, welche Änderungen verfolgt werden sollen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionMethodHighlightChangesWithHighlightChangesOptionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einige Beispieldaten und Revisionen hinzu
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Änderungen mit Optionen hervorheben
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            workbook.Worksheets.RevisionLogs.HighlightChanges(options);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HighlightChangesOptions](../../highlightchangesoptions/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


