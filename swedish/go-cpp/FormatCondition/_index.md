---
title: "FormatCondition klass"
linktitle: "FormatCondition"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "FormatCondition klass. Inkapslar objektet som representerar formatcondition i Go."
type: docs
weight: 200
url: /sv/go-cpp/formatcondition/
---

## FormatCondition class

Representerar villkorsformatets villkor.

```go

type FormatCondition struct  {
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
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | Hämtar värdet eller uttrycket som är associerat med detta formatvillkor. |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | Hämtar värdet eller uttrycket som är associerat med detta formatvillkor. |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | Hämtar värdet eller uttrycket för cellens villkorsformatering. |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | Hämtar värdet eller uttrycket för cellens villkorsformatering. |
| [SetFormulas](./setformulas/) | Ställer in värdet eller uttrycket som är associerat med detta formatvillkor. |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | Ställer in värdet eller uttrycket som är associerat med detta formatvillkor. |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | Ställer in värdet eller uttrycket som är associerat med detta formatvillkor. |
| [GetFormula1](./getformula1/) | Hämtar och anger värdet eller uttrycket som är associerat med villkorsformatering. |
| [SetFormula1_String](./setformula1_string/) | Hämtar och anger värdet eller uttrycket som är associerat med villkorsformatering. |
| [GetFormula1_Int_Int](./getformula1_int_int/) | Hämtar formeln för cellens villkorsformatering. |
| [GetFormula2](./getformula2/) | Hämtar och anger värdet eller uttrycket som är associerat med villkorsformatering. |
| [SetFormula2_String](./setformula2_string/) | Hämtar och anger värdet eller uttrycket som är associerat med villkorsformatering. |
| [GetFormula2_Int_Int](./getformula2_int_int/) | Hämtar formeln för cellens villkorsformatering. |
| [GetOperator](./getoperator/) | Hämtar och anger typen av villkorlig formatoperator. |
| [SetOperator](./setoperator/) | Hämtar och anger typen av villkorlig formatoperator. |
| [GetStopIfTrue](./getstopiftrue/) | Sant, inga regler med lägre prioritet får tillämpas över denna regel när regeln utvärderas till sant. Gäller endast för Excel 2007; |
| [SetStopIfTrue](./setstopiftrue/) | Sant, inga regler med lägre prioritet får tillämpas över denna regel när regeln utvärderas till sant. Gäller endast för Excel 2007; |
| [GetPriority](./getpriority/) | Prioriteten för detta villkorsformateringsregel. Detta värde används för att avgöra vilken format som ska utvärderas och renderas. Lägre numeriska värden har högre prioritet än högre numeriska värden, där '1' är den högsta prioriteten. |
| [SetPriority](./setpriority/) | Prioriteten för detta villkorsformateringsregel. Detta värde används för att avgöra vilken format som ska utvärderas och renderas. Lägre numeriska värden har högre prioritet än högre numeriska värden, där '1' är den högsta prioriteten. |
| [GetStyle](./getstyle/) | Hämtar eller anger stil för villkorligt formaterade cellområden. |
| [SetStyle](./setstyle/) | Hämtar eller anger stil för villkorligt formaterade cellområden. |
| [GetType](./gettype/) | Hämtar och anger om den villkorliga formattypen. |
| [SetType](./settype/) | Hämtar och anger om den villkorliga formattypen. |
| [GetIconSet](./geticonset/) | Hämta den villkorsformateringens "IconSet"-instans. Standardinstansens IconSetType är TrafficLights31. Gäller endast för typ = IconSet. |
| [GetDataBar](./getdatabar/) | Hämta den villkorsformateringens "DataBar"-instans. Standardinstansens färg är blå. Gäller endast för typ = DataBar. |
| [GetColorScale](./getcolorscale/) | Hämta den villkorsformateringens "ColorScale"-instans. Standardinstansen är en "grön-gul-röd" 3ColorScale. Gäller endast för typ = ColorScale. |
| [GetTop10](./gettop10/) | Hämta den villkorsformateringens "Top10"-instans. Standardinstansens regel markerar celler vars värden faller i de 10 bästa. Gäller endast för typ = Top10. |
| [GetAboveAverage](./getaboveaverage/) | Hämta den villkorsformateringens "AboveAverage"-instans. Standardinstansens regel markerar celler som ligger över genomsnittet för alla värden i intervallet. Gäller endast för typ = AboveAverage. |
| [GetText](./gettext/) | Textvärdet i en "text contains"-regel för villkorsstyrd formatering. Gäller endast för typ = containsText, notContainsText, beginsWith och endsWith. Standardvärdet är null. |
| [SetText](./settext/) | Textvärdet i en "text contains"-regel för villkorsstyrd formatering. Gäller endast för typ = containsText, notContainsText, beginsWith och endsWith. Standardvärdet är null. |
| [GetTimePeriod](./gettimeperiod/) | Den tillämpliga tidsperioden i en "date occurrin"-regel för villkorsstyrd formatering. Gäller endast för typ är timePeriod. Standardvärdet är TimePeriodType.Today. |
| [SetTimePeriod](./settimeperiod/) | Den tillämpliga tidsperioden i en "date occurrin"-regel för villkorsstyrd formatering. Gäller endast för typ är timePeriod. Standardvärdet är TimePeriodType.Today. |
