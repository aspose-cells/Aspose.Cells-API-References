---
title: "SpreadsheetSplitter"
second_title: "Aspose.Cells for Java API Referansı"
description: "Elektronik tablo dosyasını birden fazla parçaya ayırır."
type: docs
url: /tr/java/com.aspose.cells/spreadsheetsplitter/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetSplitter
```

Elektronik tablo dosyasını birden fazla parçaya ayırır.

**Example**

```
         SpreadsheetSplitter.process("template.xlsx", "split.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeSplitOptions options)](#process-com.aspose.cells.LowCodeSplitOptions-) | Elektronik tablo dosyasını birden fazla parçaya ayırır. |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | Verilen şablon dosyasını birden fazla parçaya böler. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### process(LowCodeSplitOptions options) {#process-com.aspose.cells.LowCodeSplitOptions-}
```
public static void process(LowCodeSplitOptions options)
```


Elektronik tablo dosyasını birden fazla parçaya ayırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [LowCodeSplitOptions](../../com.aspose.cells/lowcodesplitoptions) | Elektronik tablo bölme seçenekleri |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


Verilen şablon dosyasını birden fazla parçaya böler.

**Remarks**

Çıktı dosyaları, belirtilen sonuç dosyasına sayfa ve bölünmüş parça sıra numarası eklenerek oluşturulur. Örneğin, belirtilen çıktı dosyası Split.xlsx ise, oluşturulan dosyalar Split\_0\_0.xlsx, Split\_0\_1.xlsx, ..., Split\_1\_0.xlsx, ... şeklinde olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| templateFile | java.lang.String | Bölünecek şablon dosyası |
| resultFile | java.lang.String | Sonuç dosyası (ad deseni) |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

