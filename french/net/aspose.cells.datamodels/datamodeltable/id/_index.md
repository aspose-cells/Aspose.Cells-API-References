---
title: "DataModelTable.Id"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataModelTable. Obtient l'identifiant de la table du modèle de données"
type: docs
url: /fr/net/aspose.cells.datamodels/datamodeltable/id/
---
## DataModelTable.Id property

Obtient l'ID de la table du modèle de données.

```csharp
public string Id { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using Aspose.Cells.Tables;
    using System;

    public class DataModelTablePropertyIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour créer une table
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Item 2");

            // Créez un ListObject (table)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Obtenir le DataModelTable (c'est en lecture seule dans le classeur)
            DataModelTable dataModelTable = workbook.DataModel.Tables[0];

            // Afficher la valeur actuelle de l'Id
            Console.WriteLine("Current DataModelTable Id: " + dataModelTable.Id);

            // Remarque : la propriété Id est en lecture seule, nous ne pouvons donc pas la définir.
            // Cela montre comment accéder à et utiliser l'Id existant.

            // Exemple d'utilisation : comparer les ID de tables lors du travail avec plusieurs tables.
            DataModelTable secondTable = null;
            if (workbook.DataModel.Tables.Count > 1)
            {
                secondTable = workbook.DataModel.Tables[1];
                if (dataModelTable.Id != secondTable.Id)
                {
                    Console.WriteLine("Different table IDs detected");
                }
            }

            // Enregistrez le classeur
            workbook.Save("DataModelTableIdDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataModelTable](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


