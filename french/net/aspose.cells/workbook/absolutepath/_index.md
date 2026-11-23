---
title: "Workbook.AbsolutePath"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient et définit le chemin absolu du fichier"
type: docs
url: /fr/net/aspose.cells/workbook/absolutepath/
---
## Workbook.AbsolutePath property

Obtient et définit le chemin absolu du fichier.

```csharp
public string AbsolutePath { get; set; }
```

### Remarques

Utilisé uniquement pour les liens externes.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyAbsolutePathDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook sourceBook = new Workbook();
            
            // Ajouter plusieurs feuilles de calcul
            sourceBook.Worksheets.Add("Sheet1");
            sourceBook.Worksheets.Add("Sheet2");

            // Enregistrez le classeur pour obtenir un chemin physique
            string sourcePath = Path.GetFullPath("output");
            if (!Directory.Exists(sourcePath))
            {
                Directory.CreateDirectory(sourcePath);
            }
            string sourceFilePath = Path.Combine(sourcePath, "example.xlsx");
            sourceBook.Save(sourceFilePath);

            // Rouvrez le classeur pour démontrer AbsolutePath
            Workbook reopenedBook = new Workbook(sourceFilePath);
            
            // Utilisez la propriété AbsolutePath pour construire le chemin complet
            string pathToBook = Path.Combine(reopenedBook.AbsolutePath, reopenedBook.FileName);
            Console.WriteLine("Full path to workbook: " + pathToBook);

            // Ajoutez des hyperliens en utilisant le chemin
            SetHyperlink(reopenedBook.Worksheets[0], 0, pathToBook, reopenedBook.Worksheets[0].Name, "A1");
            SetHyperlink(reopenedBook.Worksheets[0], 1, pathToBook, reopenedBook.Worksheets[1].Name, "B1");

            // Enregistrer le classeur modifié
            string destPath = Path.Combine(sourcePath, "modified_example.xlsx");
            reopenedBook.Save(destPath);
        }

        private static void SetHyperlink(Worksheet sheet, int linkIndex, string path, string sheetName, string cellRef)
        {
            HyperlinkCollection hyperlinks = sheet.Hyperlinks;
            hyperlinks.Add(cellRef, 1, 1, path + "#" + sheetName + "!A1");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


