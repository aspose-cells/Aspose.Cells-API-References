---
title: "PdfSecurityOptions 类"
linktitle: "PdfSecurityOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PdfSecurityOptions 类。封装了在 Go 中表示 pdfsecurityoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pdfsecurityoptions/
---

## PdfSecurityOptions class

PDF 文档的加密和访问权限选项。PDF/A 不允许安全设置。

```go

type PdfSecurityOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewPdfSecurityOptions](./newpdfsecurityoptions/) | PdfSecurityOptions 的构造函数 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetUserPassword](./getuserpassword/) | 获取或设置打开加密 PDF 文档所需的用户密码。 |
| [SetUserPassword](./setuserpassword/) | 获取或设置打开加密 PDF 文档所需的用户密码。 |
| [GetOwnerPassword](./getownerpassword/) | 获取或设置加密 PDF 文档的所有者密码。 |
| [SetOwnerPassword](./setownerpassword/) | 获取或设置加密 PDF 文档的所有者密码。 |
| [GetPrintPermission](./getprintpermission/) | 指示是否允许打印文档。 |
| [SetPrintPermission](./setprintpermission/) | 指示是否允许打印文档。 |
| [GetModifyDocumentPermission](./getmodifydocumentpermission/) | 指示是否允许通过除 AnnotationsPermission、FillFormsPermission 和 AssembleDocumentPermission 控制之外的操作来修改文档内容。 |
| [SetModifyDocumentPermission](./setmodifydocumentpermission/) | 指示是否允许通过除 AnnotationsPermission、FillFormsPermission 和 AssembleDocumentPermission 控制之外的操作来修改文档内容。 |
| [GetAnnotationsPermission](./getannotationspermission/) | 指示是否允许添加或修改文本批注，填写交互式表单字段。 |
| [SetAnnotationsPermission](./setannotationspermission/) | 指示是否允许添加或修改文本批注，填写交互式表单字段。 |
| [GetFillFormsPermission](./getfillformspermission/) | 指示是否允许填写已有的交互式表单字段（包括签名字段），即使 ModifyDocumentPermission 已被清除。 |
| [SetFillFormsPermission](./setfillformspermission/) | 指示是否允许填写已有的交互式表单字段（包括签名字段），即使 ModifyDocumentPermission 已被清除。 |
| [GetExtractContentPermission](./getextractcontentpermission/) | 指示是否允许通过除 AccessibilityExtractContent 控制之外的操作复制或以其他方式提取文档中的文本和图形。 |
| [SetExtractContentPermission](./setextractcontentpermission/) | 指示是否允许通过除 AccessibilityExtractContent 控制之外的操作复制或以其他方式提取文档中的文本和图形。 |
| [GetAccessibilityExtractContent](./getaccessibilityextractcontent/) | 指示是否允许提取文本和图形（以支持残障用户的可访问性或出于其他目的）。 |
| [SetAccessibilityExtractContent](./setaccessibilityextractcontent/) | 指示是否允许提取文本和图形（以支持残障用户的可访问性或出于其他目的）。 |
| [GetAssembleDocumentPermission](./getassembledocumentpermission/) | 指示是否允许组装文档（插入、旋转或删除页面并创建书签或缩略图），即使 ModifyDocumentPermission 已被清除。 |
| [SetAssembleDocumentPermission](./setassembledocumentpermission/) | 指示是否允许组装文档（插入、旋转或删除页面并创建书签或缩略图），即使 ModifyDocumentPermission 已被清除。 |
| [GetFullQualityPrintPermission](./getfullqualityprintpermission/) | 指示是否允许将文档打印为一种表示形式，以便可以生成 PDF 内容的忠实数字副本。 |
| [SetFullQualityPrintPermission](./setfullqualityprintpermission/) | 指示是否允许将文档打印为一种表示形式，以便可以生成 PDF 内容的忠实数字副本。 |
