---
title: "VbaProject"
second_title: "Aspose.Cells for Java API Referansı"
description: "VBA projesini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/vbaproject/
---

**Inheritance:**
java.lang.Object
```
public class VbaProject
```

VBA projesini temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [copy(VbaProject source)](#copy-com.aspose.cells.VbaProject-) | VBA projesini başka bir dosyadan kopyala. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertRawData()](#getCertRawData--) | Bu VBA projesi imzalıysa sertifikanın ham verilerini alır. |
| [getClass()](#getClass--) |  |
| [getEncoding()](#getEncoding--) | VBA projesinin kodlamasını alır. |
| [getIslockedForViewing()](#getIslockedForViewing--) | Bu VBA projesinin görüntüleme için kilitli olup olmadığını gösterir. |
| [getModules()](#getModules--) | Tüm [VbaModule](../../com.aspose.cells/vbamodule) nesnelerini alır. |
| [getName()](#getName--) | VBA projesinin adını alır. |
| [getReferences()](#getReferences--) | VBA projesinin tüm referanslarını alır. |
| [hashCode()](#hashCode--) |  |
| [isLockedForView()](#isLockedForView--) | Bu VBA projesinin görüntüleme için kilitli olup olmadığını gösterir. |
| [isProtected()](#isProtected--) | Bu VBA projesinin korumalı olup olmadığını gösterir. |
| [isSigned()](#isSigned--) | VBA kodunun imzalı olup olmadığını gösterir. |
| [isValidSigned()](#isValidSigned--) | VBA projesinin imzasının geçerli olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(boolean islockedForViewing, String password)](#protect-boolean-java.lang.String-) | Bu VBA projesini korur veya korumasını kaldırır. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | VBA projesinin kodlamasını ayarlar. |
| [setName(String value)](#setName-java.lang.String-) | VBA projesinin adını ayarlar. |
| [sign(DigitalSignature digitalSignature)](#sign-com.aspose.cells.DigitalSignature-) | Bu VBA projesini bir DigitalSignature ile imzala. |
| [toString()](#toString--) |  |
| [validatePassword(String password)](#validatePassword-java.lang.String-) | Koruma şifresini doğrular. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProject source) {#copy-com.aspose.cells.VbaProject-}
```
public void copy(VbaProject source)
```


VBA projesini başka bir dosyadan kopyala.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [VbaProject](../../com.aspose.cells/vbaproject) |  |

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
### getCertRawData() {#getCertRawData--}
```
public byte[] getCertRawData()
```


Bu VBA projesi imzalıysa sertifikanın ham verilerini alır.

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


VBA projesinin kodlamasını alır.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getIslockedForViewing() {#getIslockedForViewing--}
```
public boolean getIslockedForViewing()
```


Bu VBA projesinin görüntüleme için kilitli olup olmadığını gösterir.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen VbaProject.IsLockedForView özelliğini kullanın. Bu özellik Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getModules() {#getModules--}
```
public VbaModuleCollection getModules()
```


Tüm [VbaModule](../../com.aspose.cells/vbamodule) nesnelerini alır.

**Returns:**
[VbaModuleCollection](../../com.aspose.cells/vbamodulecollection)
### getName() {#getName--}
```
public String getName()
```


VBA projesinin adını alır.

**Returns:**
java.lang.String
### getReferences() {#getReferences--}
```
public VbaProjectReferenceCollection getReferences()
```


VBA projesinin tüm referanslarını alır.

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


Bu VBA projesinin görüntüleme için kilitli olup olmadığını gösterir. Doğruysa, kodlar görünür olmayacaktır.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Bu VBA projesinin korumalı olup olmadığını gösterir.

**Returns:**
boolean
### isSigned() {#isSigned--}
```
public boolean isSigned()
```


VBA kodunun imzalı olup olmadığını gösterir.

**Returns:**
boolean
### isValidSigned() {#isValidSigned--}
```
public boolean isValidSigned()
```


VBA projesinin imzasının geçerli olup olmadığını gösterir.

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


Bu VBA projesini korur veya korumasını kaldırır.

**Remarks**

islockedForViewing true ise, şifre null olamaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| islockedForViewing | boolean | görünüm için projenin kilitlenip kilitlenmediğini gösterir. |
| password | java.lang.String | Değer null ise, bu VBA projesinin korumasını kaldırır, aksi takdirde bu VBA projesini korur. |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


VBA projesinin kodlamasını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


VBA projesinin adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### sign(DigitalSignature digitalSignature) {#sign-com.aspose.cells.DigitalSignature-}
```
public void sign(DigitalSignature digitalSignature)
```


Bu VBA projesini bir DigitalSignature ile imzala.

**Parameters:**
| Parametre | Tür | Açıklama |
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


Koruma şifresini doğrular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| password | java.lang.String | parola |

**Returns:**
boolean - Parolanın bu VBA projesinin koruma parolası olup olmadığını belirtir
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

