---
title: "Workbook.FileName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient et définit le nom de fichier actuel"
type: docs
url: /fr/net/aspose.cells/workbook/filename/
---
## Workbook.FileName property

Obtient et définit le nom de fichier actuel.

```csharp
public string FileName { get; set; }
```

### Remarques

Si le fichier est ouvert par flux et qu'il existe des références de formules externes, veuillez définir le nom du fichier.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyFileNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Définir la propriété du nom de fichier
            wb.FileName = "SampleWorkbook.xlsx";
            
            // Ajouter des données pour démontrer la fonctionnalité
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Workbook FileName Demo");
            sheet.Cells["A2"].PutValue("Current FileName:");
            sheet.Cells["B2"].PutValue(wb.FileName);
            
            // Enregistrez le classeur
            wb.Save(wb.FileName);
            
            Console.WriteLine($"Workbook created with filename: {wb.FileName}");
            
            // Démontrer le changement du nom de fichier
            Workbook wb2 = new Workbook();
            wb2.FileName = "ChangedName.xlsx";
            Console.WriteLine($"New workbook filename set to: {wb2.FileName}");
            
            // Démontrer l'utilisation de liens externes
            if (wb.Worksheets.ExternalLinks.Count > 0)
            {
                string externalSource = wb.Worksheets.ExternalLinks[0].DataSource;
                wb2.FileName = externalSource;
                Console.WriteLine($"Updated filename to external source: {wb2.FileName}");
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


