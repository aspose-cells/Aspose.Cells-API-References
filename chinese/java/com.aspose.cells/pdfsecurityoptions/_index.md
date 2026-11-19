---
title: "PdfSecurityOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 PDF 文档的加密和访问权限选项。"
type: docs
url: /zh/java/com.aspose.cells/pdfsecurityoptions/
---

**Inheritance:**
java.lang.Object
```
public class PdfSecurityOptions
```

用于对 PDF 文档进行加密和访问权限设置的选项。PDF/A 不允许安全设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PdfSecurityOptions()](#PdfSecurityOptions--) | PdfSecurityOptions 的构造函数 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--) | 指示是否允许提取文本和图形（以支持残障用户的可访问性或用于其他目的）。 |
| [getAnnotationsPermission()](#getAnnotationsPermission--) | 指示是否允许添加或修改文本批注、填写交互式表单字段。 |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--) | 指示是否允许组装文档（插入、旋转或删除页面以及创建书签或缩略图），即使 [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) 已被清除。 |
| [getClass()](#getClass--) |  |
| [getExtractContentPermission()](#getExtractContentPermission--) | 指示是否允许通过除 [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--) 控制的操作之外的方式复制或提取文档中的文本和图形。 |
| [getExtractContentPermissionObsolete()](#getExtractContentPermissionObsolete--) | 根据 PDF 参考文献，此复制或提取内容的权限已废弃。 |
| [getFillFormsPermission()](#getFillFormsPermission--) | 指示是否允许填写现有的交互式表单字段（包括签名字段），即使 [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) 已被清除。 |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--) | 指示是否允许打印文档，以生成能够忠实再现 PDF 内容的数字副本。 |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--) | 指示是否允许通过除 [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--) 、 [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) 和 [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--) 控制的操作之外修改文档内容。 |
| [getOwnerPassword()](#getOwnerPassword--) | 获取加密 PDF 文档的所有者密码。 |
| [getPrintPermission()](#getPrintPermission--) | 指示是否允许打印文档。 |
| [getUserPassword()](#getUserPassword--) | 获取打开加密 PDF 文档所需的用户密码。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccessibilityExtractContent(boolean value)](#setAccessibilityExtractContent-boolean-) | 指示是否允许提取文本和图形（以支持残障用户的可访问性或用于其他目的）。 |
| [setAnnotationsPermission(boolean value)](#setAnnotationsPermission-boolean-) | 指示是否允许添加或修改文本批注、填写交互式表单字段。 |
| [setAssembleDocumentPermission(boolean value)](#setAssembleDocumentPermission-boolean-) | 指示是否允许组装文档（插入、旋转或删除页面以及创建书签或缩略图），即使 [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) 已被清除。 |
| [setExtractContentPermission(boolean value)](#setExtractContentPermission-boolean-) | 指示是否允许通过除 [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--) 控制的操作之外的方式复制或提取文档中的文本和图形。 |
| [setExtractContentPermissionObsolete(boolean value)](#setExtractContentPermissionObsolete-boolean-) | 根据 PDF 参考文献，此复制或提取内容的权限已废弃。 |
| [setFillFormsPermission(boolean value)](#setFillFormsPermission-boolean-) | 指示是否允许填写现有的交互式表单字段（包括签名字段），即使 [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) 已被清除。 |
| [setFullQualityPrintPermission(boolean value)](#setFullQualityPrintPermission-boolean-) | 指示是否允许打印文档，以生成能够忠实再现 PDF 内容的数字副本。 |
| [setModifyDocumentPermission(boolean value)](#setModifyDocumentPermission-boolean-) | 指示是否允许通过除 [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--) 、 [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) 和 [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--) 控制的操作之外修改文档内容。 |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | 设置加密 PDF 文档的所有者密码。 |
| [setPrintPermission(boolean value)](#setPrintPermission-boolean-) | 指示是否允许打印文档。 |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | 设置打开加密 PDF 文档所需的用户密码。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSecurityOptions() {#PdfSecurityOptions--}
```
public PdfSecurityOptions()
```


PdfSecurityOptions 的构造函数

**Example**

以下代码为输出 PDF 设置高分辨率打印权限。

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
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
### getAccessibilityExtractContent() {#getAccessibilityExtractContent--}
```
public boolean getAccessibilityExtractContent()
```


指示是否允许提取文本和图形（以支持残障用户的可访问性或用于其他目的）。

**Returns:**
boolean
### getAnnotationsPermission() {#getAnnotationsPermission--}
```
public boolean getAnnotationsPermission()
```


指示是否允许添加或修改文本批注、填写交互式表单字段。

**Remarks**

如果也设置了 [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) ，则创建或修改交互式表单字段（包括签名字段）。

**Returns:**
boolean
### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}
```
public boolean getAssembleDocumentPermission()
```


指示是否允许组装文档（插入、旋转或删除页面以及创建书签或缩略图），即使 [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) 已被清除。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExtractContentPermission() {#getExtractContentPermission--}
```
public boolean getExtractContentPermission()
```


指示是否允许通过除 [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--) 控制的操作之外的方式复制或提取文档中的文本和图形。

**Returns:**
boolean
### getExtractContentPermissionObsolete() {#getExtractContentPermissionObsolete--}
```
public boolean getExtractContentPermissionObsolete()
```


根据 PDF 参考文献，此复制或提取内容的权限已废弃。

**Remarks**

注意：此成员现已废弃。请改用 ExtractContentPermission 属性。该属性将在 2023 年 9 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getFillFormsPermission() {#getFillFormsPermission--}
```
public boolean getFillFormsPermission()
```


指示是否允许填写现有的交互式表单字段（包括签名字段），即使 [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) 已被清除。

**Returns:**
boolean
### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}
```
public boolean getFullQualityPrintPermission()
```


指示是否允许打印文档，以生成能够忠实再现 PDF 内容的数字副本。

**Remarks**

当它被清除（且已设置 [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--)）时，打印将限制为外观的低级表示，可能质量下降。

**Returns:**
boolean
### getModifyDocumentPermission() {#getModifyDocumentPermission--}
```
public boolean getModifyDocumentPermission()
```


指示是否允许通过除 [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--) 、 [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) 和 [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--) 控制的操作之外修改文档内容。

**Returns:**
boolean
### getOwnerPassword() {#getOwnerPassword--}
```
public String getOwnerPassword()
```


获取加密 PDF 文档的所有者密码。

**Remarks**

所有者密码允许用户在未指定任何访问限制的情况下打开加密的 PDF 文档。

**Returns:**
java.lang.String
### getPrintPermission() {#getPrintPermission--}
```
public boolean getPrintPermission()
```


指示是否允许打印文档。

**Remarks**

可能不是最高质量级别，取决于是否也设置了 [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--)。

**Returns:**
boolean
### getUserPassword() {#getUserPassword--}
```
public String getUserPassword()
```


获取打开加密 PDF 文档所需的用户密码。

**Remarks**

打开加密的 PDF 文档进行查看时，需要提供所有者密码或用户密码。

用户密码可以为 null 或空字符串，在这种情况下打开 PDF 文档时不需要用户提供密码。

使用正确的所有者密码打开文档可获得对文档的完全访问权限。

使用正确的用户密码打开文档（或打开没有用户密码的文档）可根据指定的权限获得有限访问。

**Returns:**
java.lang.String
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




### setAccessibilityExtractContent(boolean value) {#setAccessibilityExtractContent-boolean-}
```
public void setAccessibilityExtractContent(boolean value)
```


指示是否允许提取文本和图形（以支持残障用户的可访问性或用于其他目的）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAnnotationsPermission(boolean value) {#setAnnotationsPermission-boolean-}
```
public void setAnnotationsPermission(boolean value)
```


指示是否允许添加或修改文本批注、填写交互式表单字段。

**Remarks**

如果也设置了 [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) ，则创建或修改交互式表单字段（包括签名字段）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAssembleDocumentPermission(boolean value) {#setAssembleDocumentPermission-boolean-}
```
public void setAssembleDocumentPermission(boolean value)
```


指示是否允许组装文档（插入、旋转或删除页面以及创建书签或缩略图），即使 [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) 已被清除。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExtractContentPermission(boolean value) {#setExtractContentPermission-boolean-}
```
public void setExtractContentPermission(boolean value)
```


指示是否允许通过除 [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--) 控制的操作之外的方式复制或提取文档中的文本和图形。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExtractContentPermissionObsolete(boolean value) {#setExtractContentPermissionObsolete-boolean-}
```
public void setExtractContentPermissionObsolete(boolean value)
```


根据 PDF 参考文献，此复制或提取内容的权限已废弃。

**Remarks**

注意：此成员现已废弃。请改用 ExtractContentPermission 属性。该属性将在 2023 年 9 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFillFormsPermission(boolean value) {#setFillFormsPermission-boolean-}
```
public void setFillFormsPermission(boolean value)
```


指示是否允许填写现有的交互式表单字段（包括签名字段），即使 [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) 已被清除。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFullQualityPrintPermission(boolean value) {#setFullQualityPrintPermission-boolean-}
```
public void setFullQualityPrintPermission(boolean value)
```


指示是否允许打印文档，以生成能够忠实再现 PDF 内容的数字副本。

**Remarks**

当它被清除（且已设置 [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--)）时，打印将限制为外观的低级表示，可能质量下降。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setModifyDocumentPermission(boolean value) {#setModifyDocumentPermission-boolean-}
```
public void setModifyDocumentPermission(boolean value)
```


指示是否允许通过除 [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--) 、 [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) 和 [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--) 控制的操作之外修改文档内容。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public void setOwnerPassword(String value)
```


设置加密 PDF 文档的所有者密码。

**Remarks**

所有者密码允许用户在未指定任何访问限制的情况下打开加密的 PDF 文档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPrintPermission(boolean value) {#setPrintPermission-boolean-}
```
public void setPrintPermission(boolean value)
```


指示是否允许打印文档。

**Remarks**

可能不是最高质量级别，取决于是否也设置了 [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public void setUserPassword(String value)
```


设置打开加密 PDF 文档所需的用户密码。

**Remarks**

打开加密的 PDF 文档进行查看时，需要提供所有者密码或用户密码。

用户密码可以为 null 或空字符串，在这种情况下打开 PDF 文档时不需要用户提供密码。

使用正确的所有者密码打开文档可获得对文档的完全访问权限。

使用正确的用户密码打开文档（或打开没有用户密码的文档）可根据指定的权限获得有限访问。

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

