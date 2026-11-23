---
title: "ListObject.AlternativeText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Obtient et définit le texte alternatif"
type: docs
url: /fr/net/aspose.cells.tables/listobject/alternativetext/
---
## ListObject.AlternativeText property

Obtient et définit le texte alternatif.

```csharp
public string AlternativeText { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAlternativeTextDemo
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

            // Créer un objet liste/tableau
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Définir le texte alternatif et la description
            table.AlternativeText = "Test";
            table.AlternativeDescription = "aSXADCS";
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Recharger et vérifier
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            ListObject loadedTable = loadedWorkbook.Worksheets[0].ListObjects[0];
            
            Console.WriteLine("AlternativeText: " + loadedTable.AlternativeText);
            Console.WriteLine("AlternativeDescription: " + loadedTable.AlternativeDescription);
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


