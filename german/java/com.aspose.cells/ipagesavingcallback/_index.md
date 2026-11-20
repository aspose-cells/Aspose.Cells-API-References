---
title: "IPageSavingCallback"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Steuert/Zeigt den Fortschritt des Seiten‑Speichervorgangs an."
type: docs
url: /de/java/com.aspose.cells/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Steuert/Zeigt den Fortschritt des Seiten‑Speichervorgangs an.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [pageEndSaving(PageEndSavingArgs args)](#pageEndSaving-com.aspose.cells.PageEndSavingArgs-) | Steuern/Angeben, dass eine Seite beendet wird, um ausgegeben zu werden. |
| [pageStartSaving(PageStartSavingArgs args)](#pageStartSaving-com.aspose.cells.PageStartSavingArgs-) | Steuern/Angeben, dass eine Seite beginnt, ausgegeben zu werden. |
### pageEndSaving(PageEndSavingArgs args) {#pageEndSaving-com.aspose.cells.PageEndSavingArgs-}
```
public abstract void pageEndSaving(PageEndSavingArgs args)
```


Steuern/Angeben, dass eine Seite beendet wird, um ausgegeben zu werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| args | [PageEndSavingArgs](../../com.aspose.cells/pageendsavingargs) | Informationen für das Beenden des Speichervorgangs einer Seite. |

### pageStartSaving(PageStartSavingArgs args) {#pageStartSaving-com.aspose.cells.PageStartSavingArgs-}
```
public abstract void pageStartSaving(PageStartSavingArgs args)
```


Steuern/Angeben, dass eine Seite beginnt, ausgegeben zu werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| args | [PageStartSavingArgs](../../com.aspose.cells/pagestartsavingargs) | Informationen zum Starten des Speichervorgangs einer Seite. |

