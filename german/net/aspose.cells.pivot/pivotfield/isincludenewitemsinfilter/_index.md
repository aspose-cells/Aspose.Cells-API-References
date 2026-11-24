---
title: "PivotField.IsIncludeNewItemsInFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt an, ob neue Elemente in das Feld im manuellen Filter aufgenommen werden sollen. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/
---
## PivotField.IsIncludeNewItemsInFilter property

Gibt an, ob neue Elemente in das Feld im manuellen Filter aufgenommen werden sollen. Der Standardwert ist falsch.

```csharp
public bool IsIncludeNewItemsInFilter { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsIncludeNewItemsInFilterDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Rufen Sie das Pivot‑Feld ab und setzen Sie IsIncludeNewItemsInFilter
            PivotField field = pivotTable.RowFields[0];
            field.IsIncludeNewItemsInFilter = true;
            
            // Geben Sie den Eigenschaftswert aus
            Console.WriteLine("IsIncludeNewItemsInFilter: " + field.IsIncludeNewItemsInFilter);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldPropertyIsIncludeNewItemsInFilterDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


