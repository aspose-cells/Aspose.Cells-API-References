---
title: "PivotPageFields.PivotPageFields"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotPageFields‑konstruktor. Representerar pivot‑sidfältselementen"
type: docs
url: /sv/net/aspose.cells.pivot/pivotpagefields/pivotpagefields/
---
## PivotPageFields constructor

Representerar pivot-sidfältsobjekten.

```csharp
public PivotPageFields()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotPageFieldsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["C3"].PutValue(2000);

            // Skapa pivotsidfält med hjälp av konstruktorn
            PivotPageFields pageFields = new PivotPageFields();
            
            // Lägg till sidfält
            string[] items = { "Item1", "Item2" };
            pageFields.AddPageField(items);
            
            // Lägg till identifiering
            int[] itemIndexes = { 0, 1 };
            pageFields.AddIdentify(0, itemIndexes);

            // Lägg till pivottabell med korrekta parametrar
            PivotTableCollection pivotTables = worksheet.PivotTables;
            string sourceData = "A1:C3";
            int index = pivotTables.Add(sourceData, "E5", "PivotTable1");

            // Spara arbetsboken
            workbook.Save("PivotPageFieldsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


