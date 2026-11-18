---
title: "FileFormatInfo Klass"
linktitle: "FileFormatInfo"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "FileFormatInfo-klass. Inkapslar objektet som representerar fileformatinfo i Go."
type: docs
weight: 200
url: /sv/go-cpp/fileformatinfo/
---

## FileFormatInfo class

Innehåller data som returneras av <see cref="FileFormatUtil"/>‑metoder för filformatdetektering.

```go

type FileFormatInfo struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewFileFormatInfo](./newfileformatinfo/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [IsProtectedByRMS](./isprotectedbyrms/) | Anger om filen är skyddad av Microsoft Rights Management Server. |
| [IsEncrypted](./isencrypted/) | Returnerar true om dokumentet är krypterat och kräver ett lösenord för att öppnas. |
| [GetFileFormatType](./getfileformattype/) | Hämtar det upptäckta filformatet. |
| [GetLoadFormat](./getloadformat/) | Hämtar det upptäckta laddningsformatet |
