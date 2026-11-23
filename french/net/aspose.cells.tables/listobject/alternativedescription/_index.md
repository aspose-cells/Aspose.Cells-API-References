---
title: "ListObject.AlternativeDescription"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Obtient et définit la description alternative"
type: docs
url: /fr/net/aspose.cells.tables/listobject/alternativedescription/
---
## ListObject.AlternativeDescription property

Obtient et définit la description alternative.

```csharp
public string AlternativeDescription { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeDescriptionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créer un objet de liste
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Définir le texte alternatif et la description
            listObject.AlternativeText = "Test";
            listObject.AlternativeDescription = "aSXADCS";

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            // Recharger et vérifier les propriétés
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedListObject = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedListObject.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedListObject.AlternativeDescription);
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


