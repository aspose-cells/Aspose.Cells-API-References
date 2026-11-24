---
title: "Klasse HighlightChangesOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.HighlightChangesOptions Klasse. Stellt Optionen zum Hervorheben von Revisionen oder Änderungen in gemeinsam genutzten Excel-Dateien dar"
type: docs
url: /de/net/aspose.cells.revisions/highlightchangesoptions/
---
## HighlightChangesOptions class

Stellt Optionen zum Hervorheben von Revisionen oder Änderungen in freigegebenen Excel‑Dateien dar.

```csharp
public class HighlightChangesOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [HighlightChangesOptions](highlightchangesoptions/)(bool, bool) | Stellt Optionen zum Hervorheben von Revisionen oder Änderungen in freigegebenen Excel‑Dateien dar. |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsDemo
    {
        public static void HighlightChangesExample()
        {
            // Instanziiere ein Workbook-Objekt
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Rufe die Revisionsprotokolle ab
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Lege die Anzahl der Tage fest, um die Historie zu bewahren
            revisionLogs.DaysPreservingHistory = 30;

            // Erstelle HighlightChangesOptions
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);

            // Änderungen hervorheben
            revisionLogs.HighlightChanges(options);

            // Speichere die Arbeitsmappe mit hervorgehobenen Änderungen
            workbook.Save("HighlightedChangesWorkbook.xlsx");
            workbook.Save("HighlightedChangesWorkbook.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


