---
title: "FormatConditionType Enum"
linktitle: "FormatConditionType"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "FormatConditionType enum. Encapsule l'objet qui représente formatconditiontype en Go."
type: docs
weight: 200
url: /fr/go-cpp/formatconditiontype/
---

## FormatConditionType Enum

Type de règle de format conditionnel.

```go

type FormatConditionType int32


```

## Champs

| Champ | Description |
| --- | --- |
| [CellValue](./cellvalue/) | Cette règle de mise en forme conditionnelle compare la valeur d'une cellule à un résultat calculé par une formule, en utilisant un opérateur. |
| [Expression](./expression/) | Cette règle de mise en forme conditionnelle contient une formule à évaluer. Lorsque le résultat de la formule est vrai, la cellule est mise en surbrillance. |
| [Top10](./top10/) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules dont les valeurs se situent dans le groupe supérieur N ou inférieur N, selon spécification. |
| [UniqueValues](./uniquevalues/) | Cette règle de mise en forme conditionnelle met en surbrillance les valeurs uniques dans la plage. |
| [DuplicateValues](./duplicatevalues/) | Cette règle de mise en forme conditionnelle met en surbrillance les valeurs dupliquées. |
| [ContainsText](./containstext/) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant le texte donné. Équivalent à l'utilisation de la fonction feuille SEARCH() pour déterminer si la cellule contient le texte. |
| [NotContainsText](./notcontainstext/) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui ne contiennent pas le texte donné. Équivalent à l'utilisation de la fonction feuille SEARCH() pour déterminer si la cellule contient le texte ou non. |
| [BeginsWith](./beginswith/) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules de la plage qui commencent par le texte donné. Équivalent à l'utilisation de la fonction feuille LEFT() et à la comparaison des valeurs. |
| [EndsWith](./endswith/) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules se terminant par le texte donné. Équivalent à l'utilisation de la fonction feuille RIGHT() et à la comparaison des valeurs. |
| [ContainsBlanks](./containsblanks/) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont complètement vides. Équivalent à l'utilisation de LEN(TRIM()). Cela signifie que si la cellule ne contient que des caractères que TRIM() supprimerait, elle est considérée comme vide. Une cellule vide est également considérée comme vide. |
| [NotContainsBlanks](./notcontainsblanks/) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui ne sont pas vides. Équivalent à l'utilisation de LEN(TRIM()). Cela signifie que si la cellule ne contient que des caractères que TRIM() supprimerait, elle est considérée comme vide. Une cellule vide est également considérée comme vide. |
| [ContainsErrors](./containserrors/) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules avec des erreurs de formule. Équivalent à l'utilisation de la fonction feuille ISERROR() pour déterminer s'il y a une erreur de formule. |
| [NotContainsErrors](./notcontainserrors/) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules sans erreurs de formule. Équivalent à l'utilisation de la fonction feuille ISERROR() pour déterminer s'il y a une erreur de formule. |
| [TimePeriod](./timeperiod/) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules contenant des dates dans la période spécifiée. La valeur sous-jacente de la cellule est évaluée, de sorte que la cellule n'a pas besoin d'être formatée en tant que date pour être évaluée. Par exemple, avec une cellule contenant la valeur 38913, le format conditionnel sera appliqué si la règle nécessite une valeur du 14/07/2006. |
| [AboveAverage](./aboveaverage/) | Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont au-dessus ou en dessous de la moyenne de toutes les valeurs de la plage. |
| [ColorScale](./colorscale/) | Cette règle de mise en forme conditionnelle crée une échelle gradatedcolor sur les cellules. |
| [DataBar](./databar/) | Cette règle de mise en forme conditionnelle affiche une barre gradateddata dans la plage de cellules. |
| [IconSet](./iconset/) | Cette règle de mise en forme conditionnelle applique des icônes aux cellsaccording selon leurs valeurs. |
