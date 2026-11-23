---
title: "Classe ErrorCheckOption"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ErrorCheckOption. Paramètre de vérification d'erreurs appliqué à certaines plages"
type: docs
url: /fr/net/aspose.cells/errorcheckoption/
---
## ErrorCheckOption class

Paramètre de vérification d'erreurs appliqué à certaines plages.

```csharp
public class ErrorCheckOption
```

## Méthodes

| Nom | Description |
| --- | --- |
| [AddRange](../../aspose.cells/errorcheckoption/addrange/)(CellArea) | Ajoute une plage influencée par ce paramètre. |
| [GetCountOfRange](../../aspose.cells/errorcheckoption/getcountofrange/)() | Obtient le nombre de plages influencées par ce paramètre. |
| [GetRange](../../aspose.cells/errorcheckoption/getrange/)(int) | Obtient la plage influencée de ce paramètre selon l'index donné. |
| [IsErrorCheck](../../aspose.cells/errorcheckoption/iserrorcheck/)(ErrorCheckType) | Vérifie si le type d'erreur donné sera vérifié. |
| [RemoveRange](../../aspose.cells/errorcheckoption/removerange/)(int) | Supprime une plage selon l'index donné. |
| [SetErrorCheck](../../aspose.cells/errorcheckoption/seterrorcheck/)(ErrorCheckType, bool) | Définit si le type d'erreur donné sera vérifié. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionDemo
    {
        public static void ErrorCheckOptionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenez la ErrorCheckOptionCollection de la feuille de calcul
            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;

            // Ajoutez une nouvelle ErrorCheckOption à la collection
            int optionIdx = opts.Add();
            ErrorCheckOption opt = opts[optionIdx];

            // Définissez les options de vérification d'erreurs
            opt.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            opt.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            opt.SetErrorCheck(ErrorCheckType.TextDate, false);
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.SetErrorCheck(ErrorCheckType.Validation, false);

            // Définissez une zone de cellules et ajoutez‑la à la ErrorCheckOption
            CellArea ca = CellArea.CreateCellArea("A1", "B10");
            opt.AddRange(ca);

            // Enregistrez le classeur
            workbook.Save("ErrorCheckOptionExample.xlsx");
            workbook.Save("ErrorCheckOptionExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


