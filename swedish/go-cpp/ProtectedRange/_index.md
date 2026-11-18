---
title: "ProtectedRange-klass"
linktitle: "ProtectedRange"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ProtectedRange-klass. Inkapslar objektet som representerar protectedrange i Go."
type: docs
weight: 200
url: /sv/go-cpp/protectedrange/
---

## ProtectedRange class

Ett specificerat område som får redigeras när bladskyddet är AKTIVT.

```go

type ProtectedRange struct  {
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
| [GetName](./getname/) | Hämtar Range‑titeln. Detta används som en beskrivning, inte som en namngiven områdesdefinition. |
| [SetName](./setname/) | Hämtar Range‑titeln. Detta används som en beskrivning, inte som en namngiven områdesdefinition. |
| [GetCellArea](./getcellarea/) | Hämtar CellArea‑objektet som representerar cellområdet som ska skyddas. |
| [GetAreas](./getareas/) | Hämtar alla refererade områden. |
| [AddArea](./addarea/) | Lägger till ett refererat område till detta |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | Indikerar om kalkylbladet är skyddat med lösenord. |
| [GetPassword](./getpassword/) | Representerar lösenordet för att skydda området. |
| [SetPassword](./setpassword/) | Representerar lösenordet för att skydda området. |
| [GetSecurityDescriptor](./getsecuritydescriptor/) | Säkerhetsbeskrivningen definierar användarkonton som kan redigera detta område utan att ange ett lösenord för åtkomst. |
| [SetSecurityDescriptor](./setsecuritydescriptor/) | Säkerhetsbeskrivningen definierar användarkonton som kan redigera detta område utan att ange ett lösenord för åtkomst. |
