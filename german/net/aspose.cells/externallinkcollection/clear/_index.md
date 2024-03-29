---
title: Clear
second_title: Aspose.Cells für .NET-API-Referenz
description: Entfernt alle externen Links.
type: docs
weight: 40
url: /de/net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Entfernt alle externen Links.

```csharp
public void Clear()
```

### Bemerkungen

Beim Entfernen externer Links werden auch alle darauf verweisenden Formeln entfernt, weil die Verweise ungültig werden.

### Siehe auch

* class [ExternalLinkCollection](../../externallinkcollection)
* namensraum [Aspose.Cells](../../externallinkcollection)
* Montage [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Entfernt alle externen Links.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| updateReferencesAsLocal | Boolean | Ob alle Verweise auf externe Links als Verweise auf die aktuelle Arbeitsmappe selbst aktualisiert werden. |

### Bemerkungen

Wenn Verweise aktualisiert werden müssen, werden Verweise auf externe Links in Formeln in die aktuelle Arbeitsmappe geändert. Beispielsweise lautet die ursprüngliche Formel einer Zelle "='externalsource.xlam'!customfunction()", nach dem Entfernen externer Links, die Formel wird zu „=customfunction()“. Wenn Verweise nicht aktualisiert werden müssen, werden alle Formeln mit Verweisen auf externe Links ebenfalls entfernt, da diese Verweise ungültig werden.

### Siehe auch

* class [ExternalLinkCollection](../../externallinkcollection)
* namensraum [Aspose.Cells](../../externallinkcollection)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
