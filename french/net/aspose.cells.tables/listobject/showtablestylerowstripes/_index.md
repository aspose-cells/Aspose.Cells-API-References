---
title: "ListObject.ShowTableStyleRowStripes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Indique si le format de bandes de lignes est appliqué à"
type: docs
url: /fr/net/aspose.cells.tables/listobject/showtablestylerowstripes/
---
## ListObject.ShowTableStyleRowStripes property

Indique si le formatage à bandes de lignes est appliqué.

```csharp
public bool ShowTableStyleRowStripes { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleRowStripesDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(300);

            // Créer un objet de liste
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];

            // Démontrer la propriété ShowTableStyleRowStripes
            Console.WriteLine("Before: ShowTableStyleRowStripes = " + listObject.ShowTableStyleRowStripes);
            listObject.ShowTableStyleRowStripes = false;
            Console.WriteLine("After: ShowTableStyleRowStripes = " + listObject.ShowTableStyleRowStripes);

            // Enregistrez le classeur
            workbook.Save("ListObjectShowTableStyleRowStripesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


