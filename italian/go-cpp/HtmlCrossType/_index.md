---
title: "HtmlCrossType Enum"
linktitle: "HtmlCrossType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "HtmlCrossType enum. Incapsula l'oggetto che rappresenta htmlcrosstype in Go."
type: docs
weight: 200
url: /it/go-cpp/htmlcrosstype/
---

## HtmlCrossType Enum

Rappresenta cinque tipi di stringa incrociata HTML.

```go

type HtmlCrossType int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [Default](./default/) | Visualizza come MS Excel, dipende dalla cella successiva. Se la cella successiva è nulla, la stringa attraverserà, altrimenti verrà troncata |
| [MSExport](./msexport/) | Visualizza la stringa come MS Excel esportando html. |
| [Cross](./cross/) | Visualizza la stringa incrociata HTML, questa prestazione per la creazione di file HTML di grandi dimensioni sarà più di dieci volte più veloce rispetto all'impostazione del valore su Default o FitToCell. |
| [CrossHideRight](./crosshideright/) | Visualizza la stringa incrociata HTML e nascondi la stringa di destra quando i testi si sovrappongono. |
| [FitToCell](./fittocell/) | Visualizza solo la stringa all'interno della larghezza della cella. |
