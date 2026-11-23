---
title: "Classe CellsDataTableFactory"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CellsDataTableFactory. Utilitaire pour créer ICellsDataTable à partir d'objets personnalisés pour la commodité des utilisateurs"
type: docs
url: /fr/net/aspose.cells/cellsdatatablefactory/
---
## CellsDataTableFactory class

Utilitaire pour créer ICellsDataTable à partir d'objets personnalisés pour la commodité de l'utilisateur.

```csharp
public class CellsDataTableFactory
```

## Méthodes

| Nom | Description |
| --- | --- |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance)(double[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_6)(ICollection) | Crée ICellsDataTable à partir de la collection fournie. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_3)(int[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_8)(object[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_1)(double[], bool) | Crée ICellsDataTable à partir de la séquence donnée de valeurs double. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_2)(double[], string[]) | Crée ICellsDataTable à partir de la séquence donnée de valeurs double. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_7)(ICollection, bool) | Crée ICellsDataTable à partir de la collection fournie. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_4)(int[], bool) | Crée ICellsDataTable à partir de la séquence donnée de valeurs entières. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_5)(int[], string[]) | Crée ICellsDataTable à partir de la séquence donnée de valeurs entières. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_9)(object[], bool) | Crée ICellsDataTable à partir de la séquence donnée d'objets. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_10)(object[], string[]) | Crée ICellsDataTable à partir de la séquence donnée d'objets. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_11)(object[][], bool, string[]) | Crée un ICellsDataTable à partir d'une séquence donnée d'objets. |

### Exemples

```csharp
using Aspose.Cells;
using System;
using System.Collections.Generic;

namespace AsposeCellsExamples
{
    public class CellsDataTableFactoryDemo
    {
        public static void RunDemo()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Obtenir l'instance de CellsDataTableFactory à partir du classeur
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Créer une instance de ICellsDataTable à partir de la liste de données personnalisées
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Importer le tableau de données dans la feuille de calcul en commençant à la cellule A1
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Enregistrez le classeur
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
            workbook.Save("CellsDataTableFactoryDemo.pdf");
        }
    }

    // Classe de données personnalisées
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


