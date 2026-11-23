---
title: "Workbook.AcceptAllRevisions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Accepte toutes les modifications suivies dans le classeur"
type: docs
url: /fr/net/aspose.cells/workbook/acceptallrevisions/
---
## Workbook.AcceptAllRevisions method

Accepte toutes les modifications suivies dans le classeur.

```csharp
public void AcceptAllRevisions()
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAcceptAllRevisionsDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des révisions
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter quelques révisions (le suivi des modifications doit d'abord être activé dans Excel)
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Enregistrer avec les révisions
            string sourcePath = "source_with_revisions.xlsx";
            workbook.Save(sourcePath, SaveFormat.Xlsx);
            
            // Rouvrir le classeur
            workbook = new Workbook(sourcePath);
            
            // Vérifier s'il y a des révisions et les accepter
            if (workbook.HasRevisions)
            {
                Console.WriteLine("Workbook has revisions. Accepting all...");
                workbook.AcceptAllRevisions();
                
                // Enregistrer sans révisions
                string destPath = "output_no_revisions.xlsx";
                workbook.Save(destPath, SaveFormat.Xlsx);
                Console.WriteLine("Revisions accepted and saved to: " + destPath);
            }
            else
            {
                Console.WriteLine("Workbook has no revisions.");
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


