---
title: "PaginatedSaveOptions.IsFontSubstitutionCharGranularity"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible"
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/
---
## PaginatedSaveOptions.IsFontSubstitutionCharGranularity property

Indique s'il faut uniquement substituer la police du caractère lorsque la police de la cellule n'est pas compatible.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Remarques

La valeur par défaut est false. Nous essaierons d'abord la police par défaut du classeur et de PdfSaveOption/système pour la police de la cellule.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIsFontSubstitutionCharGranularityDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Sample Text with Font Substitution");

            XpsSaveOptions saveOptions = new XpsSaveOptions
            {
                IsFontSubstitutionCharGranularity = true,
                DefaultFont = "Arial"
            };

            workbook.Save("FontSubstitutionDemo.xps", saveOptions);
        }
    }
}
```

### Voir aussi

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


