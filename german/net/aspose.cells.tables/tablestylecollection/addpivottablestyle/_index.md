---
title: "TableStyleCollection.AddPivotTableStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TableStyleCollection-Methode. Fügt einen benutzerdefinierten Pivot-Tabellenstil hinzu"
type: docs
url: /de/net/aspose.cells.tables/tablestylecollection/addpivottablestyle/
---
## TableStyleCollection.AddPivotTableStyle method

Fügt einen benutzerdefinierten Pivot-Tabellenstil hinzu.

```csharp
public int AddPivotTableStyle(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Pivot-Tabellenstilname. |

### Rückgabewert

Der Index des Pivot-Tabellenstils.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleCollectionMethodAddPivotTableStyleWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Desktop");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(500);

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 1);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2);

            try
            {
                // Die Tabellenstil-Sammlung abrufen
                TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

                // Rufe AddPivotTableStyle mit String-Parameter auf
                int styleIndex = tableStyles.AddPivotTableStyle("CustomPivotStyle1");
                Console.WriteLine($"Added pivot table style at index: {styleIndex}");

                // Setze den neuen Stil als Standard-Pivot-Stil
                tableStyles.DefaultPivotStyleName = "CustomPivotStyle1";

                // Wende den Stil auf unsere Pivot-Tabelle an
                pivotTable.PivotTableStyleName = "CustomPivotStyle1";
                Console.WriteLine("Applied custom pivot table style successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPivotTableStyle method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TableStyleCollectionMethodAddPivotTableStyleWithStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


