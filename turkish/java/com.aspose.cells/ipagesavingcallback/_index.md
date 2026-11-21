---
title: "IPageSavingCallback"
second_title: "Aspose.Cells for Java API Referansı"
description: "Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder."
type: docs
url: /tr/java/com.aspose.cells/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Sayfa kaydetme sürecinin ilerlemesini kontrol/indike eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [pageEndSaving(PageEndSavingArgs args)](#pageEndSaving-com.aspose.cells.PageEndSavingArgs-) | Kontrol/Çıktı olarak bir sayfanın sonlandığını belirtir. |
| [pageStartSaving(PageStartSavingArgs args)](#pageStartSaving-com.aspose.cells.PageStartSavingArgs-) | Kontrol/Çıktı olarak bir sayfanın başladığını belirtir. |
### pageEndSaving(PageEndSavingArgs args) {#pageEndSaving-com.aspose.cells.PageEndSavingArgs-}
```
public abstract void pageEndSaving(PageEndSavingArgs args)
```


Kontrol/Çıktı olarak bir sayfanın sonlandığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| args | [PageEndSavingArgs](../../com.aspose.cells/pageendsavingargs) | Bir sayfanın kaydetme işlemini sonlandırma bilgisi. |

### pageStartSaving(PageStartSavingArgs args) {#pageStartSaving-com.aspose.cells.PageStartSavingArgs-}
```
public abstract void pageStartSaving(PageStartSavingArgs args)
```


Kontrol/Çıktı olarak bir sayfanın başladığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| args | [PageStartSavingArgs](../../com.aspose.cells/pagestartsavingargs) | Bir sayfanın kaydetme işlemini başlatma bilgisi. |

