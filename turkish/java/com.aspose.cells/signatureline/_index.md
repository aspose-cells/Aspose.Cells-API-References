---
title: "SignatureLine"
second_title: "Aspose.Cells for Java API Referansı"
description: "imza satırını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/signatureline/
---

**Inheritance:**
java.lang.Object
```
public class SignatureLine
```

imza satırını temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         // Create signature line object
         SignatureLine s = new SignatureLine();
         s.setSigner("Simon");
         s.setTitle("Development");
         s.setEmail("simon@aspose.com");
         s.setInstructions("Sign to confirm the excel content.");
 
         // Adds a Signature Line to the worksheet.
         Picture signatureLine = worksheet.getShapes().addSignatureLine(0, 0, s);
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SignatureLine()](#SignatureLine--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowComments()](#getAllowComments--) | Yorumların eklenip eklenemeyeceğini gösterir. |
| [getClass()](#getClass--) |  |
| [getEmail()](#getEmail--) | Şarkıcının e-posta adresini alır. |
| [getId()](#getId--) | Bu imza satırı için tanımlayıcıyı alır. |
| [getInstructions()](#getInstructions--) | İmzalama sırasında kullanıcıya gösterilen metni alır. |
| [getProviderId()](#getProviderId--) | İmza sağlayıcısının kimliğini alır. |
| [getShowSignedDate()](#getShowSignedDate--) | İmzalanma tarihinin gösterilip gösterilmeyeceğini belirtir. |
| [getSignatureLineType()](#getSignatureLineType--) | İmza tipini alır. |
| [getSigner()](#getSigner--) | İmzayı atanı alır. |
| [getTitle()](#getTitle--) | Şarkıcının unvanını alır. |
| [hashCode()](#hashCode--) |  |
| [isLine()](#isLine--) | Bir imza satırı olup olmadığını belirtir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowComments(boolean value)](#setAllowComments-boolean-) | Yorumların eklenip eklenemeyeceğini gösterir. |
| [setEmail(String value)](#setEmail-java.lang.String-) | Şarkıcının e-posta adresini ayarlar. |
| [setId(UUID value)](#setId-java.util.UUID-) | Bu imza satırı için tanımlayıcıyı ayarlar. |
| [setInstructions(String value)](#setInstructions-java.lang.String-) | İmzalama sırasında kullanıcıya gösterilen metni ayarlar. |
| [setLine(boolean value)](#setLine-boolean-) | Bir imza satırı olup olmadığını belirtir. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | İmza sağlayıcısının kimliğini ayarlar. |
| [setShowSignedDate(boolean value)](#setShowSignedDate-boolean-) | İmzalanma tarihinin gösterilip gösterilmeyeceğini belirtir. |
| [setSignatureLineType(int value)](#setSignatureLineType-int-) | İmza tipini ayarlar. |
| [setSigner(String value)](#setSigner-java.lang.String-) | İmzayı atanı ayarlar. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Şarkıcının unvanını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SignatureLine() {#SignatureLine--}
```
public SignatureLine()
```


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
### getAllowComments() {#getAllowComments--}
```
public boolean getAllowComments()
```


Yorumların eklenip eklenemeyeceğini gösterir.

**Example**

```
         if(s.getAllowComments())
         {
             // Comments could be attached.
         }
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEmail() {#getEmail--}
```
public String getEmail()
```


Şarkıcının e-posta adresini alır.

**Example**

```
         // Create signature line object
         SignatureLine s5 = new SignatureLine();
         s5.setEmail("Simon.Zhao@aspose.com");
```

**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```


Bu imza satırı için tanımlayıcıyı alır.

**Example**

```
         // Create signature line object
         SignatureLine s1 = new SignatureLine();
         s1.setId(java.util.UUID.randomUUID());
```

**Returns:**
java.util.UUID
### getInstructions() {#getInstructions--}
```
public String getInstructions()
```


İmzalama sırasında kullanıcıya gösterilen metni alır.

**Example**

```
         // Create signature line object
         SignatureLine s6 = new SignatureLine();
         s6.setInstructions("Just do it.");
```

**Returns:**
java.lang.String
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```


İmza sağlayıcısının kimliğini alır.

**Remarks**

Genellikle sağlayıcı COM eklentisinin CLSID'sidir.

**Example**

```
         // Create signature line object
         SignatureLine s2 = new SignatureLine();
         s2.setProviderId(java.util.UUID.fromString("xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"));//The GUID should be obtained from the documentation shipped with the provider.
```

**Returns:**
java.util.UUID
### getShowSignedDate() {#getShowSignedDate--}
```
public boolean getShowSignedDate()
```


İmzalanma tarihinin gösterilip gösterilmeyeceğini belirtir.

**Example**

```
         if(s.getShowSignedDate())
         {
             //Show signed date.
         }
```

**Returns:**
boolean
### getSignatureLineType() {#getSignatureLineType--}
```
public int getSignatureLineType()
```


İmza tipini alır. Default - Varsayılan değer ayarlandığında, ilgili ProviderId değeri \{0000000000-0000-0000-0000-0000000000\} olarak sabitlenir. Stamp - Değer Stamp olduğunda, ilgili ProviderId değeri genellikle \{000CD6A4-0000-0000-C000-000000000046\} olur. Custom - Değer Custom olduğunda, ilgili ProviderId değerinin genellikle kullanıcı tarafından ayarlanması gerekir. Bu değer, sağlayıcıyla birlikte gelen belgelerden elde edilmelidir.

Bakınız [SignatureType](../../com.aspose.cells/signaturetype).

**Returns:**
int
### getSigner() {#getSigner--}
```
public String getSigner()
```


İmzayı atanı alır.

**Example**

```
         // Create signature line object
         SignatureLine s3 = new SignatureLine();
         s3.setSigner("Mr xxx");
```

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Şarkıcının unvanını alır.

**Example**

```
         // Create signature line object
         SignatureLine s4 = new SignatureLine();
         s4.setTitle("Development Lead");
```

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLine() {#isLine--}
```
public boolean isLine()
```


Bir imza satırı olup olmadığını belirtir.

**Example**

```
         if(s.isLine())
         {
             //Is line.
         }
```

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




### setAllowComments(boolean value) {#setAllowComments-boolean-}
```
public void setAllowComments(boolean value)
```


Yorumların eklenip eklenemeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEmail(String value) {#setEmail-java.lang.String-}
```
public void setEmail(String value)
```


Şarkıcının e-posta adresini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Bu imza satırı için tanımlayıcıyı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.UUID |  |

### setInstructions(String value) {#setInstructions-java.lang.String-}
```
public void setInstructions(String value)
```


İmzalama sırasında kullanıcıya gösterilen metni ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setLine(boolean value) {#setLine-boolean-}
```
public void setLine(boolean value)
```


Bir imza satırı olup olmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


İmza sağlayıcısının kimliğini ayarlar.

**Remarks**

Genellikle sağlayıcı COM eklentisinin CLSID'sidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.UUID |  |

### setShowSignedDate(boolean value) {#setShowSignedDate-boolean-}
```
public void setShowSignedDate(boolean value)
```


İmzalanma tarihinin gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSignatureLineType(int value) {#setSignatureLineType-int-}
```
public void setSignatureLineType(int value)
```


İmza tipini ayarlar. Default - Varsayılan değer ayarlandığında, ilgili ProviderId değeri \{0000000000-0000-0000-0000-0000000000\} olarak sabitlenir. Stamp - Değer Stamp olduğunda, ilgili ProviderId değeri genellikle \{000CD6A4-0000-0000-C000-000000000046\} olur. Custom - Değer Custom olduğunda, ilgili ProviderId değerinin genellikle kullanıcı tarafından ayarlanması gerekir. Bu değer, sağlayıcıyla birlikte gelen belgelerden elde edilmelidir.

Bakınız [SignatureType](../../com.aspose.cells/signaturetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSigner(String value) {#setSigner-java.lang.String-}
```
public void setSigner(String value)
```


İmzayı atanı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Şarkıcının unvanını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

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

