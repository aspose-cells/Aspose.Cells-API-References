---
title: "PivotItem.IsFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotItem-Eigenschaft. Gibt an, ob dieses Pivot-Element ein berechnetes Formelelement ist"
type: docs
url: /de/net/aspose.cells.pivot/pivotitem/isformula/
---
## PivotItem.IsFormula property

Gibt an, ob dieses Pivot‑Element ein berechnetes Formelelement ist.

```csharp
[Obsolete("Use PivotItem.IsCalculatedItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsFormula { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft PivotItem.IsCalculatedItem. Diese Eigenschaft wird 12 Monate später, seit November 2024, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Holen Sie das erste Pivot-Element
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // Zeigen Sie den aktuellen IsFormula-Wert an (veraltete Eigenschaft)
            Console.WriteLine("Current IsFormula value: " + pivotItem.IsFormula);

            // Setzen Sie einen neuen Wert für IsFormula (veraltete Eigenschaft)
            pivotItem.IsFormula = true;

            // Demonstrieren Sie die Wirkung – dies würde das Pivot-Element als Formelelement markieren
            Console.WriteLine("After setting IsFormula to true: " + pivotItem.IsFormula);

            // Hinweis: In der realen Anwendung sollten Sie stattdessen IsCalculatedItem verwenden, da IsFormula veraltet ist
            Console.WriteLine("IsCalculatedItem (recommended property): " + pivotItem.IsCalculatedItem);

            // Ergebnis speichern
            workbook.Save("PivotItemPropertyIsFormulaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


