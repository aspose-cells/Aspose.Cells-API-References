---
title: "DataModel.Tables"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataModel-Eigenschaft. Ruft alle Tabellen im Datemodell ab"
type: docs
url: /de/net/aspose.cells.datamodels/datamodel/tables/
---
## DataModel.Tables property

Ermittelt alle Tabellen im Datenmodell.

```csharp
public DataModelTableCollection Tables { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Greifen Sie auf das Datemodell zu
            DataModel dataModel = wb.DataModel;
            
            // Holen Sie die Tabellensammlung und zeigen Sie die Anzahl an
            Console.WriteLine($"Tables count in new workbook: {dataModel.Tables.Count}");
            
            // Laden Sie eine Beispielarbeitsmappe mit Datemodell
            string sourceFile = "example.xlsb";
            if (System.IO.File.Exists(sourceFile))
            {
                Workbook sampleWorkbook = new Workbook(sourceFile);
                DataModel sampleDataModel = sampleWorkbook.DataModel;
                
                // Greifen Sie auf die Tabellensammlung zu
                DataModelTableCollection tables = sampleDataModel.Tables;
                Console.WriteLine($"Tables count in sample file: {tables.Count}");
                
                // Durchlaufen Sie die Tabellen
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

### Siehe auch

* class [DataModelTableCollection](../../datamodeltablecollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


