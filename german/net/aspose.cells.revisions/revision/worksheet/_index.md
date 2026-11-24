---
title: "Revision.Worksheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Revision-Eigenschaft. Gibt das Arbeitsblatt zurück"
type: docs
url: /de/net/aspose.cells.revisions/revision/worksheet/
---
## Revision.Worksheet property

Gibt das Arbeitsblatt zurück.

```csharp
public Worksheet Worksheet { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Arbeitsblatteigenschaften festlegen
            worksheet.Name = "Demo Sheet";
            worksheet.IsGridlinesVisible = true;
            worksheet.DisplayZeros = false;
            worksheet.Zoom = 120;
            
            // Fügen Sie einige Daten hinzu, um Revisionen zu demonstrieren
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Schützen Sie das Arbeitsblatt, um die Nachverfolgung von Änderungen zu ermöglichen
            worksheet.Protect(ProtectionType.All);
            
            // Nehmen Sie eine Änderung vor, die als Revision verfolgt wird
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Speichern Sie die Arbeitsmappe, um Revisionen zu verfolgen
            workbook.Save("RevisionDemo.xlsx");
            
            // Laden Sie die Arbeitsmappe mit Revisionen
            Workbook workbookWithRevisions = new Workbook("RevisionDemo.xlsx");
            
            // Zugriff auf Revisionsprotokolle
            foreach (RevisionLog log in workbookWithRevisions.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    // Demonstrieren Sie den Zugriff auf die Worksheet-Eigenschaft von einer Revision
                    Console.WriteLine($"Revision Type: {revision.Type}");
                    Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");
                    Console.WriteLine($"Worksheet Index: {revision.Worksheet.Index}");
                    
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        Console.WriteLine($"Cell changed in worksheet '{cellChange.Worksheet.Name}': {cellChange.CellName}");
                    }
                }
            }
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


