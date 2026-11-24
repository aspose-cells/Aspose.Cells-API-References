---
title: "PivotTable.IsMultipleFieldFilters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt einen booleschen Wert an, der angibt, ob die Felder einer PivotTable mehrere Filter haben können."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/ismultiplefieldfilters/
---
## PivotTable.IsMultipleFieldFilters property

Gibt einen booleschen Wert an, der angibt, ob die Felder einer PivotTable mehrere Filter haben können.

```csharp
[Obsolete("Use PivotTable.AllowMultipleFiltersPerField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsMultipleFieldFilters { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die PivotTable.AllowMultipleFiltersPerField-Eigenschaft. Diese Methode wird 12 Monate später, seit Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyIsMultipleFieldFiltersDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("Fruit");
            worksheet.Cells["B3"].PutValue("Fruit");
            worksheet.Cells["B4"].PutValue("Fruit");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Erstelle eine Pivot-Tabelle
            int index = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Zeige den aktuellen Wert von IsMultipleFieldFilters an
            Console.WriteLine("Current IsMultipleFieldFilters value: " + pivotTable.IsMultipleFieldFilters);

            // Setze IsMultipleFieldFilters auf true, um mehrere Filter pro Feld zu erlauben
            pivotTable.IsMultipleFieldFilters = true;
            Console.WriteLine("IsMultipleFieldFilters set to: " + pivotTable.IsMultipleFieldFilters);

            // Aktualisiere und berechne die Pivot-Tabelle
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTablePropertyIsMultipleFieldFiltersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


