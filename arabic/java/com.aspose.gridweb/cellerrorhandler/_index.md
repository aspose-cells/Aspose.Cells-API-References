---
title: "CellErrorHandler"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الواجهة التي تهدف إلى معالجة أحداث خطأ الخلية."
type: docs
url: /ar/java/com.aspose.gridweb/cellerrorhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellErrorHandler extends Serializable
```

يمثل الواجهة التي تهدف إلى معالجة أحداث خطأ الخلية.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-) | معالجة حدث الخلية المرتبط. |
### handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-}
```
public abstract void handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)
```


معالجة حدث الخلية المرتبط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| المرسل | java.lang.Object | مصدر الحدث. |
| ex | [GridCellException](../../com.aspose.gridweb/gridcellexception) | خطأ عملية الخلية. |
| query | [OnErrorActionQuery](../../com.aspose.gridweb/onerroractionquery) | يمكن الحصول على معلومات نوع إجراء onerror. |

