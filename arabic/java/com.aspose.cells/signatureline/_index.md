---
title: "SignatureLine"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خط التوقيع."
type: docs
url: /ar/java/com.aspose.cells/signatureline/
---

**Inheritance:**
java.lang.Object
```
public class SignatureLine
```

يمثل خط التوقيع.

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
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SignatureLine()](#SignatureLine--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowComments()](#getAllowComments--) | يشير إلى ما إذا كان يمكن إرفاق التعليقات. |
| [getClass()](#getClass--) |  |
| [getEmail()](#getEmail--) | يحصل على البريد الإلكتروني للمغني. |
| [getId()](#getId--) | يحصل على المعرف لهذا سطر التوقيع. |
| [getInstructions()](#getInstructions--) | يحصل على النص المعروض للمستخدم عند توقيع. |
| [getProviderId()](#getProviderId--) | يحصل على معرف موفر التوقيع. |
| [getShowSignedDate()](#getShowSignedDate--) | يشير إلى ما إذا كان يُظهر تاريخ التوقيع. |
| [getSignatureLineType()](#getSignatureLineType--) | يحصل على نوع التوقيع. |
| [getSigner()](#getSigner--) | يحصل على المُوقّع. |
| [getTitle()](#getTitle--) | يحصل على لقب المغني. |
| [hashCode()](#hashCode--) |  |
| [isLine()](#isLine--) | يشير إلى ما إذا كان سطر توقيع. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowComments(boolean value)](#setAllowComments-boolean-) | يشير إلى ما إذا كان يمكن إرفاق التعليقات. |
| [setEmail(String value)](#setEmail-java.lang.String-) | يضبط البريد الإلكتروني للمغني. |
| [setId(UUID value)](#setId-java.util.UUID-) | يضبط المعرف لهذا سطر التوقيع. |
| [setInstructions(String value)](#setInstructions-java.lang.String-) | يضبط النص المعروض للمستخدم عند توقيع. |
| [setLine(boolean value)](#setLine-boolean-) | يشير إلى ما إذا كان سطر توقيع. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | يضبط معرف موفر التوقيع. |
| [setShowSignedDate(boolean value)](#setShowSignedDate-boolean-) | يشير إلى ما إذا كان يُظهر تاريخ التوقيع. |
| [setSignatureLineType(int value)](#setSignatureLineType-int-) | يضبط نوع التوقيع. |
| [setSigner(String value)](#setSigner-java.lang.String-) | يضبط المُوقّع. |
| [setTitle(String value)](#setTitle-java.lang.String-) | يضبط لقب المغني. |
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowComments() {#getAllowComments--}
```
public boolean getAllowComments()
```


يشير إلى ما إذا كان يمكن إرفاق التعليقات.

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


يحصل على البريد الإلكتروني للمغني.

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


يحصل على المعرف لهذا سطر التوقيع.

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


يحصل على النص المعروض للمستخدم عند توقيع.

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


يحصل على معرف موفر التوقيع.

**Remarks**

عادةً ما يكون CLSID لإضافة com الخاصة بالموفر.

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


يشير إلى ما إذا كان يُظهر تاريخ التوقيع.

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


يحصل على نوع التوقيع. Default - عندما يتم تعيين القيمة الافتراضية، تكون قيمة ProviderId المقابلة ثابتة إلى \{0000000000-0000-0000-0000-0000000000\}. Stamp - عندما تكون القيمة Stamp، تكون قيمة ProviderId المقابلة عادةً \{000CD6A4-0000-0000-C000-000000000046\}. Custom - عندما تكون القيمة Custom، عادةً ما تحتاج قيمة ProviderId المقابلة إلى أن يتم تعيينها من قبل المستخدم. يجب الحصول عليها من الوثائق المرفقة مع الموفر.

انظر [SignatureType](../../com.aspose.cells/signaturetype).

**Returns:**
int
### getSigner() {#getSigner--}
```
public String getSigner()
```


يحصل على المُوقّع.

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


يحصل على لقب المغني.

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


يشير إلى ما إذا كان سطر توقيع.

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


يشير إلى ما إذا كان يمكن إرفاق التعليقات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEmail(String value) {#setEmail-java.lang.String-}
```
public void setEmail(String value)
```


يضبط البريد الإلكتروني للمغني.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


يضبط المعرف لهذا سطر التوقيع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.UUID |  |

### setInstructions(String value) {#setInstructions-java.lang.String-}
```
public void setInstructions(String value)
```


يضبط النص المعروض للمستخدم عند توقيع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setLine(boolean value) {#setLine-boolean-}
```
public void setLine(boolean value)
```


يشير إلى ما إذا كان سطر توقيع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


يضبط معرف موفر التوقيع.

**Remarks**

عادةً ما يكون CLSID لإضافة com الخاصة بالموفر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.UUID |  |

### setShowSignedDate(boolean value) {#setShowSignedDate-boolean-}
```
public void setShowSignedDate(boolean value)
```


يشير إلى ما إذا كان يُظهر تاريخ التوقيع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSignatureLineType(int value) {#setSignatureLineType-int-}
```
public void setSignatureLineType(int value)
```


يضبط نوع التوقيع. Default - عندما يتم تعيين القيمة الافتراضية، تكون قيمة ProviderId المقابلة ثابتة إلى \{0000000000-0000-0000-0000-0000000000\}. Stamp - عندما تكون القيمة Stamp، تكون قيمة ProviderId المقابلة عادةً \{000CD6A4-0000-0000-C000-000000000046\}. Custom - عندما تكون القيمة Custom، عادةً ما تحتاج قيمة ProviderId المقابلة إلى أن يتم تعيينها من قبل المستخدم. يجب الحصول عليها من الوثائق المرفقة مع الموفر.

انظر [SignatureType](../../com.aspose.cells/signaturetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSigner(String value) {#setSigner-java.lang.String-}
```
public void setSigner(String value)
```


يضبط المُوقّع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


يضبط لقب المغني.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

