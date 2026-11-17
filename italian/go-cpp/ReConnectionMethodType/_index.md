---
title: "ReConnectionMethodType Enum"
linktitle: "ReConnectionMethodType"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "ReConnectionMethodType enum. Incapsula l'oggetto che rappresenta reconnectionmethodtype in Go."
type: docs
weight: 200
url: /it/go-cpp/reconnectionmethodtype/
---

## ReConnectionMethodType Enum

Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce.

```go

type ReConnectionMethodType int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [Required](./required/) | Al refresh utilizza le informazioni di connessione esistenti e se risultano non valide, ottieni le informazioni di connessione aggiornate, se disponibili dal file di connessione esterno. |
| [Always](./always/) | Ad ogni refresh ottieni le informazioni di connessione aggiornate dal file di connessione esterno, se disponibili, e usale al posto delle informazioni di connessione esistenti. In questo caso l'aggiornamento dei dati fallirà se il file di connessione esterno non è disponibile. |
| [Never](./never/) | Non ottenere mai le informazioni di connessione aggiornate dal file di connessione esterno, anche se è disponibile e anche se le informazioni di connessione esistenti sono non valide |
