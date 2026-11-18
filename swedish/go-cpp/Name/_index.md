---
title: "Namnklass"
linktitle: "Namn"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Namnklass. Inkapslar objektet som representerar namn i Go."
type: docs
weight: 200
url: /sv/go-cpp/name/
---

## Name class

Representerar ett definierat namn för ett cellområde.

```go

type Name struct  {
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
| [GetComment](./getcomment/) | Hämtar och anger kommentaren för namnet.Gäller endast för Excel 2007 eller högre versioner. |
| [SetComment](./setcomment/) | Hämtar och anger kommentaren för namnet.Gäller endast för Excel 2007 eller högre versioner. |
| [GetText](./gettext/) | Hämtar namntexten för objektet. |
| [SetText](./settext/) | Hämtar namntexten för objektet. |
| [GetFullText](./getfulltext/) | Hämtar namn  fulltext för objektet med omfångsinställningen. |
| [GetRefersTo](./getrefersto/) | Returnerar eller anger formeln som namnet är definierat att referera till, inledningsvis med ett likhetstecken. |
| [SetRefersTo_String](./setrefersto_string/) | Returnerar eller anger formeln som namnet är definierat att referera till, inledningsvis med ett likhetstecken. |
| [GetR1C1RefersTo](./getr1c1refersto/) | Hämtar eller anger en R1C1-referens för Namnet. |
| [SetR1C1RefersTo](./setr1c1refersto/) | Hämtar eller anger en R1C1-referens för Namnet. |
| [GetRefersTo_Bool_Bool](./getrefersto_bool_bool/) | Hämta referensen för detta Namn. |
| [GetRefersTo_Bool_Bool_Int_Int](./getrefersto_bool_bool_int_int/) | Hämta referensen för detta Namn baserat på specificerad cell. |
| [SetRefersTo_String_Bool_Bool](./setrefersto_string_bool_bool/) | Ange referensen för detta Namn. |
| [IsReferred](./isreferred/) | Indikerar om detta namn refereras av andra formler. |
| [IsVisible](./isvisible/) | Indikerar om namnet är synligt. |
| [SetIsVisible](./setisvisible/) | Indikerar om namnet är synligt. |
| [GetSheetIndex](./getsheetindex/) | Indikerar att detta namn tillhör Arbetsbok eller Arbetsblad.0 = Globalt namn, annars index till blad (en-baserat) |
| [SetSheetIndex](./setsheetindex/) | Indikerar att detta namn tillhör Arbetsbok eller Arbetsblad.0 = Globalt namn, annars index till blad (en-baserat) |
| [ToString](./tostring/) | Returnerar en sträng som representerar det aktuella Range-objektet. |
| [GetRanges](./getranges/) | Hämtar alla områden som refereras av detta namn. |
| [GetRanges_Bool](./getranges_bool/) | Hämtar alla områden som refereras av detta namn. |
| [GetReferredAreas](./getreferredareas/) | Hämtar alla referenser som refereras av detta namn. |
| [GetRange](./getrange/) | Hämtar området om detta namn refererar till ett område. |
| [GetRange_Bool](./getrange_bool/) | Hämtar området om detta namn refererar till ett område |
| [GetRange_Int_Int_Int](./getrange_int_int_int/) | Hämtar området om detta namn refererar till ett område.Om referensen för detta namn inte är absolut kan området vara olika för olika celler. |
