---
title: "LowCodePdfSaveOptions-klass"
linktitle: "LowCodePdfSaveOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "LowCodePdfSaveOptions-klass. Inkapslar objektet som representerar lowcodepdfsaveoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/lowcodepdfsaveoptions/
---

## LowCodePdfSaveOptions class

Alternativ för att spara pdf på ett lågkodssätt.

```go

type LowCodePdfSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewLowCodePdfSaveOptions](./newlowcodepdfsaveoptions/) | Standardkonstruktor. |
| [NewLowCodePdfSaveOptions_LowCodeSaveOptions](./newlowcodepdfsaveoptions_lowcodesaveoptions/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetSaveFormat](./getsaveformat/) | Sparformatet för utdata. Vid konvertering till pdf kan det endast vara SaveFormat.Pdf. |
| [SetSaveFormat](./setsaveformat/) | Sparformatet för utdata. Vid konvertering till pdf kan det endast vara SaveFormat.Pdf. |
| [GetPdfOptions](./getpdfoptions/) | Alternativen för att spara Pdf-fil. |
| [SetPdfOptions](./setpdfoptions/) | Alternativen för att spara Pdf-fil. |
| [GetOutputFile](./getoutputfile/) | Hämtar och anger filen (med sökväg om behövs) för att spara de genererade data. När egenskapen sätts till ett värde annat än null eller en tom sträng, kommer OutputStream att ignoreras. |
| [SetOutputFile](./setoutputfile/) | Hämtar och anger filen (med sökväg om behövs) för att spara de genererade data. När egenskapen sätts till ett värde annat än null eller en tom sträng, kommer OutputStream att ignoreras. |
| [GetOutputStream](./getoutputstream/) | Hämtar och anger strömmen för att skriva de genererade data till. När egenskapen sätts till ett värde annat än null, kommer OutputFile att ignoreras. |
| [SetOutputStream](./setoutputstream/) | Hämtar och anger strömmen för att skriva de genererade data till. När egenskapen sätts till ett värde annat än null, kommer OutputFile att ignoreras. |
