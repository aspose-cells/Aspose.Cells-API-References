---
title: "PivotTableCollection.Remove"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTableCollection-metod. Raderar den angivna PivotTable och tar bort PivotTable-data"
type: docs
url: /sv/net/aspose.cells.pivot/pivottablecollection/remove/
---
## Remove(PivotTable) {#remove}

Tar bort den angivna PivotTable och tar bort PivotTable-data

```csharp
public void Remove(PivotTable pivotTable)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable-objekt |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Hämta pivottabellsamling
            PivotTableCollection pivotTables = sheet.PivotTables;
            
            // Kontrollera om det finns några pivot‑tabeller
            if (pivotTables.Count > 0)
            {
                // Hämta den första pivot‑tabellen
                PivotTable pivotTable = pivotTables[0];
                
                // Ta bort pivottabellen
                pivotTables.Remove(pivotTable);
                
                Console.WriteLine("Pivot table removed successfully. Count: " + pivotTables.Count);
            }
            
            // Spara arbetsboken
            workbook.Save("PivotTableRemoved.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Remove(PivotTable, bool) {#remove_1}

Tar bort den angivna PivotTable

```csharp
public void Remove(PivotTable pivotTable, bool keepData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable-objekt |
| keepData | Boolean | Om PivotTable‑data ska behållas |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableBooleanDemo
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
            int index = worksheet.PivotTables.Add("A1:B4", "D5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demonstrera Remove-metoden med PivotTable och booleska parametrar
            Console.WriteLine("Before removal - Cell D5 value: " + worksheet.Cells["D5"].StringValue);
            
            // Ta bort pivottabellen men behåll data (true)
            worksheet.PivotTables.Remove(pivotTable, true);
            Console.WriteLine("After removal (keep data) - Cell D5 value: " + worksheet.Cells["D5"].StringValue);

            // Lägg till en annan pivottabell
            index = worksheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
            pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("\nBefore removal - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
            
            // Ta bort pivottabellen och rensa data (false)
            worksheet.PivotTables.Remove(pivotTable, false);
            Console.WriteLine("After removal (clear data) - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
        }
    }
}
```

### Se även

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


