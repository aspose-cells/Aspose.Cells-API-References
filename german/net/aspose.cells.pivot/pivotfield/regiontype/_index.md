---
title: "PivotField.RegionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt die Region der Pivot-Tabelle an, in der dieses Feld angezeigt wird"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/regiontype/
---
## PivotField.RegionType property

Gibt die Region der Pivot‑Tabelle an, in der dieses Feld angezeigt wird.

```csharp
public PivotFieldType RegionType { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyRegionTypeDemo
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
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Erstelle eine Pivot-Tabelle
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Pivot-Tabellendaten aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Das erste Pivot-Feld abrufen
            PivotField pivotField = pivotTable.RowFields[0];

            // Den aktuellen RegionType-Wert anzeigen
            Console.WriteLine("Current RegionType value: " + pivotField.RegionType);

            // Demonstrieren, wie die RegionType-Eigenschaft verwendet wird
            if (pivotField.RegionType == PivotFieldType.Row)
            {
                Console.WriteLine("This pivot field is in the row area");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldRegionTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


