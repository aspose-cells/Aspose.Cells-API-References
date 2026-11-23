---
title: "DataModel.Tables"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataModel. Obtient toutes les tables du modèle de données"
type: docs
url: /fr/net/aspose.cells.datamodels/datamodel/tables/
---
## DataModel.Tables property

Obtient toutes les tables du modèle de données.

```csharp
public DataModelTableCollection Tables { get; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Accéder au modèle de données
            DataModel dataModel = wb.DataModel;
            
            // Obtenir la collection de tables et afficher le nombre
            Console.WriteLine($"Tables count in new workbook: {dataModel.Tables.Count}");
            
            // Charger le classeur d'exemple avec le modèle de données
            string sourceFile = "example.xlsb";
            if (System.IO.File.Exists(sourceFile))
            {
                Workbook sampleWorkbook = new Workbook(sourceFile);
                DataModel sampleDataModel = sampleWorkbook.DataModel;
                
                // Accéder à la collection de tables
                DataModelTableCollection tables = sampleDataModel.Tables;
                Console.WriteLine($"Tables count in sample file: {tables.Count}");
                
                // Parcourir les tables
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

### Voir aussi

* class [DataModelTableCollection](../../datamodeltablecollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


