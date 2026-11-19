---
title: "IPageSavingCallback"
second_title: "Aspose.Cells for Java API 参考"
description: "控制/指示页面保存过程的进度。"
type: docs
url: /zh/java/com.aspose.cells/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

控制/指示页面保存过程的进度。
## 方法

| 方法 | 描述 |
| --- | --- |
| [pageEndSaving(PageEndSavingArgs args)](#pageEndSaving-com.aspose.cells.PageEndSavingArgs-) | 控制/指示页面结束以输出。 |
| [pageStartSaving(PageStartSavingArgs args)](#pageStartSaving-com.aspose.cells.PageStartSavingArgs-) | 控制/指示页面开始以输出。 |
### pageEndSaving(PageEndSavingArgs args) {#pageEndSaving-com.aspose.cells.PageEndSavingArgs-}
```
public abstract void pageEndSaving(PageEndSavingArgs args)
```


控制/指示页面结束以输出。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| args | [PageEndSavingArgs](../../com.aspose.cells/pageendsavingargs) | 页面结束保存过程的信息。 |

### pageStartSaving(PageStartSavingArgs args) {#pageStartSaving-com.aspose.cells.PageStartSavingArgs-}
```
public abstract void pageStartSaving(PageStartSavingArgs args)
```


控制/指示页面开始以输出。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| args | [PageStartSavingArgs](../../com.aspose.cells/pagestartsavingargs) | 页面开始保存过程的信息。 |

