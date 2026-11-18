---
title: "VbaProject‑klass"
linktitle: "VbaProject"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "VbaProject‑klass. Inkapslar objektet som representerar vbaproject i Go."
type: docs
weight: 200
url: /sv/go-cpp/vbaproject/
---

## VbaProject class

Representerar VBA-projektet.

```go

type VbaProject struct  {
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
| [Sign](./sign/) | Signera detta VBA‑projekt med en DigitalSignature |
| [IsValidSigned](./isvalidsigned/) | Anger om signaturen för VBA‑projektet är giltig eller inte. |
| [GetCertRawData](./getcertrawdata/) | Hämtar certifikatets rådata om detta VBA‑projekt är signerat. |
| [GetEncoding](./getencoding/) | Hämtar och anger kodningen för VBA‑projektet. |
| [SetEncoding](./setencoding/) | Hämtar och anger kodningen för VBA‑projektet. |
| [GetName](./getname/) | Hämtar och anger namnet på VBA‑projektet. |
| [SetName](./setname/) | Hämtar och anger namnet på VBA‑projektet. |
| [IsSigned](./issigned/) | Anger om VBA‑kod är signerad eller inte. |
| [Protect](./protect/) | Skyddar eller avskyddar detta VBA‑projekt. |
| [IsProtected](./isprotected/) | Anger om detta VBA‑projekt är skyddat. |
| [IsLockedForView](./islockedforview/) | Anger om detta VBA‑projekt är låst för visning. Om sant, kan koden inte vara synlig. |
| [Copy](./copy/) | Kopiera VBA-projekt från en annan fil. |
| [GetModules](./getmodules/) | Hämtar alla VbaModule-objekt. |
| [GetReferences](./getreferences/) | Hämtar alla referenser till VBA-projektet. |
| [ValidatePassword](./validatepassword/) | Validerar skyddslösenordet. |
