---
title: "VbaProjectReferenceCollection-klass"
linktitle: "VbaProjectReferenceCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "VbaProjectReferenceCollection-klass. Inkapslar objektet som representerar vbaprojectreferencecollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/vbaprojectreferencecollection/
---

## VbaProjectReferenceCollection class

Representerar alla referenser till VBA-projektet.

```go

type VbaProjectReferenceCollection struct  {
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
| [Get](./get/) | Hämta referensen i listan efter index. |
| [AddRegisteredReference](./addregisteredreference/) | Lägg till en referens till ett Automation-typbibliotek. |
| [AddControlReferernce](./addcontrolreferernce/) | Lägg till en referens till ett twiddled-typbibliotek och dess utökade typbibliotek. |
| [AddProjectReferernce](./addprojectreferernce/) | Lägger till en referens till ett externt VBA-projekt. |
| [Copy](./copy/) | Kopierar referenser från ett annat VBA-projekt. |
| [GetCount](./getcount/) | Hämtar antalet element som finns i instansen. |
