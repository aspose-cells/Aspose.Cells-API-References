---
title: "PivotTable.SourceType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt den Datentyp der Datenquelle der Pivot-Tabelle zurück."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/sourcetype/
---
## PivotTable.SourceType property

Liest den Typ der Datenquelle der Pivot-Tabelle.

```csharp
public PivotTableSourceType SourceType { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertySourceTypeDemo
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
            
            worksheet.Cells["A2"].Value = "Product A";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Product B";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 2000;
            
            worksheet.Cells["A4"].Value = "Product C";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["C4"].Value = 3000;

            // Erstelle eine Pivot-Tabelle
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("=A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Zeigt den aktuellen SourceType-Wert an.
            Console.WriteLine("Current PivotTable SourceType: " + pivotTable.SourceType);

            // Berechnet Daten, um die Pivot-Tabelle anzuzeigen.
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableSourceTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotTableSourceType](../../pivottablesourcetype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


