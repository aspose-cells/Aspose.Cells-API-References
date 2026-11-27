---
title: "PivotTable.MoveTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Flyttar PivotTable till en annan plats i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/moveto/
---
## MoveTo(int, int) {#moveto}

Flyttar pivottabellen till en annan plats i kalkylbladet.

```csharp
public void MoveTo(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | radindex. |
| column | Int32 | kolumnindex. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["B3"].PutValue(2500);

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // Beräkna data för att fylla pivottabellen
            pivotTable.CalculateData();

            try
            {
                // Anropa MoveTo-metoden med (Int32, Int32)-parametrar för att flytta pivottabellen
                pivotTable.MoveTo(5, 2); // Move to row 5, column 2
                
                Console.WriteLine("Pivot table moved successfully to new location (5,2)");
                
                // Beräkna data igen för att uppdatera den flyttade pivottabellen
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MoveTo method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("PivotTableMethodMoveToWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## MoveTo(int, int, int) {#moveto_1}

Flyttar pivottabellen till en annan plats i kalkylbladet.

```csharp
public void MoveTo(int sheetIndex, int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | Int32 | index för målarket |
| row | Int32 | radindex. |
| column | Int32 | kolumnindex. |

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## MoveTo(string) {#moveto_2}

Flyttar pivottabellen till en annan plats i kalkylbladet.

```csharp
public void MoveTo(string destCellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destCellName | String | destinationscellens namn. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodMoveToWithStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Ange exempeldata
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // Skapa pivottabell
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            
            // Lägg till fält i pivottabell
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Ställ in stil och uppdatera
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            sheet.RefreshPivotTables();

            // Flytta pivottabellen till ny plats
            pivot.MoveTo("H16");
            sheet.RefreshPivotTables();

            // Spara arbetsboken
            book.Save("PivotTableMoveToExample.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


