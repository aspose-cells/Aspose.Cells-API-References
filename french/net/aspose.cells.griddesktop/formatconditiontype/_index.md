---
title: "Enum FormatConditionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridDesktop.FormatConditionType enum. Type de règle de format conditionnel"
type: docs
url: /fr/net/aspose.cells.griddesktop/formatconditiontype/
---
## FormatConditionType enumeration

Type de règle de format conditionnel.

```csharp
public enum FormatConditionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| CellValue | `0` | Cette règle de mise en forme conditionnelle compare la valeur d'une cellule à un résultat calculé par une formule, en utilisant un opérateur. |
| Expression | `1` | Cette règle de mise en forme conditionnelle contient une formule à évaluer. Lorsque le résultat de la formule est vrai, la cellule est mise en surbrillance. |
| ColorScale | `2` | Cette règle de mise en forme conditionnelle crée une échelle de couleur graduée sur les cellules. |
| DataBar | `3` | Cette règle de mise en forme conditionnelle affiche une barre de données graduée dans la plage de cellules. |
| IconSet | `4` | Cette règle de mise en forme conditionnelle applique des icônes aux cellules en fonction de leurs valeurs. |
| Top10 | `5` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules dont les valeurs se situent dans le groupe des N meilleures ou des N pires, selon la spécification. |
| UniqueValues | `6` | Cette règle de mise en forme conditionnelle met en surbrillance les valeurs uniques dans la plage. |
| DuplicateValues | `7` | Cette règle de mise en forme conditionnelle met en surbrillance les valeurs dupliquées. |
| ContainsText | `8` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant le texte donné. Équivalent à l'utilisation de la fonction feuille SEARCH() pour déterminer si la cellule contient le texte. |
| NotContainsText | `9` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui ne sont pas vides. Équivalent à l'utilisation de LEN(TRIM()). Cela signifie que si la cellule ne contient que des caractères que TRIM() supprimerait, elle est considérée comme vide. Une cellule vide est également considérée comme vide. |
| BeginsWith | `10` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules de la plage qui commencent par le texte donné. Équivalent à l'utilisation de la fonction feuille LEFT() et à la comparaison des valeurs. |
| EndsWith | `11` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules se terminant par le texte donné. Équivalent à l'utilisation de la fonction feuille RIGHT() et à la comparaison des valeurs. |
| ContainsBlanks | `12` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont complètement vides. Équivalent à l'utilisation de LEN(TRIM()). Cela signifie que si la cellule ne contient que des caractères que TRIM() supprimerait, elle est considérée comme vide. Une cellule vide est également considérée comme vide. |
| NotContainsBlanks | `13` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui ne sont pas vides. Équivalent à l'utilisation de LEN(TRIM()). Cela signifie que si la cellule ne contient que des caractères que TRIM() supprimerait, elle est considérée comme vide. Une cellule vide est également considérée comme vide. |
| ContainsErrors | `14` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant des erreurs de formule. Équivalent à l'utilisation de la fonction feuille ISERROR() pour déterminer s'il y a une erreur de formule. |
| NotContainsErrors | `15` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules sans erreurs de formule. Équivalent à l'utilisation de la fonction feuille ISERROR() pour déterminer s'il y a une erreur de formule. |
| TimePeriod | `16` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant des dates dans la période spécifiée. La valeur sous‑jacent de la cellule est évaluée, ainsi la cellule n’a pas besoin d’être formatée en tant que date pour être évaluée. Par exemple, avec une cellule contenant la valeur 38913, la mise en forme conditionnelle sera appliquée si la règle nécessite une valeur du 7/14/2006. |
| AboveAverage | `17` | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont au-dessus ou en dessous de la moyenne de toutes les valeurs de la plage. |

### Voir aussi

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


