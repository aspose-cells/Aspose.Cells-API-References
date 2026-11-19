---
title: "RowColumnEventHandler"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الواجهة التي تهدف إلى معالجة أحداث الصف/العمود."
type: docs
url: /ar/java/com.aspose.gridweb/rowcolumneventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface RowColumnEventHandler extends Serializable
```

يمثل الواجهة التي تهدف إلى معالجة أحداث الصف/العمود.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [handleCellEvent(Object sender, RowColumnEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-) | معالجة حدث الخلية المرتبط. |
### handleCellEvent(Object sender, RowColumnEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-}
```
public abstract void handleCellEvent(Object sender, RowColumnEventArgs e)
```


معالجة حدث الخلية المرتبط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المرسل | java.lang.Object | مصدر الحدث. |
| e | [RowColumnEventArgs](../../com.aspose.gridweb/rowcolumneventargs) | معامل الحدث. استدعِ e.RejectOperation() إذا كنت تريد إلغاء عملية الحذف في معالجات الأحداث RowDeleting أو ColumnDeleting. |

