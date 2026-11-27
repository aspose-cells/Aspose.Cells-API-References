---
title: "PivotTableCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTableCollection-metod. Tar bort pivottabellen på det angivna indexet och raderar pivottabellens data."
type: docs
url: /sv/net/aspose.cells.pivot/pivottablecollection/removeat/
---
## RemoveAt(int) {#removeat}

Tar bort PivotTable på det angivna indexet och raderar PivotTable-data

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | positionsindexet i PivotTable‑samlingen |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Lägg till flera pivottabeller
            sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            sheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
            sheet.PivotTables.Add("A1:B4", "D20", "PivotTable3");

            // Ta bort pivottabell på index 1 (andra pivottabellen)
            sheet.PivotTables.RemoveAt(1);

            // Verifiera antalet efter borttagning
            Console.WriteLine("Pivot Tables Count: " + sheet.PivotTables.Count);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_2}

Raderar PivotTable på det angivna indexet

```csharp
public void RemoveAt(int index, bool keepData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | positionsindexet i PivotTable‑samlingen |
| keepData | Boolean | Om PivotTable‑data ska behållas |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveAtWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Lägg till en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "D9", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demonstrera RemoveAt med keepData=true
            worksheet.PivotTables.RemoveAt(0, true);
            Console.WriteLine("Pivot table removed with keepData=true. Cell D9 value: " + worksheet.Cells["D9"].Value);

            // Lägg till en annan pivottabell
            index = worksheet.PivotTables.Add("A1:B4", "D9", "PivotTable2");
            pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demonstrera RemoveAt med keepData=false
            worksheet.PivotTables.RemoveAt(0, false);
            Console.WriteLine("Pivot table removed with keepData=false. Cell D9 value: " + worksheet.Cells["D9"].Value);
        }
    }
}
```

### Se även

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


