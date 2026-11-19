---
title: "VbaProject"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 VBA 项目。"
type: docs
url: /zh/java/com.aspose.cells/vbaproject/
---

**Inheritance:**
java.lang.Object
```
public class VbaProject
```

表示 VBA 项目。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [copy(VbaProject source)](#copy-com.aspose.cells.VbaProject-) | 从其他文件复制 VBA 项目。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertRawData()](#getCertRawData--) | 如果此 VBA 项目已签名，则获取证书原始数据。 |
| [getClass()](#getClass--) |  |
| [getEncoding()](#getEncoding--) | 获取 VBA 项目的编码。 |
| [getIslockedForViewing()](#getIslockedForViewing--) | 指示此 VBA 项目是否已锁定以供查看。 |
| [getModules()](#getModules--) | 获取所有 [VbaModule](../../com.aspose.cells/vbamodule) 对象。 |
| [getName()](#getName--) | 获取 VBA 项目的名称。 |
| [getReferences()](#getReferences--) | 获取 VBA 项目的所有引用。 |
| [hashCode()](#hashCode--) |  |
| [isLockedForView()](#isLockedForView--) | 指示此 VBA 项目是否已锁定以供查看。 |
| [isProtected()](#isProtected--) | 指示此 VBA 项目是否受保护。 |
| [isSigned()](#isSigned--) | 指示 VBA 代码是否已签名。 |
| [isValidSigned()](#isValidSigned--) | 指示 VBA 项目的签名是否有效。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(boolean islockedForViewing, String password)](#protect-boolean-java.lang.String-) | 保护或取消保护此 VBA 项目。 |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | 设置 VBA 项目的编码。 |
| [setName(String value)](#setName-java.lang.String-) | 设置 VBA 项目的名称。 |
| [sign(DigitalSignature digitalSignature)](#sign-com.aspose.cells.DigitalSignature-) | 使用数字签名对该 VBA 项目进行签名 |
| [toString()](#toString--) |  |
| [validatePassword(String password)](#validatePassword-java.lang.String-) | 验证保护密码。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProject source) {#copy-com.aspose.cells.VbaProject-}
```
public void copy(VbaProject source)
```


从其他文件复制 VBA 项目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [VbaProject](../../com.aspose.cells/vbaproject) |  |

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
### getCertRawData() {#getCertRawData--}
```
public byte[] getCertRawData()
```


如果此 VBA 项目已签名，则获取证书原始数据。

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


获取 VBA 项目的编码。

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getIslockedForViewing() {#getIslockedForViewing--}
```
public boolean getIslockedForViewing()
```


指示此 VBA 项目是否已锁定以供查看。

**Remarks**

注意：此成员现已过时。请改用 VbaProject.IsLockedForView 属性。自 2026 年 7 月起，此属性将在 12 个月后移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
boolean
### getModules() {#getModules--}
```
public VbaModuleCollection getModules()
```


获取所有 [VbaModule](../../com.aspose.cells/vbamodule) 对象。

**Returns:**
[VbaModuleCollection](../../com.aspose.cells/vbamodulecollection)
### getName() {#getName--}
```
public String getName()
```


获取 VBA 项目的名称。

**Returns:**
java.lang.String
### getReferences() {#getReferences--}
```
public VbaProjectReferenceCollection getReferences()
```


获取 VBA 项目的所有引用。

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


指示此 VBA 项目是否已锁定以供查看。如果为 true，代码将不可见。

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


指示此 VBA 项目是否受保护。

**Returns:**
boolean
### isSigned() {#isSigned--}
```
public boolean isSigned()
```


指示 VBA 代码是否已签名。

**Returns:**
boolean
### isValidSigned() {#isValidSigned--}
```
public boolean isValidSigned()
```


指示 VBA 项目的签名是否有效。

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


保护或取消保护此 VBA 项目。

**Remarks**

如果 islockedForViewing 为 true，则密码不能为空。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| islockedForViewing | boolean | 指示是否锁定项目以供查看。 |
| 密码 | java.lang.String | 如果该值为 null，则取消保护此 VBA 项目；否则保护此 VBA 项目。 |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


设置 VBA 项目的编码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置 VBA 项目的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### sign(DigitalSignature digitalSignature) {#sign-com.aspose.cells.DigitalSignature-}
```
public void sign(DigitalSignature digitalSignature)
```


使用数字签名对该 VBA 项目进行签名

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../../com.aspose.cells/digitalsignature) | 数字签名 |

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


验证保护密码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 密码 | java.lang.String | 密码 |

**Returns:**
布尔值 - 密码是否为此 VBA 项目的保护密码
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

