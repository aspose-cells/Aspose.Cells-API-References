---
title: "CellErrorHandler"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hücre hata olaylarını ele almayı amaçlayan arayüzü temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/cellerrorhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellErrorHandler extends Serializable
```

Hücre hata olaylarını ele almayı amaçlayan arayüzü temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-) | İlgili Cell Event'i ele al. |
### handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-}
```
public abstract void handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)
```


İlgili Cell Event'i ele al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sender | java.lang.Object | Olayın kaynağı. |
| ex | [GridCellException](../../com.aspose.gridweb/gridcellexception) | Hücre işlem hatası. |
| query | [OnErrorActionQuery](../../com.aspose.gridweb/onerroractionquery) | onerror eylem türü bilgisi alınabilir. |

