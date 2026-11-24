---
title: "PivotField.OriginalItems"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Ruft die ursprünglichen Basiselemente ab"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/originalitems/
---
## PivotField.OriginalItems property

Die ursprünglichen Basiselemente abrufen;

```csharp
public string[] OriginalItems { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyOriginalItemsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("AsposeGroupedField2.xlsx");
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die erste Pivot-Tabelle zu.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Auf das erste Zeilenfeld zugreifen
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Ursprüngliche Elemente und gruppierte Elemente anzeigen
            Console.WriteLine("Original Item[0]: " + pivotField.OriginalItems[0]);
            Console.WriteLine("Grouped Item[0]: " + pivotField.Items[0]);
            
            // Speichere die geänderte Arbeitsmappe
            workbook.Save("PivotFieldOriginalItemsDemo_Output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


