---
title: "Workbook.CellsDataTableFactory"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient la fabrique permettant de créer ICellsDataTable à partir d'objets personnalisés"
type: docs
url: /fr/net/aspose.cells/workbook/cellsdatatablefactory/
---
## Workbook.CellsDataTableFactory property

Obtient la fabrique pour créer ICellsDataTable à partir d'objets personnalisés

```csharp
public CellsDataTableFactory CellsDataTableFactory { get; }
```

### Exemples

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }

    public class WorkbookPropertyCellsDataTableFactoryDemo
    {
        public static void Run()
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

            // Obtenir CellsDataTableFactory depuis la propriété du classeur
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Créer une table de données à partir d'une liste
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Importer des données dans la feuille de calcul
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Enregistrer les sorties
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellsDataTableFactory](../../cellsdatatablefactory/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


