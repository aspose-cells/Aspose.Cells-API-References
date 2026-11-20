---
title: "SignatureLine"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет строку подписи."
type: docs
url: /ru/java/com.aspose.cells/signatureline/
---

**Inheritance:**
java.lang.Object
```
public class SignatureLine
```

Представляет строку подписи.

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
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SignatureLine()](#SignatureLine--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowComments()](#getAllowComments--) | Указывает, могут ли быть прикреплены комментарии. |
| [getClass()](#getClass--) |  |
| [getEmail()](#getEmail--) | Получает электронную почту исполнителя. |
| [getId()](#getId--) | Получает идентификатор этой строки подписи. |
| [getInstructions()](#getInstructions--) | Получает текст, отображаемый пользователю во время подписания. |
| [getProviderId()](#getProviderId--) | Получает идентификатор поставщика подписи. |
| [getShowSignedDate()](#getShowSignedDate--) | Указывает, показывать ли дату подписи. |
| [getSignatureLineType()](#getSignatureLineType--) | Получает тип подписи. |
| [getSigner()](#getSigner--) | Получает подписанта. |
| [getTitle()](#getTitle--) | Получает должность исполнителя. |
| [hashCode()](#hashCode--) |  |
| [isLine()](#isLine--) | Указывает, является ли это строкой подписи. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowComments(boolean value)](#setAllowComments-boolean-) | Указывает, могут ли быть прикреплены комментарии. |
| [setEmail(String value)](#setEmail-java.lang.String-) | Устанавливает электронную почту исполнителя. |
| [setId(UUID value)](#setId-java.util.UUID-) | Устанавливает идентификатор этой строки подписи. |
| [setInstructions(String value)](#setInstructions-java.lang.String-) | Устанавливает текст, отображаемый пользователю во время подписания. |
| [setLine(boolean value)](#setLine-boolean-) | Указывает, является ли это строкой подписи. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Устанавливает идентификатор поставщика подписи. |
| [setShowSignedDate(boolean value)](#setShowSignedDate-boolean-) | Указывает, показывать ли дату подписи. |
| [setSignatureLineType(int value)](#setSignatureLineType-int-) | Устанавливает тип подписи. |
| [setSigner(String value)](#setSigner-java.lang.String-) | Устанавливает подписанта. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Устанавливает должность исполнителя. |
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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowComments() {#getAllowComments--}
```
public boolean getAllowComments()
```


Указывает, могут ли быть прикреплены комментарии.

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


Получает электронную почту исполнителя.

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


Получает идентификатор этой строки подписи.

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


Получает текст, отображаемый пользователю во время подписания.

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


Получает идентификатор поставщика подписи.

**Remarks**

Обычно это CLSID COM‑надстройки поставщика.

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


Указывает, показывать ли дату подписи.

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


Получает тип подписи. Default — когда значение по умолчанию установлено, соответствующее значение ProviderId фиксируется как \{0000000000-0000-0000-0000-0000000000\}. Stamp — когда значение равно Stamp, соответствующее значение ProviderId обычно равно \{000CD6A4-0000-0000-C000-000000000046\}. Custom — когда значение равно Custom, соответствующее значение ProviderId обычно должно быть задано пользователем. Его следует получить из документации, поставляемой с провайдером.

См. [SignatureType](../../com.aspose.cells/signaturetype).

**Returns:**
int
### getSigner() {#getSigner--}
```
public String getSigner()
```


Получает подписанта.

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


Получает должность исполнителя.

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


Указывает, является ли это строкой подписи.

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


Указывает, могут ли быть прикреплены комментарии.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEmail(String value) {#setEmail-java.lang.String-}
```
public void setEmail(String value)
```


Устанавливает электронную почту исполнителя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Устанавливает идентификатор этой строки подписи.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.UUID |  |

### setInstructions(String value) {#setInstructions-java.lang.String-}
```
public void setInstructions(String value)
```


Устанавливает текст, отображаемый пользователю во время подписания.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setLine(boolean value) {#setLine-boolean-}
```
public void setLine(boolean value)
```


Указывает, является ли это строкой подписи.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Устанавливает идентификатор поставщика подписи.

**Remarks**

Обычно это CLSID COM‑надстройки поставщика.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.UUID |  |

### setShowSignedDate(boolean value) {#setShowSignedDate-boolean-}
```
public void setShowSignedDate(boolean value)
```


Указывает, показывать ли дату подписи.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSignatureLineType(int value) {#setSignatureLineType-int-}
```
public void setSignatureLineType(int value)
```


Устанавливает тип подписи. Default — когда значение по умолчанию установлено, соответствующее значение ProviderId фиксируется как \{0000000000-0000-0000-0000-0000000000\}. Stamp — когда значение равно Stamp, соответствующее значение ProviderId обычно равно \{000CD6A4-0000-0000-C000-000000000046\}. Custom — когда значение равно Custom, соответствующее значение ProviderId обычно должно быть задано пользователем. Его следует получить из документации, поставляемой с провайдером.

См. [SignatureType](../../com.aspose.cells/signaturetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSigner(String value) {#setSigner-java.lang.String-}
```
public void setSigner(String value)
```


Устанавливает подписанта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Устанавливает должность исполнителя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

