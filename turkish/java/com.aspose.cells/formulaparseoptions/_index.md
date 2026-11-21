---
title: "FormulaParseOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Formül ayrıştırılırken seçenekleri temsil eder."
type: docs
url: /tr/java/com.aspose.cells/formulaparseoptions/
---

**Inheritance:**
java.lang.Object
```
public class FormulaParseOptions
```

Formül ayrıştırılırken seçenekleri temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FormulaParseOptions()](#FormulaParseOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckAddIn()](#getCheckAddIn--) | Mevcut çalışma kitabının mevcut dış bağlantılarında kullanıcı tanımlı işlev için dış bağlantı olmadan eklentileri kontrol edip etmeyeceği. |
| [getClass()](#getClass--) |  |
| [getCustomFunctionDefinition()](#getCustomFunctionDefinition--) | Özel işlevlerin ayrıştırılması için tanım. |
| [getLocaleDependent()](#getLocaleDependent--) | Formülün yerel ayara göre biçimlendirilip biçimlendirilmediği. |
| [getParse()](#getParse--) | Verilen formülün ayrıştırılıp ayrıştırılmayacağı. |
| [getR1C1Style()](#getR1C1Style--) | Formülün R1C1 referans stilinde olup olmadığı. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckAddIn(boolean value)](#setCheckAddIn-boolean-) | Mevcut çalışma kitabının mevcut dış bağlantılarında kullanıcı tanımlı işlev için dış bağlantı olmadan eklentileri kontrol edip etmeyeceği. |
| [setCustomFunctionDefinition(CustomFunctionDefinition value)](#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Özel işlevlerin ayrıştırılması için tanım. |
| [setLocaleDependent(boolean value)](#setLocaleDependent-boolean-) | Formülün yerel ayara göre biçimlendirilip biçimlendirilmediği. |
| [setParse(boolean value)](#setParse-boolean-) | Verilen formülün ayrıştırılıp ayrıştırılmayacağı. |
| [setR1C1Style(boolean value)](#setR1C1Style-boolean-) | Formülün R1C1 referans stilinde olup olmadığı. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FormulaParseOptions() {#FormulaParseOptions--}
```
public FormulaParseOptions()
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
### getCheckAddIn() {#getCheckAddIn--}
```
public boolean getCheckAddIn()
```


Mevcut çalışma kitabının mevcut dış bağlantılarında kullanıcı tanımlı işlev için dış bağlantı olmadan eklentileri kontrol edip etmeyeceği. Varsayılan değer true'tur (eğer kullanıcı tanımlı işlev mevcut dış bağlantılardaki bir eklentiyle eşleşirse, o eklenti olarak kabul edilir).

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomFunctionDefinition() {#getCustomFunctionDefinition--}
```
public CustomFunctionDefinition getCustomFunctionDefinition()
```


Özel işlevlerin ayrıştırılması için tanım.

**Remarks**

Bazı özel gereksinimler için, örneğin kullanıcının özel motorunda özel işlev hesaplanırken, bazı parametrelerin dizi modunda hesaplanması gerektiğinde, bu özelliği kullanarak formül ayrıştırılırken bu parametreleri dizi modu olarak işaretleyebilirsiniz. Aksi takdirde kullanıcı, aynı sonucu elde etmek için bu özel işlevleri daha sonra [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-) ile güncellemelidir.

**Returns:**
[CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition)
### getLocaleDependent() {#getLocaleDependent--}
```
public boolean getLocaleDependent()
```


Formülün yerel ayarlara göre biçimlendirilip biçimlendirilmediği. Varsayılan değer false'tur.

**Returns:**
boolean
### getParse() {#getParse--}
```
public boolean getParse()
```


Verilen formülün ayrıştırılıp ayrıştırılmayacağı. Varsayılan değer true'tur. False ise, verilen formül dizesi hücrede olduğu gibi tutulur ve kullanıcı başka yöntemlerle ayrıştırana kadar veya formül verileri diğer işlemler (örneğin formüllerin hesaplanması) için gerektiğinde ayrıştırılmaz.

**Returns:**
boolean
### getR1C1Style() {#getR1C1Style--}
```
public boolean getR1C1Style()
```


Formülün R1C1 referans stilinde olup olmadığı. Varsayılan değer false'tur.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCheckAddIn(boolean value) {#setCheckAddIn-boolean-}
```
public void setCheckAddIn(boolean value)
```


Mevcut çalışma kitabının mevcut dış bağlantılarında kullanıcı tanımlı işlev için dış bağlantı olmadan eklentileri kontrol edip etmeyeceği. Varsayılan değer true'tur (eğer kullanıcı tanımlı işlev mevcut dış bağlantılardaki bir eklentiyle eşleşirse, o eklenti olarak kabul edilir).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCustomFunctionDefinition(CustomFunctionDefinition value) {#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void setCustomFunctionDefinition(CustomFunctionDefinition value)
```


Özel işlevlerin ayrıştırılması için tanım.

**Remarks**

Bazı özel gereksinimler için, örneğin kullanıcının özel motorunda özel işlev hesaplanırken, bazı parametrelerin dizi modunda hesaplanması gerektiğinde, bu özelliği kullanarak formül ayrıştırılırken bu parametreleri dizi modu olarak işaretleyebilirsiniz. Aksi takdirde kullanıcı, aynı sonucu elde etmek için bu özel işlevleri daha sonra [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-) ile güncellemelidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) |  |

### setLocaleDependent(boolean value) {#setLocaleDependent-boolean-}
```
public void setLocaleDependent(boolean value)
```


Formülün yerel ayarlara göre biçimlendirilip biçimlendirilmediği. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setParse(boolean value) {#setParse-boolean-}
```
public void setParse(boolean value)
```


Verilen formülün ayrıştırılıp ayrıştırılmayacağı. Varsayılan değer true'tur. False ise, verilen formül dizesi hücrede olduğu gibi tutulur ve kullanıcı başka yöntemlerle ayrıştırana kadar veya formül verileri diğer işlemler (örneğin formüllerin hesaplanması) için gerektiğinde ayrıştırılmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setR1C1Style(boolean value) {#setR1C1Style-boolean-}
```
public void setR1C1Style(boolean value)
```


Formülün R1C1 referans stilinde olup olmadığı. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

