---
title: "Klass PivotCache"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotCache-klass. Representerar minnescachen för vissa PivotTable-rapporter"
type: docs
url: /sv/net/aspose.cells.pivot/pivotcache/
---
## PivotCache class

Representerar minnescachen för vissa PivotTable-rapporter.

```csharp
public abstract class PivotCache : IDisposable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [MissingItemsLimit](../../aspose.cells.pivot/pivotcache/missingitemslimit/) { get; set; } | Hämtar och anger antalet oanvända objekt som får tillåtas innan oanvända objekt tas bort. Detta värde MÅSTE vara större än -2 och mindre än 1048577. [`PivotCacheMissingItemsLimitConst`](../pivotcachemissingitemslimitconst/); |
| abstract [SourceType](../../aspose.cells.pivot/pivotcache/sourcetype/) { get; } | Hämtar [`PivotTableSourceType`](../pivottablesourcetype/). |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| abstract [Dispose](../../aspose.cells.pivot/pivotcache/dispose/)() | Frigör alla resurser. |
| [GetPivotTables](../../aspose.cells.pivot/pivotcache/getpivottables/)() | Hämtar alla pivottabeller med denna pivot cache. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh)() | Uppdaterar data från datakällan och beräknar data för vyn av alla pivottabeller vars datakälla är denna pivot cache. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh_1)(PivotTableRefreshOption) | Uppdaterar data från datakällan och beräknar data för vyn av alla pivottabeller vars datakälla är denna pivot cache. |

### Anmärkningar

All data kommer att samlas i denna cache, och pivottabellen hämtar endast data från denna cache, utan att direkt åtkomma datakällan. Om datakällan för vissa [`PivotTable`](../pivottable/) är densamma, kommer de att använda en pivot cache.

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


