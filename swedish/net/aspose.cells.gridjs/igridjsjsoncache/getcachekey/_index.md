---
title: "IGridJsJsonCache.GetCacheKey"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IGridJsJsonCache-metod. Generera en cache-nyckel. Kunder kan besluta om uid ska inkluderas baserat på affärskrav. Om endast filnamnet är viktigt, ignorera uid och använd bara filnamnet – rekommenderas för att möjliggöra delning av cache över samma fil. Om det krävs att särskilja filer med samma namn, använd uid i strikt läge."
type: docs
url: /sv/net/aspose.cells.gridjs/igridjsjsoncache/getcachekey/
---
## IGridJsJsonCache.GetCacheKey method

Generera en cache-nyckel. Kunder kan besluta om uid ska inkluderas baserat på affärskrav. - Om endast filnamnet är viktigt: ignorera uid och använd bara fileName (rekommenderas, möjliggör delning av cache över samma fil). - Om det krävs att särskilja filer med samma namn: använd uid (strikt läge).

```csharp
public string GetCacheKey(string uid, string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | String | Unik identifierare för filen (kan variera per inläsning) |
| fileName | String | Originalt filnamn |

### Returvärde

Cache-nyckel

### Se även

* interface [IGridJsJsonCache](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


