---
title: "DigitalSignature"
second_title: "Aspose.Cells for Java API Reference"
description: "التوقيع في الملف."
type: docs
url: /ar/java/com.aspose.cells/digitalsignature/
---

**Inheritance:**
java.lang.Object
```
public class DigitalSignature
```

التوقيع في الملف.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)](#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-) | منشئ digitalSignature. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertificate()](#getCertificate--) | كائن الشهادة الذي تم استخدامه لتوقيع المستند. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | الغرض من التوقيع. |
| [getId()](#getId--) | يحدد GUID يمكن ربطه عبر المرجع مع GUID لخط التوقيع المخزن في محتوى المستند. |
| [getImage()](#getImage--) | يحدد صورة للتوقيع الرقمي. |
| [getProviderId()](#getProviderId--) | يحدد معرف الفئة (class ID) لمزود التوقيع. |
| [getSignTime()](#getSignTime--) | الوقت الذي تم فيه توقيع المستند. |
| [getText()](#getText--) | يحدد نص التوقيع الفعلي في التوقيع الرقمي. |
| [getXAdESType()](#getXAdESType--) | نوع XAdES. |
| [hashCode()](#hashCode--) |  |
| [isValid()](#isValid--) | إذا كان هذا التوقيع الرقمي صالحًا ولم يتم العبث بالمستند، ستكون القيمة true. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCertificate(KeyStore value)](#setCertificate-java.security.KeyStore-) | كائن الشهادة الذي تم استخدامه لتوقيع المستند. |
| [setComments(String value)](#setComments-java.lang.String-) | الغرض من التوقيع. |
| [setId(UUID value)](#setId-java.util.UUID-) | يحدد GUID يمكن ربطه عبر المرجع مع GUID لخط التوقيع المخزن في محتوى المستند. |
| [setImage(byte[] value)](#setImage-byte---) | يحدد صورة للتوقيع الرقمي. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | يحدد معرف الفئة (class ID) لمزود التوقيع. |
| [setSignTime(DateTime value)](#setSignTime-com.aspose.cells.DateTime-) | الوقت الذي تم فيه توقيع المستند. |
| [setText(String value)](#setText-java.lang.String-) | يحدد نص التوقيع الفعلي في التوقيع الرقمي. |
| [setXAdESType(int value)](#setXAdESType-int-) | نوع XAdES. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime) {#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-}
```
public DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)
```


منشئ digitalSignature.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| certificate | java.security.KeyStore | كائن الشهادة الذي تم استخدامه لتوقيع المستند. |
| privateKeyPassword | java.lang.String | كلمة المرور للمفتاح الخاص. |
| تعليقات | java.lang.String | الغرض من التوقيع. |
| signTime | [DateTime](../../com.aspose.cells/datetime) | وقت UTC عندما تم توقيع المستند. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCertificate() {#getCertificate--}
```
public KeyStore getCertificate()
```


كائن الشهادة الذي تم استخدامه لتوقيع المستند.

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


الغرض من التوقيع.

**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```


يحدد GUID يمكن ربطه عبر المرجع مع GUID لخط التوقيع المخزن في محتوى المستند. القيمة الافتراضية هي Empty (جميع الأصفار) Guid.

**Remarks**

عند التعيين، يربط [SignatureLine](../../com.aspose.cells/signatureline) بـ [DigitalSignature](../../com.aspose.cells/digitalsignature) المقابل.

**Returns:**
java.util.UUID
### getImage() {#getImage--}
```
public byte[] getImage()
```


يحدد صورة للتوقيع الرقمي. القيمة الافتراضية هي null.

**Returns:**
byte[]
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```


يحدد معرف الفئة (class ID) لمزود التوقيع. القيمة الافتراضية هي Empty (جميع الأصفار) Guid.

**Remarks**

مزود الخدمة المشفرة (CSP) هو وحدة برمجية مستقلة تقوم فعليًا بتنفيذ خوارزميات التشفير للمصادقة والترميز والتشفير. تحتفظ Microsoft Office بالقيمة \{00000000-0000-0000-0000-000000000000\} لمزود التوقيع الافتراضي، و \{000CD6A4-0000-0000-C000-000000000046\} لمزود التوقيع للغات شرق آسيا. يجب الحصول على GUID للمزود المثبت إضافيًا من الوثائق المرفقة مع المزود.

**Returns:**
java.util.UUID
### getSignTime() {#getSignTime--}
```
public DateTime getSignTime()
```


الوقت الذي تم فيه توقيع المستند.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getText() {#getText--}
```
public String getText()
```


يحدد نص التوقيع الفعلي في التوقيع الرقمي. القيمة الافتراضية هي Empty.

**Returns:**
java.lang.String
### getXAdESType() {#getXAdESType--}
```
public int getXAdESType()
```


نوع XAdES. القيمة الافتراضية هي None (XAdES غير مفعل).

انظر [XAdESType](../../com.aspose.cells/xadestype).

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


إذا كان هذا التوقيع الرقمي صالحًا ولم يتم العبث بالمستند، ستكون القيمة true.

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


كائن الشهادة الذي تم استخدامه لتوقيع المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.security.KeyStore |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


الغرض من التوقيع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


يحدد GUID يمكن ربطه عبر المرجع مع GUID لخط التوقيع المخزن في محتوى المستند. القيمة الافتراضية هي Empty (جميع الأصفار) Guid.

**Remarks**

عند التعيين، يربط [SignatureLine](../../com.aspose.cells/signatureline) بـ [DigitalSignature](../../com.aspose.cells/digitalsignature) المقابل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.UUID |  |

### setImage(byte[] value) {#setImage-byte---}
```
public void setImage(byte[] value)
```


يحدد صورة للتوقيع الرقمي. القيمة الافتراضية هي null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte[] |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


يحدد معرف الفئة (class ID) لمزود التوقيع. القيمة الافتراضية هي Empty (جميع الأصفار) Guid.

**Remarks**

مزود الخدمة المشفرة (CSP) هو وحدة برمجية مستقلة تقوم فعليًا بتنفيذ خوارزميات التشفير للمصادقة والترميز والتشفير. تحتفظ Microsoft Office بالقيمة \{00000000-0000-0000-0000-000000000000\} لمزود التوقيع الافتراضي، و \{000CD6A4-0000-0000-C000-000000000046\} لمزود التوقيع للغات شرق آسيا. يجب الحصول على GUID للمزود المثبت إضافيًا من الوثائق المرفقة مع المزود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.UUID |  |

### setSignTime(DateTime value) {#setSignTime-com.aspose.cells.DateTime-}
```
public void setSignTime(DateTime value)
```


الوقت الذي تم فيه توقيع المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


يحدد نص التوقيع الفعلي في التوقيع الرقمي. القيمة الافتراضية هي Empty.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setXAdESType(int value) {#setXAdESType-int-}
```
public void setXAdESType(int value)
```


نوع XAdES. القيمة الافتراضية هي None (XAdES غير مفعل).

انظر [XAdESType](../../com.aspose.cells/xadestype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

