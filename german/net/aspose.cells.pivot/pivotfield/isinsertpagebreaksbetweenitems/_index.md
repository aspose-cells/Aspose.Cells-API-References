---
title: "PivotField.IsInsertPageBreaksBetweenItems"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt an, ob nach jedem Element Seitenumbrüche eingefügt werden sollen. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/
---
## PivotField.IsInsertPageBreaksBetweenItems property

Gibt an, ob nach jedem Element Seitenumbrüche eingefügt werden sollen. Der Standardwert ist falsch.

```csharp
public bool IsInsertPageBreaksBetweenItems { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsInsertPageBreaksBetweenItemsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 7; i++)
            {
                worksheet.Cells["A" + i].PutValue("Category " + (i % 3 + 1));
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B7", "E3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Seitenanzahl vor dem Setzen der Eigenschaft prüfen
            SheetRender render1 = new SheetRender(worksheet, new ImageOrPrintOptions());
            Console.WriteLine("Page count before: " + render1.PageCount);

            // Setze die Eigenschaft IsInsertPageBreaksBetweenItems
            PivotField field = pivotTable.RowFields[0];
            field.IsInsertPageBreaksBetweenItems = true;
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Seitenanzahl nach dem Setzen der Eigenschaft prüfen
            SheetRender render2 = new SheetRender(worksheet, new ImageOrPrintOptions());
            Console.WriteLine("Page count after: " + render2.PageCount);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldIsInsertPageBreaksBetweenItemsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


