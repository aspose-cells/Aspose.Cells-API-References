---
title: "PivotTable.GetCellByDisplayName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable metod. Hämtar Cell‑objektet med displaynamnet för PivotField"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/getcellbydisplayname/
---
## PivotTable.GetCellByDisplayName method

Hämtar [`Cell`](../../../aspose.cells/cell/)‑objektet med displaynamnet för PivotField.

```csharp
public Cell GetCellByDisplayName(string displayName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| displayName | String | DisplayName för PivotField |

### Returvärde

Cell‑objektet

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetCellByDisplayNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Hämta displaynamn för datafält
            string displayName = pivotTable.DataFields[0].DisplayName;

            // Använd metoden GetCellByDisplayName
            Cell cell = pivotTable.GetCellByDisplayName(displayName);

            // Skriv ut resultat
            Console.WriteLine("Display Name: " + displayName);
            Console.WriteLine("Cell Name: " + (cell != null ? cell.Name : "null"));
            Console.WriteLine("Cell Value: " + (cell != null ? cell.Value.ToString() : "null"));

            // Spara arbetsboken
            workbook.Save("PivotTable_GetCellByDisplayName_Output.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../../aspose.cells/cell/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


