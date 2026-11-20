---
title: "IPageSavingCallback"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Controlla/Indica l'avanzamento del processo di salvataggio della pagina."
type: docs
url: /it/java/com.aspose.cells/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Controlla/Indica l'avanzamento del processo di salvataggio della pagina.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [pageEndSaving(PageEndSavingArgs args)](#pageEndSaving-com.aspose.cells.PageEndSavingArgs-) | Controlla/Indica la fine di una pagina da esportare. |
| [pageStartSaving(PageStartSavingArgs args)](#pageStartSaving-com.aspose.cells.PageStartSavingArgs-) | Controlla/Indica l'inizio di una pagina da esportare. |
### pageEndSaving(PageEndSavingArgs args) {#pageEndSaving-com.aspose.cells.PageEndSavingArgs-}
```
public abstract void pageEndSaving(PageEndSavingArgs args)
```


Controlla/Indica la fine di una pagina da esportare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| args | [PageEndSavingArgs](../../com.aspose.cells/pageendsavingargs) | Informazioni per una pagina al termine del processo di salvataggio. |

### pageStartSaving(PageStartSavingArgs args) {#pageStartSaving-com.aspose.cells.PageStartSavingArgs-}
```
public abstract void pageStartSaving(PageStartSavingArgs args)
```


Controlla/Indica l'inizio di una pagina da esportare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| args | [PageStartSavingArgs](../../com.aspose.cells/pagestartsavingargs) | Informazioni per una pagina all'inizio del processo di salvataggio. |

