---
title: "Enum FormatConditionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.FormatConditionType. Type de règle de format conditionnel"
type: docs
url: /fr/net/aspose.cells/formatconditiontype/
---
## FormatConditionType enumeration

Type de règle de format conditionnel.

```csharp
public enum FormatConditionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| CellValue | `1` | Cette règle de mise en forme conditionnelle compare la valeur d'une cellule à un résultat calculé par une formule, en utilisant un opérateur. |
| Expression | `2` | Cette règle de mise en forme conditionnelle contient une formule à évaluer. Lorsque le résultat de la formule est vrai, la cellule est mise en surbrillance. |
| Top10 | `4` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules dont les valeurs se situent dans le groupe des N meilleures ou des N pires, selon la spécification. |
| UniqueValues | `8` | Cette règle de mise en forme conditionnelle met en surbrillance les valeurs uniques dans la plage. |
| DuplicateValues | `16` | Cette règle de mise en forme conditionnelle met en surbrillance les valeurs dupliquées. |
| ContainsText | `32` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant le texte donné. Équivalent à l'utilisation de la fonction feuille SEARCH() pour déterminer si la cellule contient le texte. |
| NotContainsText | `64` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui ne contiennent pas le texte donné. Équivalent à l'utilisation de la fonction feuille SEARCH() pour déterminer si la cellule contient le texte ou non. |
| BeginsWith | `128` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules de la plage qui commencent par le texte donné. Équivalent à l'utilisation de la fonction feuille LEFT() et à la comparaison des valeurs. |
| EndsWith | `256` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules se terminant par le texte donné. Équivalent à l'utilisation de la fonction feuille RIGHT() et à la comparaison des valeurs. |
| ContainsBlanks | `512` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont complètement vides. Équivalent à l'utilisation de LEN(TRIM()). Cela signifie que si la cellule ne contient que des caractères que TRIM() supprimerait, elle est considérée comme vide. Une cellule vide est également considérée comme vide. |
| NotContainsBlanks | `1024` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui ne sont pas vides. Équivalent à l'utilisation de LEN(TRIM()). Cela signifie que si la cellule ne contient que des caractères que TRIM() supprimerait, elle est considérée comme vide. Une cellule vide est également considérée comme vide. |
| ContainsErrors | `2048` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant des erreurs de formule. Équivalent à l'utilisation de la fonction feuille ISERROR() pour déterminer s'il y a une erreur de formule. |
| NotContainsErrors | `4096` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules sans erreurs de formule. Équivalent à l'utilisation de la fonction feuille ISERROR() pour déterminer s'il y a une erreur de formule. |
| TimePeriod | `8192` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant des dates dans la période spécifiée. La valeur sous‑jacent de la cellule est évaluée, ainsi la cellule n’a pas besoin d’être formatée en tant que date pour être évaluée. Par exemple, avec une cellule contenant la valeur 38913, la mise en forme conditionnelle sera appliquée si la règle nécessite une valeur du 7/14/2006. |
| AboveAverage | `16384` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont au-dessus ou en dessous de la moyenne de toutes les valeurs de la plage. |
| ColorScale | `32768` | Cette règle de mise en forme conditionnelle crée une échelle de couleur graduée sur les cellules. |
| DataBar | `65536` | Cette règle de mise en forme conditionnelle affiche une barre de données graduée dans la plage de cellules. |
| IconSet | `131072` | Cette règle de mise en forme conditionnelle applique des icônes aux cellules en fonction de leurs valeurs. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionTypeDemo
    {
        public static void FormatConditionTypeExample()
        {
            // Créez un nouveau classeur.
            Workbook workbook = new Workbook();

            // Obtenez la première feuille de calcul.
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoute une mise en forme conditionnelle vide
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Définit la plage de mise en forme conditionnelle.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Ajoute une condition pour AboveAverage
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Définition des propriétés pour AboveAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // Ajoute une condition pour CellValue
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = Color.Red;

            // Ajoute une condition pour ContainsText
            int conditionIndex3 = fcs.AddCondition(FormatConditionType.ContainsText);
            FormatCondition fc3 = fcs[conditionIndex3];
            fc3.Text = "Sample";
            fc3.Style.BackgroundColor = Color.Green;

            // Enregistrez le fichier Excel
            workbook.Save("FormatConditionTypeExample.xlsx");
            workbook.Save("FormatConditionTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


