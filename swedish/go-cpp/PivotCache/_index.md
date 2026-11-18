---
title: "PivotCache klass"
linktitle: "PivotCache"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PivotCache klass. Inkapslar objektet som representerar pivotcache i Go."
type: docs
weight: 200
url: /sv/go-cpp/pivotcache/
---

## PivotCache class

Representerar minnescachen för vissa PivotTable-rapporter.

```go

type PivotCache struct  {
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
| [GetMissingItemsLimit](./getmissingitemslimit/) | Hämtar och anger antalet oanvända objekt som tillåts innan oanvända objekt kastas. Detta värde MÅSTE vara större än -2 och mindre än 1048577. PivotCacheMissingItemsLimitConst; |
| [SetMissingItemsLimit](./setmissingitemslimit/) | Hämtar och anger antalet oanvända objekt som tillåts innan oanvända objekt kastas. Detta värde MÅSTE vara större än -2 och mindre än 1048577. PivotCacheMissingItemsLimitConst; |
| [Refresh_PivotTableRefreshOption](./refresh_pivottablerefreshoption/) | Uppdaterar data från datakällan och beräknar data för vyn av alla pivottabeller vars datakälla är denna pivotcache. |
| [Refresh](./refresh/) | Uppdaterar data från datakällan och beräknar data för vyn av alla pivottabeller vars datakälla är denna pivotcache. |
| [GetPivotTables](./getpivottables/) | Hämtar alla pivottabeller med denna pivotcache. |
| [Dispose](./dispose/) | Frigör alla resurser. |
| [GetSourceType](./getsourcetype/) | Hämtar PivotTableSourceType. |
