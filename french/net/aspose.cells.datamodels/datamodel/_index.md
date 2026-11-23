---
title: "Classe DataModel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.DataModels.DataModel. Représente le modèle de données"
type: docs
url: /fr/net/aspose.cells.datamodels/datamodel/
---
## DataModel class

Représente le modèle de données.

```csharp
public class DataModel
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Relationships](../../aspose.cells.datamodels/datamodel/relationships/) { get; } | Obtient toutes les relations des tables du modèle de données. |
| [Tables](../../aspose.cells.datamodels/datamodel/tables/) { get; } | Obtient toutes les tables du modèle de données. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenez le DataModel du classeur au lieu de créer une nouvelle instance
            DataModel dataModel = workbook.DataModel;

            // Démo de l'accès aux tables et aux relations (propriétés en lecture seule)
            Console.WriteLine("Number of tables in DataModel: " + dataModel.Tables.Count);
            Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

            // Remarque : comme les Tables et les Relations sont des collections en lecture seule,
            // nous ne pouvons accéder qu'aux éléments existants mais ne pas les modifier directement

            // Enregistrer le classeur (le DataModel est généralement utilisé en interne par Aspose.Cells)
            workbook.Save("DataModelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


