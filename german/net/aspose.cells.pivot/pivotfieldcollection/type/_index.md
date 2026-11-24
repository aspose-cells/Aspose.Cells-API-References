---
title: "PivotFieldCollection.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFieldCollection-Eigenschaft. Gibt den Typ der PivotFields zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotfieldcollection/type/
---
## PivotFieldCollection.Type property

Liefert den Typ von PivotFields.

```csharp
public PivotFieldType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldCollectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 7;

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotFieldCollection rowFields = pivotTable.RowFields;

            // Typ der PivotField-Collection anzeigen
            Console.WriteLine("PivotFieldCollection Type: " + rowFields.Type);

            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            PivotFieldCollection dataFields = pivotTable.DataFields;

            // Typ der Datenfeld-Collection anzeigen
            Console.WriteLine("DataFields Type: " + dataFields.Type);

            // Daten berechnen und die Pivot-Tabelle aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Ergebnis speichern
            workbook.Save("PivotFieldCollectionTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


