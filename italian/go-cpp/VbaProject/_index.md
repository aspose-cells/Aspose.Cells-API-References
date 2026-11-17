---
title: "VbaProject Classe"
linktitle: "VbaProject"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "VbaProject class. Incapsula l'oggetto che rappresenta vbaproject in Go."
type: docs
weight: 200
url: /it/go-cpp/vbaproject/
---

## VbaProject class

Rappresenta il progetto VBA.

```go

type VbaProject struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [Sign](./sign/) | Firma questo progetto VBA con una DigitalSignature |
| [IsValidSigned](./isvalidsigned/) | Indica se la firma del progetto VBA è valida o meno. |
| [GetCertRawData](./getcertrawdata/) | Ottiene i dati grezzi del certificato se questo progetto VBA è firmato. |
| [GetEncoding](./getencoding/) | Ottiene e imposta la codifica del progetto VBA. |
| [SetEncoding](./setencoding/) | Ottiene e imposta la codifica del progetto VBA. |
| [GetName](./getname/) | Ottiene e imposta il nome del progetto VBA. |
| [SetName](./setname/) | Ottiene e imposta il nome del progetto VBA. |
| [IsSigned](./issigned/) | Indica se il VBAcode è firmato o meno. |
| [Protect](./protect/) | Protegge o rimuove la protezione di questo progetto VBA. |
| [IsProtected](./isprotected/) | Indica se questo progetto VBA è protetto. |
| [IsLockedForView](./islockedforview/) | Indica se questo progetto VBA è bloccato per la visualizzazione. Se vero, i codici non saranno visibili. |
| [Copy](./copy/) | Copia il progetto VBA da un altro file. |
| [GetModules](./getmodules/) | Ottiene tutti gli oggetti VbaModule. |
| [GetReferences](./getreferences/) | Ottiene tutti i riferimenti del progetto VBA. |
| [ValidatePassword](./validatepassword/) | Convalida la password di protezione. |
