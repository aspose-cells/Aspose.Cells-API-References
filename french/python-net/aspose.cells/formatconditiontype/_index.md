---
title: FormatConditionType dénombrement
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 2100
url: /fr/python-net/aspose.cells/formatconditiontype/
is_root: false
---
##  FormatConditionType dénombrement
Type de règle de mise en forme conditionnelle.



Le type FormatConditionType expose les membres suivants :

###  Des champs
| Champ| Description|
| :- | :- |
| CELL_VALUE | Cette règle de mise en forme conditionnelle compare une valeur de cellule<br/> à un résultat calculé de formule, à l'aide d'un opérateur.|
| EXPRESSION | Cette règle de mise en forme conditionnelle contient une formule pour<br/>évaluer. Lorsque le résultat de la formule est vrai, la cellule est<br/> Souligné.|
| COLOR_SCALE | Cette règle de mise en forme conditionnelle crée un dégradé<br/> échelle de couleur sur les cellules.|
| DATA_BAR | Cette règle de mise en forme conditionnelle affiche un dégradé<br/> barre de données dans la plage de cellules.|
| ICON_SET | Cette règle de mise en forme conditionnelle applique des icônes aux cellules<br/>selon leurs valeurs.|
| TOP10 | Cette règle de mise en forme conditionnelle met en évidence les cellules dont<br/>les valeurs tombent dans la tranche supérieure N ou inférieure N, comme<br/> spécifié.|
| UNIQUE_VALUES | Cette règle de mise en forme conditionnelle met en évidence les<br/> valeurs dans la plage.|
| DUPLICATE_VALUES | Cette règle de mise en forme conditionnelle met en évidence les doublons<br/> valeurs.|
| CONTAINS_TEXT | Cette règle de mise en forme conditionnelle met en surbrillance les cellules<br/>contenant un texte donné. Équivalent à l'utilisation de SEARCH()<br/>fonction de feuille pour déterminer si la cellule contient<br/> le texte.|
| NOT_CONTAINS_TEXT | Cette règle de mise en forme conditionnelle met en évidence les cellules qui<br/>ne contiennent pas de texte donné. Équivalent de l'utilisation de SEARCH()<br/>fonction de feuille pour déterminer si la cellule contient<br/> le texte ou non.|
| BEGINS_WITH | Cette règle de mise en forme conditionnelle met en surbrillance les cellules du<br/>plage commençant par le texte donné. Équivalent à<br/> en utilisant la fonction de feuille LEFT() et en comparant les valeurs.|
| ENDS_WITH | Cette règle de mise en forme conditionnelle met en surbrillance les cellules se terminant<br/>avec un texte donné. Équivalent à l'utilisation de la feuille RIGHT()<br/> fonction et comparer les valeurs.|
| CONTAINS_BLANKS | Cette règle de mise en forme conditionnelle met en évidence les cellules qui<br/>sont complètement vierges. Equivalent d'utiliser LEN(TRIM()).<br/>Cela signifie que si la cellule ne contient que des caractères<br/>que TRIM() supprimerait, alors il est considéré comme vide.<br/> Une cellule vide est également considérée comme vide.|
| NOT_CONTAINS_BLANKS | Cette règle de mise en forme conditionnelle met en évidence les cellules qui<br/>ne sont pas vides. Equivalent d'utiliser LEN(TRIM()). Ce<br/>signifie que si la cellule ne contient que des caractères qui<br/>TRIM() supprimerait, alors il est considéré comme vide. Un<br/> la cellule vide est également considérée comme vide.|
| CONTAINS_ERRORS | Cette règle de mise en forme conditionnelle met en surbrillance les cellules avec<br/>erreurs de formule. Équivalent à l'utilisation de la feuille ISERROR()<br/> fonction pour déterminer s'il y a une erreur de formule.|
| NOT_CONTAINS_ERRORS | Cette règle de mise en forme conditionnelle met en surbrillance les cellules<br/>sans erreur de formule. Équivalent à l'utilisation d'ISERROR()<br/> fonction de feuille pour déterminer s'il y a une erreur de formule.|
| TIME_PERIOD | Cette règle de mise en forme conditionnelle met en surbrillance les cellules<br/>contenant des dates dans la période spécifiée. Le<br/>la valeur sous-jacente de la cellule est évaluée, donc la<br/>la cellule n'a pas besoin d'être formatée comme une date pour être<br/>évalué. Par exemple, avec une cellule contenant le<br/>valeur 38913 le format conditionnel doit être appliqué si<br/> la règle requiert une valeur de 14/07/2006.|
| ABOVE_AVERAGE | Cette règle de mise en forme conditionnelle met en évidence les cellules qui<br/>sont au-dessus ou au-dessous de la moyenne pour toutes les valeurs de la<br/> gamme.|



###  Voir également
* module [aspose.cells](..)
