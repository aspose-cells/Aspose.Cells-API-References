---
title: "Enum TxtLoadStyleStrategy"
linktitle: "TxtLoadStyleStrategy"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Enum TxtLoadStyleStrategy. Encapsule l'objet qui représente txtloadstylestrategy dans Go."
type: docs
weight: 200
url: /fr/go-cpp/txtloadstylestrategy/
---

## TxtLoadStyleStrategy Enum

Spécifie comment appliquer le style aux valeurs analysées lors de la conversion d'une chaîne en nombre ou en date/heure.

```go

type TxtLoadStyleStrategy int32


```

## Champs

| Champ | Description |
| --- | --- |
| [None](./none/) | Ne définit pas de style pour la valeur analysée. |
| [BuiltIn](./builtin/) | Définit le style comme nombre/date-heure intégré lorsque la valeur analysée est une valeur numérique/date-heure simple. |
| [ExactFormat](./exactformat/) | Définit le format personnalisé exact pour la valeur analysée afin que la valeur formatée soit identique à l'entrée originale. |
