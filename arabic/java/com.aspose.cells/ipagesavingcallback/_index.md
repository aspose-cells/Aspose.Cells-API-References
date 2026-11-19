---
title: "IPageSavingCallback"
second_title: "Aspose.Cells for Java API Reference"
description: "التحكم/الإشارة إلى تقدم عملية حفظ الصفحة."
type: docs
url: /ar/java/com.aspose.cells/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

التحكم/الإشارة إلى تقدم عملية حفظ الصفحة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [pageEndSaving(PageEndSavingArgs args)](#pageEndSaving-com.aspose.cells.PageEndSavingArgs-) | تحكم/أشر إلى انتهاء صفحة ليتم إخراجها. |
| [pageStartSaving(PageStartSavingArgs args)](#pageStartSaving-com.aspose.cells.PageStartSavingArgs-) | تحكم/أشر إلى بدء صفحة ليتم إخراجها. |
### pageEndSaving(PageEndSavingArgs args) {#pageEndSaving-com.aspose.cells.PageEndSavingArgs-}
```
public abstract void pageEndSaving(PageEndSavingArgs args)
```


تحكم/أشر إلى انتهاء صفحة ليتم إخراجها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| args | [PageEndSavingArgs](../../com.aspose.cells/pageendsavingargs) | معلومات لصفحة تنتهي عملية الحفظ. |

### pageStartSaving(PageStartSavingArgs args) {#pageStartSaving-com.aspose.cells.PageStartSavingArgs-}
```
public abstract void pageStartSaving(PageStartSavingArgs args)
```


تحكم/أشر إلى بدء صفحة ليتم إخراجها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| args | [PageStartSavingArgs](../../com.aspose.cells/pagestartsavingargs) | معلومات لصفحة تبدأ عملية الحفظ. |

