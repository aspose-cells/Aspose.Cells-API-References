---
title: "ReferredArea Klass"
linktitle: "ReferredArea"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ReferredArea-klass. Inkapslar objektet som representerar referredarea i Go."
type: docs
weight: 200
url: /sv/go-cpp/referredarea/
---

## ReferredArea class

Representerar ett område som refereras av formeln.

```go

type ReferredArea struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [IsExternalLink](./isexternallink/) | Indikerar om detta är en extern länk. |
| [GetExternalFileName](./getexternalfilename/) | Hämta det externa filnamnet om detta är en extern referens. |
| [GetSheetName](./getsheetname/) | Indikerar vilket blad denna referens finns i. |
| [GetSheetNames](./getsheetnames/) | Namn på alla arbetsblad som denna instans refererar till. |
| [IsEntireRow](./isentirerow/) | Indikerar om detta område innehåller alla kolumner (hela raden). |
| [IsEntireColumn](./isentirecolumn/) | Indikerar om detta område innehåller alla rader (hela kolumnen). |
| [IsArea](./isarea/) | Indikerar om detta är ett område. |
| [GetEndColumn](./getendcolumn/) | Det sista kolumnen i området. |
| [GetStartColumn](./getstartcolumn/) | Den första kolumnen i området. |
| [GetEndRow](./getendrow/) | Den sista raden i området. |
| [GetStartRow](./getstartrow/) | Den första raden i området. |
| [GetValues](./getvalues/) | Hämtar cellvärden i detta område. |
| [GetValues_Bool](./getvalues_bool/) | Hämtar cellvärden i detta område. |
| [GetValue_Int_Int](./getvalue_int_int/) | Hämtar cellvärde med given förskjutning från det övre vänstra hörnet av detta område. |
| [GetValue_Int_Int_Bool](./getvalue_int_int_bool/) | Hämtar cellvärde med given förskjutning från det övre vänstra hörnet av detta område. |
| [ToString](./tostring/) | Returnerar referensadressen för detta område. Vanligtvis är det adressen för referensen som kan användas i en formel, till exempel "Sheet1!A1:C3". |
