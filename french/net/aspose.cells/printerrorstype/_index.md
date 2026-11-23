---
title: "Enum PrintErrorsType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.PrintErrorsType enum. Représente les constantes d'erreurs d'impression"
type: docs
url: /fr/net/aspose.cells/printerrorstype/
---
## PrintErrorsType enumeration

Représente les constantes d'erreurs d'impression.

```csharp
public enum PrintErrorsType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| PrintErrorsBlank | `0` | Représente le fait de ne pas imprimer les erreurs. |
| PrintErrorsDash | `1` | Représente l'impression des erreurs sous la forme "--". |
| PrintErrorsDisplayed | `2` | Représente l'impression des erreurs telle qu'affichée. |
| PrintErrorsNA | `3` | Représente l'impression des erreurs sous la forme "#N/A". |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintErrorsTypeDemo
    {
        public static void PrintErrorsTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la PageSetup de la feuille de calcul
            PageSetup pageSetup = worksheet.PageSetup;

            // Définir différents types d'erreur d'impression
            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            workbook.Save("PrintErrorsBlank.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            workbook.Save("PrintErrorsDash.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDisplayed;
            workbook.Save("PrintErrorsDisplayed.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsNA;
            workbook.Save("PrintErrorsNA.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


