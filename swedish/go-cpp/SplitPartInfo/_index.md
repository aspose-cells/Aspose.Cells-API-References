---
title: "SplitPartInfo-klass"
linktitle: "SplitPartInfo"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "SplitPartInfo-klass. Inkapslar objektet som representerar splitpartinfo i Go."
type: docs
weight: 200
url: /sv/go-cpp/splitpartinfo/
---

## SplitPartInfo class

Representerar informationen för en in-/utdata för flera in-/utdata, såsom aktuell sida som ska renderas när kalkylblad konverteras till bild.

```go

type SplitPartInfo struct  {
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
| [GetPartIndex](./getpartindex/) | Index för aktuell del i sekvensen (0-baserad). -1 betyder att det inte finns flera delar så resultatet är enstaka. |
| [GetSheetIndex](./getsheetindex/) | Index för bladet där den aktuella delen finns. -1 indikerar att det bara finns ett blad. |
| [GetSheetName](./getsheetname/) | Namn på bladet där den aktuella delen finns. |
