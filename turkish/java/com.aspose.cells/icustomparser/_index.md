---
title: "ICustomParser"
second_title: "Aspose.Cells for Java API Referansı"
description: "Kullanıcıların dize değerlerini diğer uygun hücre değeri nesnelerine ayrıştırmak için özel değer ayrıştırıcılarını eklemelerine izin verir."
type: docs
url: /tr/java/com.aspose.cells/icustomparser/
---
```
public interface ICustomParser
```

Kullanıcıların dize değerlerini diğer uygun hücre değeri nesnelerine ayrıştırmak için özel değer ayrıştırıcılarını eklemelerine izin verir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getFormat()](#getFormat--) | Son çağrıda [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-) tarafından ayrıştırılan değere karşılık gelen biçimlendirme desenini alır. |
| [parseObject(String value)](#parseObject-java.lang.String-) | Verilen dizeyi uygun değer nesnesine ayrıştırır. |
### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Son çağrıda [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-) tarafından ayrıştırılan değere karşılık gelen biçimlendirme desenini alır.

**Remarks**

İade edilen biçimlendirme deseni, ilgili hücreyi biçimlendirmek için kullanılabilir (hücre için Style.Custom olarak ayarlanmalıdır).

**Returns:**
java.lang.String
### parseObject(String value) {#parseObject-java.lang.String-}
```
public abstract Object parseObject(String value)
```


Verilen dizeyi uygun değer nesnesine ayrıştırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Ayrıştırılacak dize değeri |

**Returns:**
java.lang.Object - Verilen dizeden ayrıştırılan değer nesnesi. Verilen dize uygun değer nesnesine ayrıştırılamazsa, null döndürür.
