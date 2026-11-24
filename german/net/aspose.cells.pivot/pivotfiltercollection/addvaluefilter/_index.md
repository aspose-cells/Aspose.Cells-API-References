---
title: "PivotFilterCollection.AddValueFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFilterCollection-Methode. Filtert nach Werten des Daten-Pivotfelds"
type: docs
url: /de/net/aspose.cells.pivot/pivotfiltercollection/addvaluefilter/
---
## PivotFilterCollection.AddValueFilter method

Filtert nach Werten des Daten-Pivotfelds.

```csharp
public PivotFilter AddValueFilter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type, 
    double value1, double value2)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| baseFieldIndex | Int32 | Der Index des Feldes in der Quelle. |
| valueFieldIndex | Int32 | Der Index des Wertefelds im Wertebereich. |
| Typ | PivotFilterType | Der Typ der zu filternden Daten. |
| value1 | Double | Der Wert der Filterbedingung |
| value2 | Double | Der obere Grenzwert der Zwischenfilterbedingung |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddValueFilterWithInt32Int32PivotFilterTypeDoublDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Widget";
            worksheet.Cells["A3"].Value = "Gadget";
            worksheet.Cells["A4"].Value = "Thingy";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["B2"].Value = 15.99;
            worksheet.Cells["B3"].Value = 24.99;
            worksheet.Cells["B4"].Value = 9.99;

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // Wertfilter hinzufügen, um Produkte anzuzeigen, die zwischen $10 und $20 kosten
                PivotFilter filter = filters.AddValueFilter(
                    baseFieldIndex: 0,
                    valueFieldIndex: 1,
                    type: PivotFilterType.ValueBetween,
                    value1: 10.0,
                    value2: 20.0
                );

                Console.WriteLine($"Value filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding value filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddValueFilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


