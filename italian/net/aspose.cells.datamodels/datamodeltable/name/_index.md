---
title: "DataModelTable.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataModelTable. Ottiene il nome della tabella del modello di dati"
type: docs
url: /it/net/aspose.cells.datamodels/datamodeltable/name/
---
## DataModelTable.Name property

Ottiene il nome della tabella del modello di dati.

```csharp
public string Name { get; }
```

### Esempi

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

### Vedi anche

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


