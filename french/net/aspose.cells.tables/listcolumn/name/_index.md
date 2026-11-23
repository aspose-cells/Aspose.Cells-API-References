---
title: "ListColumn.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListColumn. Obtient et définit le nom de la colonne"
type: docs
url: /fr/net/aspose.cells.tables/listcolumn/name/
---
## ListColumn.Name property

Obtient et définit le nom de la colonne.

```csharp
public string Name { get; set; }
```

### Remarques

Si le nom de la colonne est défini, la valeur de la cellule correspondante sera également modifiée.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Value");
            
            // Créer un objet tableau/liste
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            Aspose.Cells.Tables.ListObject listObject = worksheet.ListObjects[index];

            // Accédez et modifiez la propriété Name du premier ListColumn
            listObject.ListColumns[0].Name = "NewID";
            
            // Vérifiez que le nom a été défini
            Console.WriteLine("First column name: " + listObject.ListColumns[0].Name);
            
            // Enregistrez le classeur
            workbook.Save("ListColumnPropertyNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


