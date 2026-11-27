---
title: "PivotFieldCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFieldCollection-egenskap. Hämtar PivotField-objektet på det specifika indexet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldcollection/item/
---
## PivotFieldCollection indexer (1 of 2)

Hämtar PivotField-objektet på det specifika indexet.

```csharp
public PivotField this[int index] { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett arbetsblad och hämta det första bladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Lägg till en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till fält i områden
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Åtkomst till det första radfältet med Item-egenskapen och sätt IsAutoSort
            pivotTable.RowFields[0].IsAutoSort = true;
            
            // Spara arbetsboken
            workbook.Save("PivotFieldCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotFieldCollection indexer (2 of 2)

Hämtar PivotField-objektet med det specifika namnet.

```csharp
public PivotField this[string name] { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            ws.Cells["A1"].Value = "Category";
            ws.Cells["B1"].Value = "Value";
            ws.Cells["A2"].Value = "A";
            ws.Cells["B2"].Value = 10;
            ws.Cells["A3"].Value = "B";
            ws.Cells["B3"].Value = 20;
            ws.Cells["A4"].Value = "A";
            ws.Cells["B4"].Value = 30;
            ws.Cells["A5"].Value = "B";
            ws.Cells["B5"].Value = 40;

            // Skapa pivottabell
            int index = ws.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pTable = ws.PivotTables[index];
            
            // Lägg till fält i pivottabell
            pTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Demonstrera användning av Item-egenskapen
            pTable.DataFields["Sum of Value"].IsAutoSort = true;
            pTable.DataFields["Sum of Value"].IsAscendSort = false;
            
            // Uppdatera och beräkna pivottabell
            pTable.RefreshData();
            pTable.CalculateData();
            
            // Spara arbetsboken
            wb.Save("PivotFieldCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


