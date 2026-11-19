---
title: "VbaProject"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مشروع VBA."
type: docs
url: /ar/java/com.aspose.cells/vbaproject/
---

**Inheritance:**
java.lang.Object
```
public class VbaProject
```

يمثل مشروع VBA.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [copy(VbaProject source)](#copy-com.aspose.cells.VbaProject-) | نسخ مشروع VBA من ملف آخر. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertRawData()](#getCertRawData--) | يحصل على البيانات الأولية للشهادة إذا تم توقيع مشروع VBA هذا. |
| [getClass()](#getClass--) |  |
| [getEncoding()](#getEncoding--) | يحصل على ترميز مشروع VBA. |
| [getIslockedForViewing()](#getIslockedForViewing--) | يشير إلى ما إذا كان مشروع VBA هذا مقفلًا للعرض. |
| [getModules()](#getModules--) | يحصل على جميع كائنات [VbaModule](../../com.aspose.cells/vbamodule). |
| [getName()](#getName--) | يحصل على اسم مشروع VBA. |
| [getReferences()](#getReferences--) | يحصل على جميع مراجع مشروع VBA. |
| [hashCode()](#hashCode--) |  |
| [isLockedForView()](#isLockedForView--) | يشير إلى ما إذا كان مشروع VBA هذا مقفلًا للعرض. |
| [isProtected()](#isProtected--) | يشير إلى ما إذا كان مشروع VBA هذا محميًا. |
| [isSigned()](#isSigned--) | يشير إلى ما إذا كان VBAcode موقّعًا أم لا. |
| [isValidSigned()](#isValidSigned--) | يشير إلى ما إذا كانت توقيع مشروع VBA صالحًا أم لا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(boolean islockedForViewing, String password)](#protect-boolean-java.lang.String-) | يحمي أو يلغي حماية مشروع VBA هذا. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | يضبط ترميز مشروع VBA. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم مشروع VBA. |
| [sign(DigitalSignature digitalSignature)](#sign-com.aspose.cells.DigitalSignature-) | وقّع مشروع VBA هذا باستخدام توقيع رقمي |
| [toString()](#toString--) |  |
| [validatePassword(String password)](#validatePassword-java.lang.String-) | يتحقق من صحة كلمة مرور الحماية. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProject source) {#copy-com.aspose.cells.VbaProject-}
```
public void copy(VbaProject source)
```


نسخ مشروع VBA من ملف آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [VbaProject](../../com.aspose.cells/vbaproject) |  |

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
### getCertRawData() {#getCertRawData--}
```
public byte[] getCertRawData()
```


يحصل على البيانات الأولية للشهادة إذا تم توقيع مشروع VBA هذا.

**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


يحصل على ترميز مشروع VBA.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getIslockedForViewing() {#getIslockedForViewing--}
```
public boolean getIslockedForViewing()
```


يشير إلى ما إذا كان مشروع VBA هذا مقفلًا للعرض.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام الخاصية VbaProject.IsLockedForView. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getModules() {#getModules--}
```
public VbaModuleCollection getModules()
```


يحصل على جميع كائنات [VbaModule](../../com.aspose.cells/vbamodule).

**Returns:**
[VbaModuleCollection](../../com.aspose.cells/vbamodulecollection)
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم مشروع VBA.

**Returns:**
java.lang.String
### getReferences() {#getReferences--}
```
public VbaProjectReferenceCollection getReferences()
```


يحصل على جميع مراجع مشروع VBA.

**Returns:**
[VbaProjectReferenceCollection](../../com.aspose.cells/vbaprojectreferencecollection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLockedForView() {#isLockedForView--}
```
public boolean isLockedForView()
```


يشير إلى ما إذا كان مشروع VBA هذا مقفلًا للعرض. إذا كان صحيحًا، لا يمكن رؤية الشيفرات.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


يشير إلى ما إذا كان مشروع VBA هذا محميًا.

**Returns:**
boolean
### isSigned() {#isSigned--}
```
public boolean isSigned()
```


يشير إلى ما إذا كان VBAcode موقّعًا أم لا.

**Returns:**
boolean
### isValidSigned() {#isValidSigned--}
```
public boolean isValidSigned()
```


يشير إلى ما إذا كانت توقيع مشروع VBA صالحًا أم لا.

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




### protect(boolean islockedForViewing, String password) {#protect-boolean-java.lang.String-}
```
public void protect(boolean islockedForViewing, String password)
```


يحمي أو يلغي حماية مشروع VBA هذا.

**Remarks**

إذا كان islockedForViewing صحيحًا، لا يمكن أن تكون كلمة المرور فارغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| islockedForViewing | boolean | يشير إلى ما إذا كان يقفل المشروع للعرض. |
| password | java.lang.String | إذا كانت القيمة فارغة، يلغي حماية مشروع VBA هذا، وإلا يحمي مشروع VBA هذا. |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


يضبط ترميز مشروع VBA.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يضبط اسم مشروع VBA.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### sign(DigitalSignature digitalSignature) {#sign-com.aspose.cells.DigitalSignature-}
```
public void sign(DigitalSignature digitalSignature)
```


وقّع مشروع VBA هذا باستخدام توقيع رقمي

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../../com.aspose.cells/digitalsignature) | DigitalSignature |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### validatePassword(String password) {#validatePassword-java.lang.String-}
```
public boolean validatePassword(String password)
```


يتحقق من صحة كلمة مرور الحماية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| password | java.lang.String | كلمة المرور |

**Returns:**
boolean - ما إذا كانت كلمة المرور هي كلمة المرور الحامية لهذا مشروع VBA
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

