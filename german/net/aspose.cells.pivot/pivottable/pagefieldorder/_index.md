---
title: "PivotTable.PageFieldOrder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt die Reihenfolge zurück und legt sie fest, in der Seitenfelder zum Layout der PivotTable-Berichte hinzugefügt werden"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/pagefieldorder/
---
## PivotTable.PageFieldOrder property

Liest und legt die Reihenfolge fest, in der Seitenfelder zum Layout des PivotTable-Berichts hinzugefügt werden.

```csharp
public PrintOrderType PageFieldOrder { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPageFieldOrderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Region";
            cells["D1"].Value = "Sales";
            
            // Beispiel-Datenzeilen hinzufügen
            for (int i = 2; i <= 10; i++)
            {
                cells[$"A{i}"].Value = $"Category{(i % 3) + 1}";
                cells[$"B{i}"].Value = $"Product{(i % 4) + 1}";
                cells[$"C{i}"].Value = $"Region{(i % 2) + 1}";
                cells[$"D{i}"].Value = i * 100;
            }

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:D11", "F5", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Felder zu Bereichen hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields["Category"]);
            pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields["Region"]);
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields["Product"]);
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields["Sales"]);

            // Setze die Reihenfolge der Seitenfelder und die Zeilenumbruchanzahl
            pivotTable.PageFieldOrder = PrintOrderType.DownThenOver;
            pivotTable.PageFieldWrapCount = 2;

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTablePageFieldOrderDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PrintOrderType](../../../aspose.cells/printordertype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


