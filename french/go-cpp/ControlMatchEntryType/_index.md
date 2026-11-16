---
title: "ControlMatchEntryType Enum"
linktitle: "ControlMatchEntryType"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "ControlMatchEntryType enum. Encapsule l'objet qui représente controlmatchentrytype en Go."
type: docs
weight: 200
url: /fr/go-cpp/controlmatchentrytype/
---

## ControlMatchEntryType Enum

Représente la façon dont une ListBox ou une ComboBox recherche dans sa liste pendant que l'utilisateur saisit.

```go

type ControlMatchEntryType int32


```

## Champs

| Champ | Description |
| --- | --- |
| [FirstLetter](./firstletter/) | Le contrôle recherche la prochaine entrée qui commence par le caractère saisi.Répéter la frappe de la même lettre parcourt toutes les entrées commençant par cette lettre. |
| [Complete](./complete/) | À chaque caractère tapé, le contrôle recherche une entrée correspondant à tous les caractères saisis. |
| [None](./none/) | La liste ne sera pas recherchée lorsque des caractères sont tapés. |
