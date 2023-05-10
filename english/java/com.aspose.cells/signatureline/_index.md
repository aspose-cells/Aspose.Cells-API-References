---
title: SignatureLine
second_title: Aspose.Cells for Java API Reference
description: Represent the signature line.
type: docs
url: /java/com.aspose.cells/signatureline/
---

**Inheritance:**
java.lang.Object
```
public class SignatureLine
```

Represent the signature line.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Adding a picture
         int imgIndex = worksheet.getPictures().add(1, 1, "sample.png");
         Picture pic = worksheet.getPictures().get(imgIndex);
         // Create signature line object
         SignatureLine s = new SignatureLine();
         s.setSigner("Simon Zhao");
         s.setTitle("Development Lead");
         s.setEmail("Simon.Zhao@aspose.com");
         // Assign the signature line object to Picture.SignatureLine property
         pic.setSignatureLine(s);
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## Constructors

| Constructor | Description |
| --- | --- |
| [SignatureLine()](#SignatureLine--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowComments()](#getAllowComments--) | Indicates whether comments could be attached. |
| [getClass()](#getClass--) |  |
| [getEmail()](#getEmail--) | Gets the email of singer. |
| [getId()](#getId--) | Gets identifier for this signature line. |
| [getInstructions()](#getInstructions--) | Gets the text shown to user at signing time. |
| [getProviderId()](#getProviderId--) | Gets the id of signature provider. |
| [getShowSignedDate()](#getShowSignedDate--) | Indicates whether show signed date. |
| [getSigner()](#getSigner--) | Gets the signer. |
| [getTitle()](#getTitle--) | Gets the title of singer. |
| [hashCode()](#hashCode--) |  |
| [isLine()](#isLine--) | Indicates whether it is a signature line. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowComments(boolean value)](#setAllowComments-boolean-) | Indicates whether comments could be attached. |
| [setEmail(String value)](#setEmail-java.lang.String-) | Sets the email of singer. |
| [setId(UUID value)](#setId-java.util.UUID-) | Sets identifier for this signature line. |
| [setInstructions(String value)](#setInstructions-java.lang.String-) | Sets the text shown to user at signing time. |
| [setLine(boolean value)](#setLine-boolean-) | Indicates whether it is a signature line. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Sets the id of signature provider. |
| [setShowSignedDate(boolean value)](#setShowSignedDate-boolean-) | Indicates whether show signed date. |
| [setSigner(String value)](#setSigner-java.lang.String-) | Sets the signer. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Sets the title of singer. |
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowComments() {#getAllowComments--}
```
public boolean getAllowComments()
```


Indicates whether comments could be attached.

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


Gets the email of singer.

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


Gets identifier for this signature line.

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


Gets the text shown to user at signing time.

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


Gets the id of signature provider. It's typically the CLSID of the provider com add-in.

**Example**

```
// Create signature line object
         SignatureLine s2 = new SignatureLine();
         s2.setProviderId(java.util.UUID.randomUUID());
```

**Returns:**
java.util.UUID
### getShowSignedDate() {#getShowSignedDate--}
```
public boolean getShowSignedDate()
```


Indicates whether show signed date.

**Example**

```
if(s.getShowSignedDate())
         {
             //Show signed date.
         }
```

**Returns:**
boolean
### getSigner() {#getSigner--}
```
public String getSigner()
```


Gets the signer.

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


Gets the title of singer.

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


Indicates whether it is a signature line.

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


Indicates whether comments could be attached.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEmail(String value) {#setEmail-java.lang.String-}
```
public void setEmail(String value)
```


Sets the email of singer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Sets identifier for this signature line.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID |  |

### setInstructions(String value) {#setInstructions-java.lang.String-}
```
public void setInstructions(String value)
```


Sets the text shown to user at signing time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLine(boolean value) {#setLine-boolean-}
```
public void setLine(boolean value)
```


Indicates whether it is a signature line.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Sets the id of signature provider. It's typically the CLSID of the provider com add-in.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID |  |

### setShowSignedDate(boolean value) {#setShowSignedDate-boolean-}
```
public void setShowSignedDate(boolean value)
```


Indicates whether show signed date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSigner(String value) {#setSigner-java.lang.String-}
```
public void setSigner(String value)
```


Sets the signer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Sets the title of singer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

