---
title: "IPageSavingCallback"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Controla/Indica el progreso del proceso de guardado de página."
type: docs
url: /es/java/com.aspose.cells/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Controla/Indica el progreso del proceso de guardado de página.
## Métodos

| Método | Descripción |
| --- | --- |
| [pageEndSaving(PageEndSavingArgs args)](#pageEndSaving-com.aspose.cells.PageEndSavingArgs-) | Control/Indicar que una página termina de ser exportada. |
| [pageStartSaving(PageStartSavingArgs args)](#pageStartSaving-com.aspose.cells.PageStartSavingArgs-) | Control/Indicar que una página comienza a ser exportada. |
### pageEndSaving(PageEndSavingArgs args) {#pageEndSaving-com.aspose.cells.PageEndSavingArgs-}
```
public abstract void pageEndSaving(PageEndSavingArgs args)
```


Control/Indicar que una página termina de ser exportada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| args | [PageEndSavingArgs](../../com.aspose.cells/pageendsavingargs) | Información para una página al finalizar el proceso de guardado. |

### pageStartSaving(PageStartSavingArgs args) {#pageStartSaving-com.aspose.cells.PageStartSavingArgs-}
```
public abstract void pageStartSaving(PageStartSavingArgs args)
```


Control/Indicar que una página comienza a ser exportada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| args | [PageStartSavingArgs](../../com.aspose.cells/pagestartsavingargs) | Información para una página al iniciar el proceso de guardado. |

