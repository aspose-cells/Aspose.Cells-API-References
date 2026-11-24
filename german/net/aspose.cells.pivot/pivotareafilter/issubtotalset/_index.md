---
title: "PivotAreaFilter.IsSubtotalSet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotAreaFilter-Methode. Gibt an, welche Zwischensumme für diesen Filter gesetzt ist"
type: docs
url: /de/net/aspose.cells.pivot/pivotareafilter/issubtotalset/
---
## PivotAreaFilter.IsSubtotalSet method

Liest, welcher Zwischensumme für diesen Filter festgelegt ist.

```csharp
public bool IsSubtotalSet(PivotFieldSubtotalType subtotalType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Der Typ der Zwischensummenfunktion. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaFilterMethodIsSubtotalSetWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // PivotTable hinzufügen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Füge ein Zeilenfeld hinzu und konfiguriere Zwischensummen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields["Category"];
            rowField.IsAutoSubtotals = true;
            rowField.SetSubtotals(PivotFieldSubtotalType.Automatic, true);

            // Erstelle einen Pivotbereich und prüfe die Zwischensummeneinstellung
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            
            // Demonstriere die Verwendung von IsSubtotalSet
            bool isSubtotalSet = pivotArea.Filters[0].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
            Console.WriteLine($"Is Automatic subtotal set: {isSubtotalSet}");

            // Speichere die Arbeitsmappe
            workbook.Save("PivotSubtotalDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


