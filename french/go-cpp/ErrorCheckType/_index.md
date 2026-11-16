---
title: "ErrorCheckType Enum"
linktitle: "ErrorCheckType"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "ErrorCheckType enum. Encapsule l'objet qui représente errorchecktype en Go."
type: docs
weight: 200
url: /fr/go-cpp/errorchecktype/
---

## ErrorCheckType Enum

Représente tous les types de vérification d'erreur.

```go

type ErrorCheckType int32


```

## Champs

| Champ | Description |
| --- | --- |
| [EvaluationError](./evaluationerror/) | Ignorer les erreurs lorsque les cellules contiennent des formules qui entraînent une erreur. |
| [EmptyCellRef](./emptycellref/) | Ignorer les erreurs lorsque les formules font référence à des cellules vides. |
| [NumberStoredAsText](./numberstoredastext/) | Ignorer les erreurs lorsque les nombres sont formatés en texte ou précédés d'une apostrophe |
| [InconsistRange](./inconsistrange/) | Ignorer les erreurs lorsque les formules omettent certaines cellules dans une région. |
| [InconsistFormula](./inconsistformula/) | Ignorer les erreurs lorsqu'une formule dans une région de votre feuille de calcul diffère des autres formules de la même région. |
| [TwoDigitTextYear](./twodigittextyear/) | Ignorer les erreurs lorsque les formules contiennent des cellules formatées en texte avec des années représentées sur 2 chiffres. |
| [UnlockedFormula](./unlockedformula/) | Ignorer les erreurs lorsque les cellules déverrouillées contiennent des formules. |
| [TableDataValidation](./tabledatavalidation/) | Ignorer les erreurs lorsque la valeur d'une cellule dans un tableau ne respecte pas les règles de validation des données spécifiées. |
| [CalculatedColumn](./calculatedcolumn/) | Ignorer les erreurs lorsque les cellules contiennent une valeur différente de la formule d’une colonne calculée. |
