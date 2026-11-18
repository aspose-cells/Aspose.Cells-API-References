---
title: "LowCodeSaveOptions-klass"
linktitle: "LowCodeSaveOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "LowCodeSaveOptions-klass. Inkapslar objektet som representerar lowcodesaveoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/lowcodesaveoptions/
---

## LowCodeSaveOptions class

Alternativ för att spara genererade resultat på ett lågkodssätt.

```go

type LowCodeSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewLowCodeSaveOptions](./newlowcodesaveoptions/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetOutputFile](./getoutputfile/) | Hämtar och anger filen (med sökväg om behövs) för att spara de genererade data. När egenskapen sätts till ett värde annat än null eller en tom sträng, kommer OutputStream att ignoreras. |
| [SetOutputFile](./setoutputfile/) | Hämtar och anger filen (med sökväg om behövs) för att spara de genererade data. När egenskapen sätts till ett värde annat än null eller en tom sträng, kommer OutputStream att ignoreras. |
| [GetOutputStream](./getoutputstream/) | Hämtar och anger strömmen för att skriva de genererade data till. När egenskapen sätts till ett värde annat än null, kommer OutputFile att ignoreras. |
| [SetOutputStream](./setoutputstream/) | Hämtar och anger strömmen för att skriva de genererade data till. När egenskapen sätts till ett värde annat än null, kommer OutputFile att ignoreras. |
| [GetSaveFormat](./getsaveformat/) | Hämtar och anger sparaformatet för utdata.Generellt, för specifika processer i lågkodssätt, är endast vissa specifika format tillåtna.Vänligen ange rätt format för motsvarande process, annars kan oväntade resultat eller till och med undantag uppstå. |
| [SetSaveFormat](./setsaveformat/) | Hämtar och anger sparaformatet för utdata.Generellt, för specifika processer i lågkodssätt, är endast vissa specifika format tillåtna.Vänligen ange rätt format för motsvarande process, annars kan oväntade resultat eller till och med undantag uppstå. |
