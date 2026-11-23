---
title: "Workbook.Worksheets"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient la collection WorksheetCollection dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/workbook/worksheets/
---
## Workbook.Worksheets property

Obtient la collection [`WorksheetCollection`](../../worksheetcollection/) dans la feuille de calcul.

```csharp
public WorksheetCollection Worksheets { get; }
```

### Valeur de retour

[`WorksheetCollection`](../../worksheetcollection/) collection

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyWorksheetsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Ajouter une nouvelle feuille de calcul
            workbook.Worksheets.Add("SecondSheet");
            
            // Accédez à la deuxième feuille de calcul et ajoutez des données
            Worksheet secondSheet = workbook.Worksheets[1];
            secondSheet.Cells["A1"].PutValue("Product");
            secondSheet.Cells["B1"].PutValue("Price");
            secondSheet.Cells["A2"].PutValue("Laptop");
            secondSheet.Cells["B2"].PutValue(999.99);
            
            // Enregistrez le classeur
            workbook.Save("WorkbookWorksheetsDemo.xlsx");
            
            // Afficher le nombre de feuilles de calcul
            Console.WriteLine($"Number of worksheets: {workbook.Worksheets.Count}");
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../../worksheetcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


