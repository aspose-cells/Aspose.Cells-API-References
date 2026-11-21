---
title: "CellEventStringHandler"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hücre olaylarını ele almayı amaçlayan arayüzü temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/celleventstringhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventStringHandler extends Serializable
```

Hücre olaylarını ele almayı amaçlayan arayüzü temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | İlgili Cell Event'i ele al. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract String handleCellEvent(Object sender, CellEventArgs e)
```


İlgili Cell Event'i ele al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sender | java.lang.Object | Olayın kaynak ızgarası. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | Olay argümanı. e.Cell, olayı tetikleyen hücredir. e.Argument, olayın argümanını içerir. |

**Returns:**
java.lang.String - string değeri
