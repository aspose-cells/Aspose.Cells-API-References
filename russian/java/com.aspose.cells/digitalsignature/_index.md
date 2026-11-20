---
title: "DigitalSignature"
second_title: "Справочник API Aspose.Cells for Java"
description: "Подпись в файле."
type: docs
url: /ru/java/com.aspose.cells/digitalsignature/
---

**Inheritance:**
java.lang.Object
```
public class DigitalSignature
```

Подпись в файле.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)](#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-) | Конструктор digitalSignature. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertificate()](#getCertificate--) | Объект сертификата, использованный для подписи документа. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Назначение подписи. |
| [getId()](#getId--) | Указывает GUID, который может быть сопоставлен с GUID строки подписи, хранящейся в содержимом документа. |
| [getImage()](#getImage--) | Указывает изображение для цифровой подписи. |
| [getProviderId()](#getProviderId--) | Указывает идентификатор класса поставщика подписи. |
| [getSignTime()](#getSignTime--) | Время, когда документ был подписан. |
| [getText()](#getText--) | Указывает текст фактической подписи в цифровой подписи. |
| [getXAdESType()](#getXAdESType--) | Тип XAdES. |
| [hashCode()](#hashCode--) |  |
| [isValid()](#isValid--) | Если эта цифровая подпись действительна и документ не был изменён, это значение будет true. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCertificate(KeyStore value)](#setCertificate-java.security.KeyStore-) | Объект сертификата, использованный для подписи документа. |
| [setComments(String value)](#setComments-java.lang.String-) | Назначение подписи. |
| [setId(UUID value)](#setId-java.util.UUID-) | Указывает GUID, который может быть сопоставлен с GUID строки подписи, хранящейся в содержимом документа. |
| [setImage(byte[] value)](#setImage-byte---) | Указывает изображение для цифровой подписи. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Указывает идентификатор класса поставщика подписи. |
| [setSignTime(DateTime value)](#setSignTime-com.aspose.cells.DateTime-) | Время, когда документ был подписан. |
| [setText(String value)](#setText-java.lang.String-) | Указывает текст фактической подписи в цифровой подписи. |
| [setXAdESType(int value)](#setXAdESType-int-) | Тип XAdES. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime) {#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-}
```
public DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)
```


Конструктор digitalSignature.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| certificate | java.security.KeyStore | Объект сертификата, использованный для подписи документа. |
| privateKeyPassword | java.lang.String | Пароль для закрытого ключа. |
| комментарии | java.lang.String | Назначение подписи. |
| signTime | [DateTime](../../com.aspose.cells/datetime) | Время UTC, когда документ был подписан. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCertificate() {#getCertificate--}
```
public KeyStore getCertificate()
```


Объект сертификата, использованный для подписи документа.

**Returns:**
java.security.KeyStore
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComments() {#getComments--}
```
public String getComments()
```


Назначение подписи.

**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```


Указывает GUID, который можно сопоставить с GUID строки подписи, хранящейся в содержимом документа. Значение по умолчанию — Empty (все нули) Guid.

**Remarks**

При установке связывает [SignatureLine](../../com.aspose.cells/signatureline) с соответствующей [DigitalSignature](../../com.aspose.cells/digitalsignature).

**Returns:**
java.util.UUID
### getImage() {#getImage--}
```
public byte[] getImage()
```


Указывает изображение для цифровой подписи. Значение по умолчанию — null.

**Returns:**
byte[]
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```


Указывает идентификатор класса поставщика подписи. Значение по умолчанию — Empty (все нули) Guid.

**Remarks**

Криптографический сервис-провайдер (CSP) — это независимый программный модуль, который фактически выполняет криптографические алгоритмы для аутентификации, кодирования и шифрования. Microsoft Office резервирует значение \{00000000-0000-0000-0000-000000000000\} для своего поставщика подписи по умолчанию и \{000CD6A4-0000-0000-C000-000000000046\} для своего поставщика подписи для восточноазиатских языков. GUID дополнительно установленного поставщика следует получить из документации, поставляемой с этим провайдером.

**Returns:**
java.util.UUID
### getSignTime() {#getSignTime--}
```
public DateTime getSignTime()
```


Время, когда документ был подписан.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getText() {#getText--}
```
public String getText()
```


Указывает текст фактической подписи в цифровой подписи. Значение по умолчанию — Empty.

**Returns:**
java.lang.String
### getXAdESType() {#getXAdESType--}
```
public int getXAdESType()
```


Тип XAdES. Значение по умолчанию — None (XAdES отключён).

См. [XAdESType](../../com.aspose.cells/xadestype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isValid() {#isValid--}
```
public boolean isValid()
```


Если эта цифровая подпись действительна и документ не был изменён, это значение будет true.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCertificate(KeyStore value) {#setCertificate-java.security.KeyStore-}
```
public void setCertificate(KeyStore value)
```


Объект сертификата, использованный для подписи документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.security.KeyStore |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


Назначение подписи.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Указывает GUID, который можно сопоставить с GUID строки подписи, хранящейся в содержимом документа. Значение по умолчанию — Empty (все нули) Guid.

**Remarks**

При установке связывает [SignatureLine](../../com.aspose.cells/signatureline) с соответствующей [DigitalSignature](../../com.aspose.cells/digitalsignature).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.UUID |  |

### setImage(byte[] value) {#setImage-byte---}
```
public void setImage(byte[] value)
```


Указывает изображение для цифровой подписи. Значение по умолчанию — null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte[] |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Указывает идентификатор класса поставщика подписи. Значение по умолчанию — Empty (все нули) Guid.

**Remarks**

Криптографический сервис-провайдер (CSP) — это независимый программный модуль, который фактически выполняет криптографические алгоритмы для аутентификации, кодирования и шифрования. Microsoft Office резервирует значение \{00000000-0000-0000-0000-000000000000\} для своего поставщика подписи по умолчанию и \{000CD6A4-0000-0000-C000-000000000046\} для своего поставщика подписи для восточноазиатских языков. GUID дополнительно установленного поставщика следует получить из документации, поставляемой с этим провайдером.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.UUID |  |

### setSignTime(DateTime value) {#setSignTime-com.aspose.cells.DateTime-}
```
public void setSignTime(DateTime value)
```


Время, когда документ был подписан.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Указывает текст фактической подписи в цифровой подписи. Значение по умолчанию — Empty.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setXAdESType(int value) {#setXAdESType-int-}
```
public void setXAdESType(int value)
```


Тип XAdES. Значение по умолчанию — None (XAdES отключён).

См. [XAdESType](../../com.aspose.cells/xadestype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

