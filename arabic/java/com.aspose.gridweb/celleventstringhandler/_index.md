---
title: "CellEventStringHandler"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الواجهة التي تهدف إلى معالجة أحداث الخلية."
type: docs
url: /ar/java/com.aspose.gridweb/celleventstringhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventStringHandler extends Serializable
```

يمثل الواجهة التي تهدف إلى معالجة أحداث الخلية.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | معالجة حدث الخلية المرتبط. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract String handleCellEvent(Object sender, CellEventArgs e)
```


معالجة حدث الخلية المرتبط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المرسل | java.lang.Object | شبكة المصدر للحدث. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | معامل الحدث. الـ e.Cell هو الخلية التي تُطلق الحدث. الـ e.Argument يحتوي على معامل الحدث. |

**Returns:**
java.lang.String - قيمة نصية
