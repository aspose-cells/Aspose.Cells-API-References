---
title: "SignatureLine"
second_title: "Aspose.Cells for Java API 参考"
description: "表示签名线。"
type: docs
url: /zh/java/com.aspose.cells/signatureline/
---

**Inheritance:**
java.lang.Object
```
public class SignatureLine
```

表示签名线。

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
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SignatureLine()](#SignatureLine--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowComments()](#getAllowComments--) | 指示是否可以附加评论。 |
| [getClass()](#getClass--) |  |
| [getEmail()](#getEmail--) | 获取签署人的电子邮件。 |
| [getId()](#getId--) | 获取此签名行的标识符。 |
| [getInstructions()](#getInstructions--) | 获取签署时向用户显示的文本。 |
| [getProviderId()](#getProviderId--) | 获取签名提供者的 ID。 |
| [getShowSignedDate()](#getShowSignedDate--) | 指示是否显示签署日期。 |
| [getSignatureLineType()](#getSignatureLineType--) | 获取签名类型。 |
| [getSigner()](#getSigner--) | 获取签名者。 |
| [getTitle()](#getTitle--) | 获取歌手的头衔。 |
| [hashCode()](#hashCode--) |  |
| [isLine()](#isLine--) | 指示它是否是签名行。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowComments(boolean value)](#setAllowComments-boolean-) | 指示是否可以附加评论。 |
| [setEmail(String value)](#setEmail-java.lang.String-) | 设置歌手的电子邮件。 |
| [setId(UUID value)](#setId-java.util.UUID-) | 设置此签名行的标识符。 |
| [setInstructions(String value)](#setInstructions-java.lang.String-) | 设置在签署时向用户显示的文本。 |
| [setLine(boolean value)](#setLine-boolean-) | 指示它是否是签名行。 |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | 设置签名提供程序的 ID。 |
| [setShowSignedDate(boolean value)](#setShowSignedDate-boolean-) | 指示是否显示签署日期。 |
| [setSignatureLineType(int value)](#setSignatureLineType-int-) | 设置签名类型。 |
| [setSigner(String value)](#setSigner-java.lang.String-) | 设置签名者。 |
| [setTitle(String value)](#setTitle-java.lang.String-) | 设置歌手的头衔。 |
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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowComments() {#getAllowComments--}
```
public boolean getAllowComments()
```


指示是否可以附加评论。

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


获取签署人的电子邮件。

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


获取此签名行的标识符。

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


获取签署时向用户显示的文本。

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


获取签名提供者的 ID。

**Remarks**

它通常是提供程序 COM 加载项的 CLSID。

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


指示是否显示签署日期。

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


获取签名类型。默认 - 当默认值被设置时，相应的 ProviderId 值固定为 \{0000000000-0000-0000-0000-0000000000\}。Stamp - 当值为 Stamp 时，相应的 ProviderId 值通常为 \{000CD6A4-0000-0000-C000-000000000046\}。Custom - 当值为 Custom 时，相应的 ProviderId 值通常需要用户设置。它应从随提供程序提供的文档中获取。

请参阅 [SignatureType](../../com.aspose.cells/signaturetype)。

**Returns:**
int
### getSigner() {#getSigner--}
```
public String getSigner()
```


获取签名者。

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


获取歌手的头衔。

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


指示它是否是签名行。

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


指示是否可以附加评论。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEmail(String value) {#setEmail-java.lang.String-}
```
public void setEmail(String value)
```


设置歌手的电子邮件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


设置此签名行的标识符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.UUID |  |

### setInstructions(String value) {#setInstructions-java.lang.String-}
```
public void setInstructions(String value)
```


设置在签署时向用户显示的文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setLine(boolean value) {#setLine-boolean-}
```
public void setLine(boolean value)
```


指示它是否是签名行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


设置签名提供程序的 ID。

**Remarks**

它通常是提供程序 COM 加载项的 CLSID。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.UUID |  |

### setShowSignedDate(boolean value) {#setShowSignedDate-boolean-}
```
public void setShowSignedDate(boolean value)
```


指示是否显示签署日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSignatureLineType(int value) {#setSignatureLineType-int-}
```
public void setSignatureLineType(int value)
```


获取签名类型。默认 - 当默认值被设置时，相应的 ProviderId 值固定为 \{0000000000-0000-0000-0000-0000000000\}。Stamp - 当值为 Stamp 时，相应的 ProviderId 值通常为 \{000CD6A4-0000-0000-C000-000000000046\}。Custom - 当值为 Custom 时，相应的 ProviderId 值通常需要用户设置。它应从随提供程序提供的文档中获取。

请参阅 [SignatureType](../../com.aspose.cells/signaturetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSigner(String value) {#setSigner-java.lang.String-}
```
public void setSigner(String value)
```


设置签名者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


设置歌手的头衔。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

