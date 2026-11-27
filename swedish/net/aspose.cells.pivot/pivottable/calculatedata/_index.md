---
title: "PivotTable.CalculateData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable metod. Beräknar pivottabellens data till celler"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata_1}

Beräknar pivottabellens data till celler.

```csharp
public void CalculateData()
```

### Anmärkningar

Denna metod beräknar endast data med den cachade datan i [`PivotCache`](../pivotcache/). Så om du vill beräkna med den senaste datakällan, vänligen använd [`Refresh`](../../pivotcache/refresh/) metoden för att beräkna. Om endast inställningarna för pivottabellen har ändrats, räcker `CalculateData`.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            
            DateTime baseDate = new DateTime(2021, 11, 1);
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+2}"].PutValue(baseDate.AddDays(i));
                worksheet.Cells[$"B{i+2}"].PutValue(100 + i * 10);
            }

            // Skapa pivottabell - åtgärdad genom att säkerställa korrekta parametrar
            int pivotIndex = worksheet.PivotTables.Add("A1:B16", "D3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till fält till pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Använd datumfilter
            PivotField dateField = pivotTable.RowFields[0];
            dateField.FilterByDate(PivotFilterType.November, new DateTime(2021, 1, 1), new DateTime(2021, 12, 31));
            
            // Beräkna pivottabellens data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata}

Beräknar pivottabell med alternativ.

```csharp
public PivotTable[] CalculateData(PivotTableCalculateOption option)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | PivotTableCalculateOption | Alternativen för att beräkna pivottabellen |

### Returvärde

Returnerar alla pivottabeller som har beräknats. Om [`RefreshData`](../../pivottablecalculateoption/refreshdata/) är sann, kommer alla pivottabeller baserade på samma pivotcache att beräknas tillsammans.

### Anmärkningar

Om [`RefreshData`](../../pivottablecalculateoption/refreshdata/) är sann, kommer denna metod att uppdatera pivotcachen från datakällan och sedan beräkna alla pivottabeller baserade på samma pivotcache. Annars beräknas endast med den cachade datan i pivotcachen.

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataWithPivotTableCalculateOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Ställ in beräkningsalternativ
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                RefreshData = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Beräkna med alternativ
            pivotTable.CalculateData(options);

            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


