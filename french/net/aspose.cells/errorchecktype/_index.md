---
title: "Enum ErrorCheckType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ErrorCheckType enum. Représente tous les types de vérification d'erreurs"
type: docs
url: /fr/net/aspose.cells/errorchecktype/
---
## ErrorCheckType enumeration

Représente tous les types de vérification d'erreur.

```csharp
public enum ErrorCheckType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| EvaluationError | `1` | Ignorez les erreurs lorsque les cellules contiennent des formules qui entraînent une erreur. |
| Calc | `1` |  |
| EmptyCellRef | `2` | Ignorer les erreurs lorsque les formules font référence à des cellules vides. |
| NumberStoredAsText | `4` | Ignorer les erreurs lorsque les nombres sont formatés en texte ou sont précédés d'une apostrophe |
| TextNumber | `4` | Ignorer les erreurs lorsque les nombres sont formatés en texte ou sont précédés d'une apostrophe |
| InconsistRange | `8` | Ignorer les erreurs lorsque les formules omettent certaines cellules dans une région. |
| InconsistFormula | `16` | Ignorer les erreurs lorsqu'une formule dans une région de votre feuille de calcul diffère des autres formules de la même région. |
| TwoDigitTextYear | `32` | Ignorer les erreurs lorsque les formules contiennent des cellules formatées en texte avec des années représentées sur 2 chiffres. |
| TextDate | `32` | Ignorer les erreurs lorsque les formules contiennent des cellules formatées en texte avec des années représentées sur 2 chiffres. |
| UnlockedFormula | `64` | Ignorer les erreurs lorsque des cellules déverrouillées contiennent des formules. |
| UnproctedFormula | `64` | Ignorer les erreurs lorsque des cellules déverrouillées contiennent des formules. |
| TableDataValidation | `128` | Ignorer les erreurs lorsque la valeur d'une cellule dans un tableau ne respecte pas les règles de validation des données spécifiées. |
| Validation | `128` | Ignorer les erreurs lorsque la valeur d'une cellule dans un tableau ne respecte pas les règles de validation des données spécifiées. |
| CalculatedColumn | `129` | Ignorer les erreurs lorsque les cellules contiennent une valeur différente de la formule d'une colonne calculée. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckTypeDemo
    {
        public static void ErrorCheckTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la ErrorCheckOptionCollection
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;

            // Ajouter une nouvelle ErrorCheckOption
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];

            // Définir divers types de vérification d'erreurs sur false
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.Validation, false);

            // Définir une zone de cellules pour l'option de vérification d'erreurs
            CellArea cellArea = CellArea.CreateCellArea("A1", "B10");
            errorCheckOption.AddRange(cellArea);

            // Enregistrez le classeur
            workbook.Save("ErrorCheckTypeExample.xlsx");
            workbook.Save("ErrorCheckTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


