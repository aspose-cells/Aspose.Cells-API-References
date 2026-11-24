---
title: "PivotTable.GrandTotalName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt die Bezeichnung zurück, die in der Überschrift der Gesamtsummenspalte oder -zeile angezeigt wird. Der Standardwert ist die Zeichenfolge Grand Total"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/grandtotalname/
---
## PivotTable.GrandTotalName property

Gibt die Bezeichnung zurück, die in der Überschrift der Gesamtsumme‑Spalte oder -Zeile angezeigt wird. Der Standardwert ist der String "Grand Total".

```csharp
public string GrandTotalName { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyGrandTotalNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Laptop";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Laptop";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 1500;
            
            worksheet.Cells["A4"].Value = "Phone";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["C4"].Value = 800;
            
            worksheet.Cells["A5"].Value = "Phone";
            worksheet.Cells["B5"].Value = "South";
            worksheet.Cells["C5"].Value = 1200;

            // Erstelle eine Pivot-Tabelle
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Zeilen- und Datenfelder hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Anzeige des aktuellen GrandTotalName-Werts
            Console.WriteLine("Current GrandTotalName: " + pivotTable.GrandTotalName);

            // GrandTotalName ändern
            pivotTable.GrandTotalName = "Total Summary";

            // Daten berechnen und die Pivot-Tabelle aktualisieren
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableGrandTotalNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


