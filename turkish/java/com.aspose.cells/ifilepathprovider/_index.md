---
title: "IFilePathProvider"
second_title: "Aspose.Cells for Java API Referansı"
description: "Dışa aktarılan dosya yolu sağlayıcısını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/ifilepathprovider/
---
```
public interface IFilePathProvider
```

Dışa aktarılan dosya yolu sağlayıcısını temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getFullName(String sheetName)](#getFullName-java.lang.String-) | Worksheet'i ayrı ayrı HTML'ye dışa aktarırken, dosyanın tam yolunu Worksheet adıyla alır. |
### getFullName(String sheetName) {#getFullName-java.lang.String-}
```
public abstract String getFullName(String sheetName)
```


Worksheet'i ayrı ayrı HTML'ye dışa aktarırken, dosyanın tam yolunu Worksheet adıyla alır. Böylece Worksheet'ler arasındaki referanslar doğru şekilde dışa aktarılabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | java.lang.String | Çalışma sayfası adı |

**Returns:**
java.lang.String - dosyanın tam yolu
