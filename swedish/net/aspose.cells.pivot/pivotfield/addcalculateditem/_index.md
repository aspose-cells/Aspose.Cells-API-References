---
title: "PivotField.AddCalculatedItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField metod. Lägg till ett beräknat formelobjekt till pivåfältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/addcalculateditem/
---
## PivotField.AddCalculatedItem method

Lägg till ett beräknat formelobjekt i pivotfältet.

```csharp
public void AddCalculatedItem(string name, string formula)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Elementets namn. |
| formel | String | Formeln för pivotelementet. |

### Anmärkningar

Stöder endast att lägga till beräknat element till rad-/kolumnfält.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodAddCalculatedItemWithStringStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "grape";
            sheet.Cells["A3"].Value = "kiwi";
            sheet.Cells["A4"].Value = "grape";
            sheet.Cells["A5"].Value = "kiwi";
            
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 50;
            sheet.Cells["B3"].Value = 70;
            sheet.Cells["B4"].Value = 30;
            sheet.Cells["B5"].Value = 20;

            // Skapa pivottabell med korrekta parametrar
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Hämta pivåfältet och lägg till beräknat element
            PivotField fruitField = pivotTable.RowFields[0];
            fruitField.AddCalculatedItem("grape_kiwi_total", "=grape + kiwi");
            
            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotFieldAddCalculatedItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


