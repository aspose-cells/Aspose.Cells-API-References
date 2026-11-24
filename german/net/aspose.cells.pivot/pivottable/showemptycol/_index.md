---
title: "PivotTable.ShowEmptyCol"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob leere Spalten in die Tabelle aufgenommen werden"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showemptycol/
---
## PivotTable.ShowEmptyCol property

Gibt an, ob leere Spalten in die Tabelle aufgenommen werden sollen

```csharp
public bool ShowEmptyCol { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowEmptyColDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Erstelle eine Pivot-Tabelle
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aktuellen Wert von ShowEmptyCol anzeigen
            Console.WriteLine("Current ShowEmptyCol value: " + pivotTable.ShowEmptyCol);

            // Setze ShowEmptyCol auf false (leere Spalten ausblenden)
            pivotTable.ShowEmptyCol = false;
            Console.WriteLine("ShowEmptyCol set to false - empty columns will be hidden");

            // PivotTable-Daten berechnen
            pivotTable.CalculateData();

            // Arbeitsmappe mit ausgeblendeten leeren Spalten speichern
            workbook.Save("PivotTableHideEmptyCols.xlsx");

            // Setze ShowEmptyCol zurück auf true (leere Spalten anzeigen)
            pivotTable.ShowEmptyCol = true;
            Console.WriteLine("ShowEmptyCol set to true - empty columns will be shown");

            // PivotTable-Daten erneut berechnen
            pivotTable.CalculateData();

            // Arbeitsmappe mit sichtbaren leeren Spalten speichern
            workbook.Save("PivotTableShowEmptyCols.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


