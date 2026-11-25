---
title: "DataModel.Tables"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataModel. Ottiene tutte le tabelle nel modello di dati"
type: docs
url: /it/net/aspose.cells.datamodels/datamodel/tables/
---
## DataModel.Tables property

Ottiene tutte le tabelle nel modello dati.

```csharp
public DataModelTableCollection Tables { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Accedi al modello di dati
            DataModel dataModel = wb.DataModel;
            
            // Ottieni la raccolta di tabelle e mostra il conteggio
            Console.WriteLine($"Tables count in new workbook: {dataModel.Tables.Count}");
            
            // Carica una cartella di lavoro di esempio con modello di dati
            string sourceFile = "example.xlsb";
            if (System.IO.File.Exists(sourceFile))
            {
                Workbook sampleWorkbook = new Workbook(sourceFile);
                DataModel sampleDataModel = sampleWorkbook.DataModel;
                
                // Accedi alla raccolta di tabelle
                DataModelTableCollection tables = sampleDataModel.Tables;
                Console.WriteLine($"Tables count in sample file: {tables.Count}");
                
                // Itera attraverso le tabelle
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

### Vedi anche

* class [DataModelTableCollection](../../datamodeltablecollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


