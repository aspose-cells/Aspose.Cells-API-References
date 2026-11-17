---
title: "ControlMatchEntryType Enum"
linktitle: "ControlMatchEntryType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "ControlMatchEntryType enum. Incapsula l'oggetto che rappresenta controlmatchentrytype in Go."
type: docs
weight: 200
url: /it/go-cpp/controlmatchentrytype/
---

## ControlMatchEntryType Enum

Rappresenta come una ListBox o ComboBox ricerca l'elenco mentre l'utente digita.

```go

type ControlMatchEntryType int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [FirstLetter](./firstletter/) | Il controllo cerca la voce successiva che inizia con il carattere inserito.Digitare ripetutamente la stessa lettera scorre tutte le voci che iniziano con quella lettera. |
| [Complete](./complete/) | Man mano che ogni carattere viene digitato, il controllo cerca una voce che corrisponda a tutti i caratteri inseriti. |
| [None](./none/) | L'elenco non verrà cercato quando i caratteri vengono digitati. |
