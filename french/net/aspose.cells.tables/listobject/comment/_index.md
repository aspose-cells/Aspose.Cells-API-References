---
title: "ListObject.Comment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Obtient et définit le commentaire du tableau"
type: docs
url: /fr/net/aspose.cells.tables/listobject/comment/
---
## ListObject.Comment property

Obtient et définit le commentaire du tableau.

```csharp
public string Comment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyCommentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple pour l'objet de liste
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(100);

            // Créer un objet de liste
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObj = worksheet.ListObjects[index];

            // Définir et démontrer la propriété Comment
            listObj.Comment = "This is a sample comment for the list object";
            Console.WriteLine("List Object Comment: " + listObj.Comment);

            // Redimensionner l'objet de liste pour inclure plus de données
            listObj.Resize(0, 0, 2, 1, true);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(200);

            // Enregistrez le classeur
            workbook.Save("ListObjectCommentDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


