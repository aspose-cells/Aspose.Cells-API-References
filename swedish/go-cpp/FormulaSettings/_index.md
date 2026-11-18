---
title: "FormulaSettings klass"
linktitle: "FormulaSettings"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "FormulaSettings klass. Inkapslar objektet som representerar formulasettings i Go."
type: docs
weight: 200
url: /sv/go-cpp/formulasettings/
---

## FormulaSettings class

Inställningar för formler och beräkning.

```go

type FormulaSettings struct  {
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
| [GetCalculateOnOpen](./getcalculateonopen/) | Anger om applikationen måste utföra en fullständig beräkning när arbetsboken öppnas. |
| [SetCalculateOnOpen](./setcalculateonopen/) | Anger om applikationen måste utföra en fullständig beräkning när arbetsboken öppnas. |
| [GetCalculateOnSave](./getcalculateonsave/) | Anger om arbetsboken ska omberäknas innan dokumentet sparas, när den är i manuellt beräkningsläge. |
| [SetCalculateOnSave](./setcalculateonsave/) | Anger om arbetsboken ska omberäknas innan dokumentet sparas, när den är i manuellt beräkningsläge. |
| [GetForceFullCalculation](./getforcefullcalculation/) | Anger om den beräknar alla formler varje gång en beräkning utlöses. |
| [SetForceFullCalculation](./setforcefullcalculation/) | Anger om den beräknar alla formler varje gång en beräkning utlöses. |
| [GetCalculationMode](./getcalculationmode/) | Hämtar eller anger läget för arbetsboksberäkning i MS Excel. |
| [SetCalculationMode](./setcalculationmode/) | Hämtar eller anger läget för arbetsboksberäkning i MS Excel. |
| [GetCalculationId](./getcalculationid/) | Specificerar versionen av beräkningsmotorn som används för att beräkna värden i arbetsboken. |
| [SetCalculationId](./setcalculationid/) | Specificerar versionen av beräkningsmotorn som används för att beräkna värden i arbetsboken. |
| [GetEnableIterativeCalculation](./getenableiterativecalculation/) | Anger om iterativ beräkning ska aktiveras för att lösa cirkulära referenser. |
| [SetEnableIterativeCalculation](./setenableiterativecalculation/) | Anger om iterativ beräkning ska aktiveras för att lösa cirkulära referenser. |
| [GetMaxIteration](./getmaxiteration/) | Det maximala antalet iterationer för att lösa en cirkulär referens. |
| [SetMaxIteration](./setmaxiteration/) | Det maximala antalet iterationer för att lösa en cirkulär referens. |
| [GetMaxChange](./getmaxchange/) | Den maximala förändringen för att lösa en cirkulär referens. |
| [SetMaxChange](./setmaxchange/) | Den maximala förändringen för att lösa en cirkulär referens. |
| [GetPrecisionAsDisplayed](./getprecisionasdisplayed/) | Anger om precisionen för beräknade resultat ska sättas som de visas under beräkning av formler. |
| [SetPrecisionAsDisplayed](./setprecisionasdisplayed/) | Anger om precisionen för beräknade resultat ska sättas som de visas under beräkning av formler. |
| [GetEnableCalculationChain](./getenablecalculationchain/) | Anger om beräkningskedja för formler ska aktiveras. Standard är falskt. |
| [SetEnableCalculationChain](./setenablecalculationchain/) | Anger om beräkningskedja för formler ska aktiveras. Standard är falskt. |
| [GetPreservePaddingSpaces](./getpreservepaddingspaces/) | Anger om de mellanslag och radbrytningar som är insatta mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt. |
| [SetPreservePaddingSpaces](./setpreservepaddingspaces/) | Anger om de mellanslag och radbrytningar som är insatta mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt. |
