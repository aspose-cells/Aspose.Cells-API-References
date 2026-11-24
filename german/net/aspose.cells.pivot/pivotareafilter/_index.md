---
title: "Klasse PivotAreaFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotAreaFilter‑Klasse. Stellt den Filter von PivotArea für PivotTable dar."
type: docs
url: /de/net/aspose.cells.pivot/pivotareafilter/
---
## PivotAreaFilter class

Stellt den Filter von [`PivotArea`](../pivotarea/) für [`PivotTable`](../pivottable/) dar.

```csharp
public class PivotAreaFilter
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PivotAreaFilter](pivotareafilter/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FieldIndex](../../aspose.cells.pivot/pivotareafilter/fieldindex/) { get; } | Liest den Index des Feldes in den Quellfeldern, auf das sich dieser Filter bezieht. Ein Wert von -2 kennzeichnet das Wertefeld. |
| [Selected](../../aspose.cells.pivot/pivotareafilter/selected/) { get; set; } | Gibt an, ob dieses Feld eine Auswahl hat. Funktioniert nur, wenn die PivotTable in der Gliederungsansicht ist. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [IsSubtotalSet](../../aspose.cells.pivot/pivotareafilter/issubtotalset/)(PivotFieldSubtotalType) | Liest, welcher Zwischensumme für diesen Filter festgelegt ist. |
| [SetSubtotals](../../aspose.cells.pivot/pivotareafilter/setsubtotals/)(PivotFieldSubtotalType, bool) | Zwischensumme für den Filter. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten einrichten
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            
            // PivotTable erstellen - Rückgabewertbehandlung korrigieren
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // PivotAreaFilter erstellen und konfigurieren
            PivotAreaFilter filter = new PivotAreaFilter();
            filter.Selected = true;
            filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            
            // Methoden demonstrieren
            bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
            Console.WriteLine($"Sum subtotal visibility set: {isSumSet}");
            
            workbook.Save("PivotAreaFilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


