---
title: "WorksheetCollection.ActiveSheetIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorksheetCollection. Représente l'index de la feuille active lorsque le classeur est ouvert"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/activesheetindex/
---
## WorksheetCollection.ActiveSheetIndex property

Représente l'index de la feuille de calcul active lorsque le classeur est ouvert.

```csharp
public int ActiveSheetIndex { get; set; }
```

### Remarques

L'index de la feuille commence à zéro.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetIndexDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec 3 feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Définir l'index de la feuille active à 1 (deuxième feuille)
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Vérifier la feuille active
            Console.WriteLine("Active Sheet: " + workbook.Worksheets[workbook.Worksheets.ActiveSheetIndex].Name);

            // Enregistrez le classeur
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ActiveSheetDemo.xlsx");
            workbook.Save(outputPath);

            Console.WriteLine("File saved to: " + outputPath);
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


