---
title: "Enum TableDataSourceType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Tables.TableDataSourceType enum. Représente le type de source de données des tableaux"
type: docs
url: /fr/net/aspose.cells.tables/tabledatasourcetype/
---
## TableDataSourceType enumeration

Représente le type de source de données de la table.

```csharp
public enum TableDataSourceType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Worksheet | `0` | Tableau de feuille de calcul Excel |
| SharePoint | `1` | Liste liée SharePoint en lecture-écriture |
| XML | `2` | Table du mapper XML |
| QueryTable | `3` | Table de requête |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableDataSourceTypeDemo
    {
        public static void TableDataSourceTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Ajoutez un ListObject (table) à la feuille de calcul
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Définir le nom d'affichage du tableau
            listObject.DisplayName = "SampleTable";

            // Définir le type de source de données du tableau
            TableDataSourceType dataSourceType = listObject.DataSourceType;

            // Afficher le type de source de données
            Console.WriteLine("Data Source Type: " + dataSourceType);

            // Enregistrez le classeur
            workbook.Save("TableDataSourceTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


