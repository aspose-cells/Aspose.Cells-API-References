---
title: "Enumération TxtValueQuoteType"
linktitle: "TxtValueQuoteType"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Enumération TxtValueQuoteType. Encapsule l'objet qui représente txtvaluequotetype en Go."
type: docs
weight: 200
url: /fr/go-cpp/txtvaluequotetype/
---

## TxtValueQuoteType Enum

Spécifie le type d'utilisation des guillemets pour les valeurs dans les fichiers au format texte.

```go

type TxtValueQuoteType int32


```

## Champs

| Champ | Description |
| --- | --- |
| [Normal](./normal/) | Toutes les valeurs contenant des caractères spéciaux tels que les guillemets, le caractère de séparation seront entre guillemets. Même comportement que celui de MS Excel lors de l'exportation d'un fichier texte. |
| [Always](./always/) | Toutes les valeurs seront toujours entre guillemets. |
| [Minimum](./minimum/) | Citez uniquement les valeurs lorsque c'est nécessaire. Par exemple, si une valeur contient un guillemet mais que le guillemet n'est pas au début de cette valeur, cette valeur ne sera pas citée. |
| [Never](./never/) | Aucune valeur ne sera citée. Le fichier texte exporté avec ce type peut ne pas être relu correctement parce que les guillemets nécessaires sont absents. |
