---
title: "Workbook.AcceptAllRevisions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Akzeptiert alle nachverfolgten Änderungen in der Arbeitsmappe"
type: docs
url: /de/net/aspose.cells/workbook/acceptallrevisions/
---
## Workbook.AcceptAllRevisions method

Akzeptiert alle nachverfolgten Änderungen in der Arbeitsmappe.

```csharp
public void AcceptAllRevisions()
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAcceptAllRevisionsDemo
    {
        public static void Run()
        {
            // Arbeitsmappe mit Revisionen erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Revisionen hinzufügen (Nachverfolgung muss zuerst in Excel aktiviert sein)
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Mit Revisionen speichern
            string sourcePath = "source_with_revisions.xlsx";
            workbook.Save(sourcePath, SaveFormat.Xlsx);
            
            // Arbeitsmappe erneut öffnen
            workbook = new Workbook(sourcePath);
            
            // Prüfen, ob Revisionen vorhanden sind, und sie akzeptieren
            if (workbook.HasRevisions)
            {
                Console.WriteLine("Workbook has revisions. Accepting all...");
                workbook.AcceptAllRevisions();
                
                // Speichern ohne Revisionen
                string destPath = "output_no_revisions.xlsx";
                workbook.Save(destPath, SaveFormat.Xlsx);
                Console.WriteLine("Revisions accepted and saved to: " + destPath);
            }
            else
            {
                Console.WriteLine("Workbook has no revisions.");
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


