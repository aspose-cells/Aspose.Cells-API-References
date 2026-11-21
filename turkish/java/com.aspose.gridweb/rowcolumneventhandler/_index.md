---
title: "RowColumnEventHandler"
second_title: "Aspose.Cells for Java API Referansı"
description: "Satır/sütun olaylarını ele almayı amaçlayan arayüzü temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/rowcolumneventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface RowColumnEventHandler extends Serializable
```

Satır/sütun olaylarını ele almayı amaçlayan arayüzü temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [handleCellEvent(Object sender, RowColumnEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-) | İlgili Cell Event'i ele al. |
### handleCellEvent(Object sender, RowColumnEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-}
```
public abstract void handleCellEvent(Object sender, RowColumnEventArgs e)
```


İlgili Cell Event'i ele al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sender | java.lang.Object | Olayın kaynağı. |
| e | [RowColumnEventArgs](../../com.aspose.gridweb/rowcolumneventargs) | Olay argümanı. RowDeleting veya ColumnDeleting olay işleyicilerinde silme işlemini iptal etmek istiyorsanız e.RejectOperation() çağırın. |

