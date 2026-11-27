---
title: "PivotItemCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItemCollection‑egenskap. Hämtar PivotItem‑objektet på det specifika indexet."
type: docs
url: /sv/net/aspose.cells.pivot/pivotitemcollection/item/
---
## PivotItemCollection indexer (1 of 2)

Hämtar PivotItem‑objektet på det specifika indexet.

```csharp
public PivotItem this[int index] { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 150;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 200;
            
            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Kom åt pivotelement med Item‑egenskapen
            PivotItemCollection pivotItems = pivotTable.RowFields[0].PivotItems;
            
            // Demonstrera användning av Item-egenskapen
            Console.WriteLine("First pivot item: " + pivotItems[0].Name);
            Console.WriteLine("Second pivot item: " + pivotItems[1].Name);
            Console.WriteLine("Third pivot item: " + pivotItems[2].Name);
        }
    }
}
```

### Se även

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotItemCollection indexer (2 of 2)

Hämtar [`PivotItem`](../../pivotitem/) med det specifika namnet.

```csharp
public PivotItem this[string itemValue] { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("PivotTest3.xlsx");
            
            // Lägg till ett nytt kalkylblad för pivottabell
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            Worksheet dataSheet = workbook.Worksheets["New Hardware - Yearly"];

            // Lägg till pivottabell
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "PivotTable");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "2014");

            // Konfigurera pivottabell
            pivotTable.RowFields["Vendor"].SetSubtotals(PivotFieldSubtotalType.None, true);
            pivotTable.ShowColumnGrandTotals = false;

            // Uppdatera och beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demonstrera användning av Item‑egenskapen och flyttoperationer
            PivotItemCollection items = pivotTable.RowFields["Item"].PivotItems;
            
            // Kom åt element med Item‑egenskapen
            items["4H12"].Move(0, true);
            items["DIF400"].Move(-1, true);
            
            pivotTable.CalculateData();
            
            items["CA32"].Move(0, true);
            items["AAA3"].Move(-1, true);

            // Spara arbetsboken
            workbook.Save("PivotItemCollectionDemo_Output.xlsx");
        }
    }
}
```

### Se även

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


