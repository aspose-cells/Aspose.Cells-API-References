---
title: "MergedCellsShrinkType-enum"
linktitle: "MergedCellsShrinkType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "MergedCellsShrinkType-enum. Inkapslar objektet som representerar mergedcellsshrinktype i Go."
type: docs
weight: 200
url: /sv/go-cpp/mergedcellsshrinktype/
---

## MergedCellsShrinkType Enum

Representerar strategin för att krympa sammanslagna celler för operationer såsom att ta bort tomma rader/kolumner.

```go

type MergedCellsShrinkType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [None](./none/) | Lämnar de sammanslagna cellerna som de är utan någon ändring. |
| [ShrinkToFit](./shrinktofit/) | Krymper det sammanslagna området om det behövs, genom att ta bort rader från botten eller kolumner från höger, samtidigt som allt innehåll förblir synligt. |
| [KeepHeaderOnly](./keepheaderonly/) | Behåller endast rubrikraderna/kolumnerna i det sammanslagna området när den övre vänstra cellen i det sammanslagna området inte är tom. |
