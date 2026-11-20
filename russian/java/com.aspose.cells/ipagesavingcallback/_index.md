---
title: "IPageSavingCallback"
second_title: "Справочник API Aspose.Cells for Java"
description: "Контролировать/Указывать прогресс процесса сохранения страниц."
type: docs
url: /ru/java/com.aspose.cells/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Контролировать/Указывать прогресс процесса сохранения страниц.
## Методы

| Метод | Описание |
| --- | --- |
| [pageEndSaving(PageEndSavingArgs args)](#pageEndSaving-com.aspose.cells.PageEndSavingArgs-) | Контролировать/Указывать, что страница завершена для вывода. |
| [pageStartSaving(PageStartSavingArgs args)](#pageStartSaving-com.aspose.cells.PageStartSavingArgs-) | Контролировать/Указывать, что страница начинается для вывода. |
### pageEndSaving(PageEndSavingArgs args) {#pageEndSaving-com.aspose.cells.PageEndSavingArgs-}
```
public abstract void pageEndSaving(PageEndSavingArgs args)
```


Контролировать/Указывать, что страница завершена для вывода.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| args | [PageEndSavingArgs](../../com.aspose.cells/pageendsavingargs) | Информация о завершении процесса сохранения страницы. |

### pageStartSaving(PageStartSavingArgs args) {#pageStartSaving-com.aspose.cells.PageStartSavingArgs-}
```
public abstract void pageStartSaving(PageStartSavingArgs args)
```


Контролировать/Указывать, что страница начинается для вывода.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| args | [PageStartSavingArgs](../../com.aspose.cells/pagestartsavingargs) | Информация о начале процесса сохранения страницы. |

