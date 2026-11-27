---
title: "Enum GridRenameStrategy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridDesktop.Data.GridRenameStrategy enum. Strategialternativ för dubblettnamn på kolumner"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridrenamestrategy/
---
## GridRenameStrategy enumeration

Strategialternativ för dubblettnamn på kolumner.

```csharp
public enum GridRenameStrategy
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Exception | `0` | Kastar undantag. |
| Digit | `1` | Namngiven med siffra. Duplicerade namn blir ...1, ...2 osv. |
| Letter | `2` | Namngiven med bokstav.. Duplicerade namn blir ...A, ...B osv. |

### Anmärkningar

När data med rubriker bearbetas kräver vissa scenarier att rubrikerna inte dupliceras för någon kolumn. Till exempel, när data exporteras till en datatabell och rubriken måste användas som datatabellens kolumnnamn, är duplicerade rubrikvärden ogiltiga. I sådana situationer kan användaren bestämma hur de ska hanteras genom att ange denna strategi.

### Se även

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


