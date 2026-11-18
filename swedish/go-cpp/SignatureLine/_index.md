---
title: "SignatureLine Klass"
linktitle: "SignatureLine"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "SignatureLine klass. Inkapslar objektet som representerar signatureline i Go."
type: docs
weight: 200
url: /sv/go-cpp/signatureline/
---

## SignatureLine class

Representerar signaturlinjen.

```go

type SignatureLine struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewSignatureLine](./newsignatureline/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetId](./getid/) | Hämtar eller anger identifierare för denna signaturlinje. |
| [SetId](./setid/) | Hämtar eller anger identifierare för denna signaturlinje. |
| [GetProviderId](./getproviderid/) | Hämtar eller anger ID för signaturleverantör. |
| [SetProviderId](./setproviderid/) | Hämtar eller anger ID för signaturleverantör. |
| [GetSigner](./getsigner/) | Hämtar eller anger undertecknaren. |
| [SetSigner](./setsigner/) | Hämtar eller anger undertecknaren. |
| [GetTitle](./gettitle/) | Hämtar eller anger titeln för undertecknaren. |
| [SetTitle](./settitle/) | Hämtar eller anger titeln för undertecknaren. |
| [GetEmail](./getemail/) | Hämtar eller anger e‑post för undertecknaren. |
| [SetEmail](./setemail/) | Hämtar eller anger e‑post för undertecknaren. |
| [IsLine](./isline/) | Indikerar om det är en signaturlinje. |
| [SetIsLine](./setisline/) | Indikerar om det är en signaturlinje. |
| [GetAllowComments](./getallowcomments/) | Indikerar om kommentarer kan bifogas. |
| [SetAllowComments](./setallowcomments/) | Indikerar om kommentarer kan bifogas. |
| [GetShowSignedDate](./getshowsigneddate/) | Indikerar om signeringsdatum ska visas. |
| [SetShowSignedDate](./setshowsigneddate/) | Indikerar om signeringsdatum ska visas. |
| [GetInstructions](./getinstructions/) | Hämtar eller anger texten som visas för användaren vid signering. |
| [SetInstructions](./setinstructions/) | Hämtar eller anger texten som visas för användaren vid signering. |
| [GetSignatureLineType](./getsignaturelinetype/) | Hämtar eller anger signaturtypen. Default - När standardvärdet är angivet, är det motsvarande ProviderId‑värdet fastställt till {0000000000-0000-0000-0000-0000000000}. Stamp - När värdet är Stamp, är det motsvarande ProviderId‑värdet vanligtvis {000CD6A4-0000-0000-C000-000000000046}. Custom - När värdet är Custom, måste det motsvarande ProviderId‑värdet vanligtvis anges av användaren. Det bör hämtas från dokumentationen som medföljer leverantören. |
| [SetSignatureLineType](./setsignaturelinetype/) | Hämtar eller anger signaturtypen. Default - När standardvärdet är angivet, är det motsvarande ProviderId‑värdet fastställt till {0000000000-0000-0000-0000-0000000000}. Stamp - När värdet är Stamp, är det motsvarande ProviderId‑värdet vanligtvis {000CD6A4-0000-0000-C000-000000000046}. Custom - När värdet är Custom, måste det motsvarande ProviderId‑värdet vanligtvis anges av användaren. Det bör hämtas från dokumentationen som medföljer leverantören. |
