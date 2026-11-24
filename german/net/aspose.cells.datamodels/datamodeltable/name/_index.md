---
title: "DataModelTable.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModelTable-Eigenschaft. Gibt den Namen der Datenmodell-Tabelle zurück"
type: docs
url: /de/net/aspose.cells.datamodels/datamodeltable/name/
---
## DataModelTable.Name property

Ermittelt den Namen der Datenmodell-Tabelle.

```csharp
public string Name { get; }
```

### Beispiele

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

### Siehe auch

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


