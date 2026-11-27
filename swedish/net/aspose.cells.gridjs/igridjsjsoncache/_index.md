---
title: "Gränssnitt IGridJsJsonCache"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridJs.IGridJsJsonCache-gränssnitt. JSON-cachegränssnitt som kunder implementerar med specifika lagrings- och ogiltigförklaringsstrategier"
type: docs
url: /sv/net/aspose.cells.gridjs/igridjsjsoncache/
---
## IGridJsJsonCache interface

JSON-cachegränssnitt – kunder implementerar specifika lagrings- och ogiltigförklaringsstrategier

```csharp
public interface IGridJsJsonCache
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ClearAll](../../aspose.cells.gridjs/igridjsjsoncache/clearall/)() | Rensa alla cachar |
| [GetCacheKey](../../aspose.cells.gridjs/igridjsjsoncache/getcachekey/)(string, string) | Generera en cache-nyckel. Kunder kan besluta om uid ska inkluderas baserat på affärskrav. - Om endast filnamnet är viktigt: ignorera uid och använd bara fileName (rekommenderas, möjliggör delning av cache över samma fil). - Om det krävs att särskilja filer med samma namn: använd uid (strikt läge). |
| [Invalidate](../../aspose.cells.gridjs/igridjsjsoncache/invalidate/)(string) | Ogiltigförklara den angivna cacheposten. |
| [InvalidateAllForUid](../../aspose.cells.gridjs/igridjsjsoncache/invalidateallforuid/)(string) | Ogiltigförklara alla cacheposter som innehåller den angivna uid. Detta är användbart när du inte vet det exakta fileName som används för cachning. |
| [SetJson](../../aspose.cells.gridjs/igridjsjsoncache/setjson/)(string, string) | Skriv JSON till cache. |
| [TryGetJson](../../aspose.cells.gridjs/igridjsjsoncache/trygetjson/)(string) | Försök att hämta JSON från cache. |

### Se även

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


