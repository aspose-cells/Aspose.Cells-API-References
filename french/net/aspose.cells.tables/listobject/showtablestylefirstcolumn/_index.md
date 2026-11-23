---
title: "ListObject.ShowTableStyleFirstColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Indique si la première colonne du tableau est le style appliqué"
type: docs
url: /fr/net/aspose.cells.tables/listobject/showtablestylefirstcolumn/
---
## ListObject.ShowTableStyleFirstColumn property

Indique si la première colonne du tableau a le style appliqué.

```csharp
public bool ShowTableStyleFirstColumn { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleFirstColumnDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["B4"].PutValue(3.2);

            // Créer un objet de liste
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];
            
            // Appliquer le style de la première colonne
            listObject.ShowTableStyleFirstColumn = true;
            
            // Enregistrez le classeur
            workbook.Save("ListObjectShowFirstColumnStyle.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("File saved with first column style applied to the table.");
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


