---
title: "WorksheetCollection.ActiveSheetName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorksheetCollection. Représente le nom de la feuille de calcul active lorsque le classeur est ouvert"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/activesheetname/
---
## WorksheetCollection.ActiveSheetName property

Représente le nom de la feuille de calcul active lorsque le classeur est ouvert.

```csharp
public string ActiveSheetName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter plusieurs feuilles de calcul
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Définir la feuille active par son nom
            workbook.Worksheets.ActiveSheetName = "Sheet2";

            // Vérifier la feuille active
            Console.WriteLine("Active Sheet: " + workbook.Worksheets.ActiveSheetName);

            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


