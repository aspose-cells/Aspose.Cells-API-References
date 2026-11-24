---
title: "Schnittstelle IGridJsJsonCache"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridJs.IGridJsJsonCache Schnittstelle. JSON‑Cache‑Schnittstelle, Kunden implementieren spezifische Speicher‑ und Ungültigkeitsstrategien."
type: docs
url: /de/net/aspose.cells.gridjs/igridjsjsoncache/
---
## IGridJsJsonCache interface

JSON‑Cache‑Schnittstelle – Kunden implementieren spezifische Speicher‑ und Ungültigkeitsstrategien.

```csharp
public interface IGridJsJsonCache
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ClearAll](../../aspose.cells.gridjs/igridjsjsoncache/clearall/)() | Alle Caches leeren |
| [GetCacheKey](../../aspose.cells.gridjs/igridjsjsoncache/getcachekey/)(string, string) | Erzeugt einen Cache‑Schlüssel. Kunden können entscheiden, ob die UID basierend auf geschäftlichen Anforderungen einbezogen wird. - Wenn nur der Dateiname wichtig ist: UID ignorieren und nur fileName verwenden (empfohlen, ermöglicht das Teilen des Caches über dieselbe Datei). - Wenn die Unterscheidung von Dateien mit gleichem Namen erforderlich ist: UID verwenden (strikter Modus). |
| [Invalidate](../../aspose.cells.gridjs/igridjsjsoncache/invalidate/)(string) | Ungültigmacht den angegebenen Cache‑Eintrag. |
| [InvalidateAllForUid](../../aspose.cells.gridjs/igridjsjsoncache/invalidateallforuid/)(string) | Ungültigmacht alle Cache‑Einträge, die die angegebene UID enthalten. Dies ist nützlich, wenn der genaue für das Caching verwendete fileName nicht bekannt ist. |
| [SetJson](../../aspose.cells.gridjs/igridjsjsoncache/setjson/)(string, string) | Schreibt JSON in den Cache. |
| [TryGetJson](../../aspose.cells.gridjs/igridjsjsoncache/trygetjson/)(string) | Versucht, JSON aus dem Cache abzurufen. |

### Siehe auch

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


