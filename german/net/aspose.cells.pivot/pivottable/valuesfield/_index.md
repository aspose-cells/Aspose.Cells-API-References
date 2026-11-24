---
title: "PivotTable.ValuesField"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable‑Eigenschaft. Gibt ein PivotField‑Objekt zurück, das alle Datenfelder in einer PivotTable darstellt. Nur lesbar. Es wird nur erstellt, wenn im Datenbereich zwei oder mehr Datenfelder vorhanden sind. Standardmäßig befindet es sich im Zeilenbereich. Sie können es mit der Methode PivotTable.AddFieldToArea in den Zeilen‑/Spaltenbereich ziehen."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/valuesfield/
---
## PivotTable.ValuesField property

Gibt ein [`PivotField`](../../pivotfield/)‑Objekt zurück, das alle Datenfelder in einer PivotTable darstellt. Nur lesbar. Es wird nur erstellt, wenn im Datenbereich zwei oder mehr Datenfelder vorhanden sind. Standardmäßig befindet es sich im Zeilenbereich. Sie können es mit der Methode PivotTable.AddFieldToArea() in den Zeilen‑/Spaltenbereich ziehen.

```csharp
public PivotField ValuesField { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyValuesFieldDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(1500);
            worksheet.Cells["A4"].PutValue("Product A");
            worksheet.Cells["B4"].PutValue("South");
            worksheet.Cells["C4"].PutValue(2000);
            worksheet.Cells["A5"].PutValue("Product B");
            worksheet.Cells["B5"].PutValue("North");
            worksheet.Cells["C5"].PutValue(1200);

            try
            {
                // Erstelle eine Pivot-Tabelle
                int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Felder zu Bereichen hinzufügen
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

                // Daten berechnen, um die Pivot-Tabelle zu füllen
                pivotTable.CalculateData();

                // Greifen Sie auf die ValuesField-Eigenschaft zu (schreibgeschützt)
                PivotField valuesField = pivotTable.ValuesField;

                if (valuesField != null)
                {
                    Console.WriteLine("ValuesField Name: " + valuesField.Name);
                    Console.WriteLine("ValuesField DisplayName: " + valuesField.DisplayName);
                    Console.WriteLine("ValuesField Position: " + valuesField.Position);
                    Console.WriteLine("ValuesField RegionType: " + valuesField.RegionType);
                    Console.WriteLine("ValuesField IsValuesField: " + valuesField.IsValuesField);
                }
                else
                {
                    Console.WriteLine("ValuesField is null - no data fields in the pivot table");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("PivotTableValuesFieldDemo.xlsx");
                Console.WriteLine("PivotTable with ValuesField demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


