---
title: "ExternalLink.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalLink-Eigenschaft. Gibt an, ob dieser externe Link in MS Excel sichtbar ist"
type: docs
url: /de/net/aspose.cells/externallink/isvisible/
---
## ExternalLink.IsVisible property

Gibt an, ob dieser externe Link in MS Excel sichtbar ist.

```csharp
public bool IsVisible { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit externen Verknüpfungen
            Workbook workbook = new Workbook();
            
            // Füge einige Daten zum ersten Arbeitsblatt hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("External Link Demo");
            
            // Erstellen Sie eine neue Arbeitsmappe, um sie als Quelle für externe Links zu verwenden
            Workbook externalWorkbook = new Workbook();
            externalWorkbook.Worksheets[0].Cells["A1"].PutValue(100);
            externalWorkbook.Save("external_data.xlsx");
            
            // Fügen Sie eine externe Linkreferenz hinzu
            workbook.Worksheets[0].Cells["B1"].Formula = "='[external_data.xlsx]Sheet1'!A1";
            
            // Überprüfen Sie externe Links (sie werden beim Laden von Formeln automatisch erstellt)
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link visibility: {link.IsVisible}");
                Console.WriteLine($"External link data source: {link.DataSource}");
            }
            
            // Erstellen Sie eine weitere Arbeitsmappe, um das Laden einer vorhandenen Datei zu demonstrieren
            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("=SUM([example.xls]Sheet1!A1:A10)");
            
            // Speichern und erneut laden, um externe Links zu demonstrieren
            workbook2.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Überprüfen Sie externe Links in der geladenen Arbeitsmappe
            foreach (ExternalLink link in loadedWorkbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link URL: {link.DataSource}, Visible: {link.IsVisible}");
            }
        }
    }
}
```

### Siehe auch

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


