---
title: "PaginatedSaveOptions.DefaultFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans pdfimage. Définissez le DefaultFont tel que MingLiu ou MS Gothic pour afficher ces caractères. Si cette propriété n'est pas définie, Aspose.Cells utilisera la police système par défaut pour afficher ces caractères Unicode."
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/defaultfont/
---
## PaginatedSaveOptions.DefaultFont property

Lorsque les caractères dans le fichier Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF, l'image. Définissez la propriété DefaultFont, par exemple MingLiu ou MS Gothic, pour afficher ces caractères. Si cette propriété n'est pas définie, Aspose.Cells utilisera la police par défaut du système pour afficher ces caractères Unicode.

```csharp
public string DefaultFont { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyDefaultFontDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("This text will use the default font");
            worksheet.Cells["A2"].PutValue("如果默认字体支持中文，这将显示正确");

            // Configurez les options d'enregistrement PDF avec la police par défaut
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultFont = "宋体";
            pdfSaveOptions.CheckWorkbookDefaultFont = true;

            // Enregistrer en PDF
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Voir aussi

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


