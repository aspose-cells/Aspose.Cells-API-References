---
title: "PivotPageFields.PivotPageFields"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotPageFields-Konstruktor. Stellt die Pivot-Seitenfeld-Elemente dar."
type: docs
url: /de/net/aspose.cells.pivot/pivotpagefields/pivotpagefields/
---
## PivotPageFields constructor

Stellt die Pivot-Seitenfeld-Elemente dar.

```csharp
public PivotPageFields()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotPageFieldsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["C3"].PutValue(2000);

            // Erstelle Pivot-Seitenfelder mit dem Konstruktor.
            PivotPageFields pageFields = new PivotPageFields();
            
            // Seitenfelder hinzufügen
            string[] items = { "Item1", "Item2" };
            pageFields.AddPageField(items);
            
            // Identifikation hinzufügen
            int[] itemIndexes = { 0, 1 };
            pageFields.AddIdentify(0, itemIndexes);

            // Pivot-Tabelle mit korrekten Parametern hinzufügen
            PivotTableCollection pivotTables = worksheet.PivotTables;
            string sourceData = "A1:C3";
            int index = pivotTables.Add(sourceData, "E5", "PivotTable1");

            // Speichere die Arbeitsmappe
            workbook.Save("PivotPageFieldsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


