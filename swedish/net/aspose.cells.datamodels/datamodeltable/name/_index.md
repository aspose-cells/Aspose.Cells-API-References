---
title: "DataModelTable‑egenskap. Hämtar anslutningsnamnet för datamodelltabellen"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Visa det aktuella ConnectionName‑värdet"
type: docs
url: /sv/net/aspose.cells.datamodels/datamodeltable/name/
---
## DataModelTable.Name property

Hämtar namnet på datamodelltabellen.

```csharp
public string Name { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Pivot;
    using System;

    public class DataModelTablePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            DataModel dataModel = workbook.DataModel;
            if (dataModel.Tables.Count == 0)
            {
                Console.WriteLine("Workbook data model contains no tables. Add tables to the data model first.");
                return;
            }

            DataModelTable table = dataModel.Tables[0];
            Console.WriteLine("Current DataModelTable Name: " + table.Name);
            
            Worksheet sheet = workbook.Worksheets.Add("Report");
            int pivotIndex = sheet.PivotTables.Add("PivotTable1", "A1", table.Name);
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            workbook.Save("DataModelTableNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


