---
title: "IGridJsJsonCache.GetCacheKey"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IGridJsJsonCache-Methode. Erzeugt einen Cache-Schlüssel. Kunden können entscheiden, ob die UID basierend auf geschäftlichen Anforderungen einbezogen wird. Wenn nur der Dateiname wichtig ist, ignorieren Sie die UID und verwenden ausschließlich fileName – empfohlen, um den Cache über dieselbe Datei zu teilen. Wenn das Unterscheiden von Dateien mit demselben Namen erforderlich ist, verwenden Sie den strikten UID‑Modus."
type: docs
url: /de/net/aspose.cells.gridjs/igridjsjsoncache/getcachekey/
---
## IGridJsJsonCache.GetCacheKey method

Erzeugt einen Cache‑Schlüssel. Kunden können entscheiden, ob die UID basierend auf geschäftlichen Anforderungen einbezogen wird. - Wenn nur der Dateiname wichtig ist: UID ignorieren und nur fileName verwenden (empfohlen, ermöglicht das Teilen des Caches über dieselbe Datei). - Wenn die Unterscheidung von Dateien mit gleichem Namen erforderlich ist: UID verwenden (strikter Modus).

```csharp
public string GetCacheKey(string uid, string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | String | Eindeutiger Bezeichner der Datei (kann pro Ladevorgang variieren) |
| fileName | String | Ursprünglicher Dateiname |

### Rückgabewert

Cache-Schlüssel

### Siehe auch

* interface [IGridJsJsonCache](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


