---
title: "IGridJsJsonCache"
second_title: "Aspose.Cells for Java API-Referenz"
description: "JSON‑Cache‑Schnittstelle – Kunden implementieren spezifische Speicher‑ und Ungültigkeitsstrategien"
type: docs
url: /de/java/com.aspose.gridjs/igridjsjsoncache/
---
```
public interface IGridJsJsonCache
```

JSON‑Cache‑Schnittstelle – Kunden implementieren spezifische Speicher‑ und Ungültigkeitsstrategien
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [clearAll()](#clearAll--) | Alle Caches leeren |
| [getCacheKey(String uid, String fileName)](#getCacheKey-java.lang.String-java.lang.String-) | Erzeuge einen Cache-Schlüssel. |
| [invalidate(String cacheKey)](#invalidate-java.lang.String-) | Den angegebenen Cache-Eintrag ungültig machen. |
| [invalidateAllForUid(String uid)](#invalidateAllForUid-java.lang.String-) | Ungültig machen aller Cache-Einträge, die die angegebene UID enthalten. |
| [setJson(String cacheKey, String json)](#setJson-java.lang.String-java.lang.String-) | JSON in den Cache schreiben. |
| [tryGetJson(String cacheKey)](#tryGetJson-java.lang.String-) | Versuchen, JSON aus dem Cache abzurufen. |
### clearAll() {#clearAll--}
```
public abstract void clearAll()
```


Alle Caches leeren

### getCacheKey(String uid, String fileName) {#getCacheKey-java.lang.String-java.lang.String-}
```
public abstract String getCacheKey(String uid, String fileName)
```


Erzeugen Sie einen Cache-Schlüssel. Kunden können basierend auf geschäftlichen Anforderungen entscheiden, ob die uid einbezogen wird. - Wenn nur der Dateiname wichtig ist: uid ignorieren und nur fileName verwenden (empfohlen, ermöglicht das Teilen des Caches für dieselbe Datei). - Wenn eine Unterscheidung von Dateien mit demselben Namen erforderlich ist: uid verwenden (strikter Modus).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Eindeutiger Bezeichner der Datei (kann pro Ladevorgang variieren) |
| fileName | java.lang.String | Ursprünglicher Dateiname |

**Returns:**
java.lang.String - Cache-Schlüssel
### invalidate(String cacheKey) {#invalidate-java.lang.String-}
```
public abstract void invalidate(String cacheKey)
```


Den angegebenen Cache-Eintrag ungültig machen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cacheKey | java.lang.String | Cache-Schlüssel |

### invalidateAllForUid(String uid) {#invalidateAllForUid-java.lang.String-}
```
public abstract void invalidateAllForUid(String uid)
```


Alle Cache-Einträge, die die angegebene uid enthalten, ungültig machen. Dies ist nützlich, wenn Sie den genauen für das Caching verwendeten fileName nicht kennen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | java.lang.String | Eindeutiger Bezeichner zum Abgleichen in Cache-Schlüsseln |

### setJson(String cacheKey, String json) {#setJson-java.lang.String-java.lang.String-}
```
public abstract void setJson(String cacheKey, String json)
```


JSON in den Cache schreiben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cacheKey | java.lang.String | Cache-Schlüssel |
| JSON | java.lang.String | JSON-Zeichenfolge |

### tryGetJson(String cacheKey) {#tryGetJson-java.lang.String-}
```
public abstract String tryGetJson(String cacheKey)
```


Versuchen, JSON aus dem Cache abzurufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cacheKey | java.lang.String | Cache-Schlüssel |

**Returns:**
java.lang.String - JSON-Zeichenfolge bei Cache-Treffer, sonst null
