---
title: "DigitalSignature 类"
linktitle: "DigitalSignature"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DigitalSignature 类。封装在 Go 中表示数字签名的对象。"
type: docs
weight: 200
url: /zh/go-cpp/digitalsignature/
---

## DigitalSignature class

文件中的签名。

```go

type DigitalSignature struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewDigitalSignature_Stream_String_String_Date](./newdigitalsignature_stream_string_string_date/) | DigitalSignature 的构造函数。 |
| [NewDigitalSignature_String_String_String_Date](./newdigitalsignature_string_string_string_date/) | DigitalSignature 的构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetComments](./getcomments/) | 签名的目的。 |
| [SetComments](./setcomments/) | 签名的目的。 |
| [GetSignTime](./getsigntime/) | 文档签署的时间。 |
| [SetSignTime](./setsigntime/) | 文档签署的时间。 |
| [GetId](./getid/) | 指定一个 GUID，可与文档内容中存储的签名行的 GUID 交叉引用。默认值为空 GUID（全为零）。 |
| [SetId](./setid/) | 指定一个 GUID，可与文档内容中存储的签名行的 GUID 交叉引用。默认值为空 GUID（全为零）。 |
| [GetText](./gettext/) | 指定数字签名中实际签名的文本。默认值为空。 |
| [SetText](./settext/) | 指定数字签名中实际签名的文本。默认值为空。 |
| [GetImage](./getimage/) | 指定数字签名的图像。默认值为 null。 |
| [SetImage](./setimage/) | 指定数字签名的图像。默认值为 null。 |
| [GetProviderId](./getproviderid/) | 指定签名提供程序的类 ID。默认值为空 GUID（全为零）。 |
| [SetProviderId](./setproviderid/) | 指定签名提供程序的类 ID。默认值为空 GUID（全为零）。 |
| [IsValid](./isvalid/) | 如果此数字签名有效且文档未被篡改，则此值将为 true。 |
| [GetXAdESType](./getxadestype/) | XAdES 类型。默认值为 None（XAdES 已关闭）。 |
| [SetXAdESType](./setxadestype/) | XAdES 类型。默认值为 None（XAdES 已关闭）。 |
