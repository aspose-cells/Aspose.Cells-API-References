---
title: "IPageSavingCallback"
second_title: "Aspose.Cells för Java API-referens"
description: "Styr/indikera framsteg för sid sparningsprocessen."
type: docs
url: /sv/java/com.aspose.cells/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Styr/indikera framsteg för sid sparningsprocessen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [pageEndSaving(PageEndSavingArgs args)](#pageEndSaving-com.aspose.cells.PageEndSavingArgs-) | Kontroll/Indikera att en sida avslutas för utskrift. |
| [pageStartSaving(PageStartSavingArgs args)](#pageStartSaving-com.aspose.cells.PageStartSavingArgs-) | Kontroll/Indikera att en sida påbörjas för utskrift. |
### pageEndSaving(PageEndSavingArgs args) {#pageEndSaving-com.aspose.cells.PageEndSavingArgs-}
```
public abstract void pageEndSaving(PageEndSavingArgs args)
```


Kontroll/Indikera att en sida avslutas för utskrift.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| args | [PageEndSavingArgs](../../com.aspose.cells/pageendsavingargs) | Information för en sida avslutar sparprocessen. |

### pageStartSaving(PageStartSavingArgs args) {#pageStartSaving-com.aspose.cells.PageStartSavingArgs-}
```
public abstract void pageStartSaving(PageStartSavingArgs args)
```


Kontroll/Indikera att en sida påbörjas för utskrift.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| args | [PageStartSavingArgs](../../com.aspose.cells/pagestartsavingargs) | Information för en sida startar sparprocessen. |

