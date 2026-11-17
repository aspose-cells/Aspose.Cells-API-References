---
title: "SignatureLine Class"
linktitle: "SignatureLine"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "SignatureLine class. Incapsula l'oggetto che rappresenta signatureline in Go."
type: docs
weight: 200
url: /it/go-cpp/signatureline/
---

## SignatureLine class

Rappresenta la linea di firma.

```go

type SignatureLine struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewSignatureLine](./newsignatureline/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetId](./getid/) | Ottiene o imposta l'identificatore per questa linea di firma. |
| [SetId](./setid/) | Ottiene o imposta l'identificatore per questa linea di firma. |
| [GetProviderId](./getproviderid/) | Ottiene o imposta l'ID del provider di firma. |
| [SetProviderId](./setproviderid/) | Ottiene o imposta l'ID del provider di firma. |
| [GetSigner](./getsigner/) | Ottiene o imposta il firmatario. |
| [SetSigner](./setsigner/) | Ottiene o imposta il firmatario. |
| [GetTitle](./gettitle/) | Ottiene o imposta il titolo del cantante. |
| [SetTitle](./settitle/) | Ottiene o imposta il titolo del cantante. |
| [GetEmail](./getemail/) | Ottiene o imposta l'email del cantante. |
| [SetEmail](./setemail/) | Ottiene o imposta l'email del cantante. |
| [IsLine](./isline/) | Indica se è una linea di firma. |
| [SetIsLine](./setisline/) | Indica se è una linea di firma. |
| [GetAllowComments](./getallowcomments/) | Indica se i commenti possono essere allegati. |
| [SetAllowComments](./setallowcomments/) | Indica se i commenti possono essere allegati. |
| [GetShowSignedDate](./getshowsigneddate/) | Indica se mostrare la data di firma. |
| [SetShowSignedDate](./setshowsigneddate/) | Indica se mostrare la data di firma. |
| [GetInstructions](./getinstructions/) | Ottiene o imposta il testo mostrato all'utente al momento della firma. |
| [SetInstructions](./setinstructions/) | Ottiene o imposta il testo mostrato all'utente al momento della firma. |
| [GetSignatureLineType](./getsignaturelinetype/) | Ottiene o imposta il tipo di firma. Default - Quando il valore predefinito è impostato, il valore corrispondente di ProviderId è fissato a {0000000000-0000-0000-0000-0000000000}. Stamp - Quando il valore è Stamp, il valore corrispondente di ProviderId è solitamente {000CD6A4-0000-0000-C000-000000000046}. Custom - Quando il valore è Custom, il valore corrispondente di ProviderId di solito deve essere impostato dall'utente. dovrebbe essere ottenuto dalla documentazione fornita con il provider. |
| [SetSignatureLineType](./setsignaturelinetype/) | Ottiene o imposta il tipo di firma. Default - Quando il valore predefinito è impostato, il valore corrispondente di ProviderId è fissato a {0000000000-0000-0000-0000-0000000000}. Stamp - Quando il valore è Stamp, il valore corrispondente di ProviderId è solitamente {000CD6A4-0000-0000-C000-000000000046}. Custom - Quando il valore è Custom, il valore corrispondente di ProviderId di solito deve essere impostato dall'utente. dovrebbe essere ottenuto dalla documentazione fornita con il provider. |
