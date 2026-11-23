---
title: "ListObject.ShowTableStyleColumnStripes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Indique si le formatage en bandes de colonnes est appliqué"
type: docs
url: /fr/net/aspose.cells.tables/listobject/showtablestylecolumnstripes/
---
## ListObject.ShowTableStyleColumnStripes property

Indique si le formatage à bandes de colonnes est appliqué.

```csharp
public bool ShowTableStyleColumnStripes { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleColumnStripesDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // Créer un objet de liste et obtenir la référence
            int listObjectIndex = worksheet.ListObjects.Add("A1", "B4", true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // Définir la propriété des bandes de colonnes
            listObject.ShowTableStyleColumnStripes = true;
            
            // Enregistrez le classeur
            workbook.Save("ListObjectWithColumnStripes.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with column stripes enabled.");
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


