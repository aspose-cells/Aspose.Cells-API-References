---
title: "DataModel.Tables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataModel egenskap. Hämtar alla tabeller i datamodellen"
type: docs
url: /sv/net/aspose.cells.datamodels/datamodel/tables/
---
## DataModel.Tables property

Hämtar alla tabeller i datamodellen.

```csharp
public DataModelTableCollection Tables { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DataModels;

namespace AsposeCellsExamples
{
    public class DataModelPropertyTablesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Få åtkomst till datamodellen
            DataModel dataModel = wb.DataModel;
            
            // Hämta tabellsamlingen och visa antalet
            Console.WriteLine($"Tables count in new workbook: {dataModel.Tables.Count}");
            
            // Läs in exempelarbetsbok med datamodell
            string sourceFile = "example.xlsb";
            if (System.IO.File.Exists(sourceFile))
            {
                Workbook sampleWorkbook = new Workbook(sourceFile);
                DataModel sampleDataModel = sampleWorkbook.DataModel;
                
                // Få åtkomst till tabellsamlingen
                DataModelTableCollection tables = sampleDataModel.Tables;
                Console.WriteLine($"Tables count in sample file: {tables.Count}");
                
                // Iterera genom tabeller
                foreach (DataModelTable table in tables)
                {
                    Console.WriteLine($"Table name: {table.Name}");
                }
            }
            else
            {
                Console.WriteLine($"Sample file '{sourceFile}' not found. Create an Excel file with data model to see tables information.");
            }
        }
    }
}
```

### Se även

* class [DataModelTableCollection](../../datamodeltablecollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


