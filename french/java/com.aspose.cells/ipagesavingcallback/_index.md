---
title: "IPageSavingCallback"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Contrôle/Indique la progression du processus d'enregistrement de la page."
type: docs
url: /fr/java/com.aspose.cells/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Contrôle/Indique la progression du processus d'enregistrement de la page.
## Méthodes

| Méthode | Description |
| --- | --- |
| [pageEndSaving(PageEndSavingArgs args)](#pageEndSaving-com.aspose.cells.PageEndSavingArgs-) | Contrôle/Indique la fin d'une page à exporter. |
| [pageStartSaving(PageStartSavingArgs args)](#pageStartSaving-com.aspose.cells.PageStartSavingArgs-) | Contrôle/Indique le début d'une page à exporter. |
### pageEndSaving(PageEndSavingArgs args) {#pageEndSaving-com.aspose.cells.PageEndSavingArgs-}
```
public abstract void pageEndSaving(PageEndSavingArgs args)
```


Contrôle/Indique la fin d'une page à exporter.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| args | [PageEndSavingArgs](../../com.aspose.cells/pageendsavingargs) | Informations concernant une page terminent le processus d'enregistrement. |

### pageStartSaving(PageStartSavingArgs args) {#pageStartSaving-com.aspose.cells.PageStartSavingArgs-}
```
public abstract void pageStartSaving(PageStartSavingArgs args)
```


Contrôle/Indique le début d'une page à exporter.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| args | [PageStartSavingArgs](../../com.aspose.cells/pagestartsavingargs) | Informations concernant le démarrage du processus d'enregistrement d'une page. |

