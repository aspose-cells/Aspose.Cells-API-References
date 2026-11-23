---
title: "PaginatedSaveOptions.OnePagePerSheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Si OnePagePerSheet est vrai, tout le contenu d'une feuille sera exporté sur une seule page dans le résultat. La taille du papier du pagesetup sera invalide et les autres paramètres du pagesetup resteront effectifs"
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/onepagepersheet/
---
## PaginatedSaveOptions.OnePagePerSheet property

Si OnePagePerSheet est vrai, tout le contenu d'une feuille sera exporté sur une seule page dans le résultat. Le format de papier du pagesetup sera invalide, et les autres paramètres du pagesetup resteront effectifs.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des données de test
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            
            // Ajoutez des données d'exemple aux deux feuilles
            for (int i = 0; i < 10; i++)
            {
                sheet1.Cells[i, 0].Value = $"Sheet1 Data {i + 1}";
                sheet2.Cells[i, 0].Value = $"Sheet2 Data {i + 1}";
            }

            // Définissez les options d'enregistrement PDF avec OnePagePerSheet
            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;

            // Enregistrez le classeur au format PDF
            workbook.Save("output.pdf", options);
        }
    }
}
```

### Voir aussi

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


