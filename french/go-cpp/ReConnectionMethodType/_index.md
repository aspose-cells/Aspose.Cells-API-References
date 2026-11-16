---
title: "ReConnectionMethodType Enum"
linktitle: "ReConnectionMethodType"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Enum ReConnectionMethodType. Encapsule l'objet qui représente reconnectionmethodtype en Go."
type: docs
weight: 200
url: /fr/go-cpp/reconnectionmethodtype/
---

## ReConnectionMethodType Enum

Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue.

```go

type ReConnectionMethodType int32


```

## Champs

| Champ | Description |
| --- | --- |
| [Required](./required/) | Lors du rafraîchissement, utilisez les informations de connexion existantes et, si elles s'avèrent invalides, obtenez les informations de connexion mises à jour, si elles sont disponibles dans le fichier de connexion externe. |
| [Always](./always/) | À chaque rafraîchissement, obtenez les informations de connexion mises à jour à partir du fichier de connexion externe, si disponible, et utilisez-les à la place des informations de connexion existantes. Dans ce cas, le rafraîchissement des données échouera si le fichier de connexion externe est indisponible. |
| [Never](./never/) | Ne jamais obtenir les informations de connexion mises à jour à partir du fichier de connexion externe, même si elles sont disponibles et même si les informations de connexion existantes sont invalides. |
