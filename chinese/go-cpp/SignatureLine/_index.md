---
title: "SignatureLine 类"
linktitle: "SignatureLine"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SignatureLine 类。封装在 Go 中表示 signatureline 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/signatureline/
---

## SignatureLine class

表示签名线。

```go

type SignatureLine struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewSignatureLine](./newsignatureline/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetId](./getid/) | 获取或设置此签名行的标识符。 |
| [SetId](./setid/) | 获取或设置此签名行的标识符。 |
| [GetProviderId](./getproviderid/) | 获取或设置签名提供者的 ID。 |
| [SetProviderId](./setproviderid/) | 获取或设置签名提供者的 ID。 |
| [GetSigner](./getsigner/) | 获取或设置签署人。 |
| [SetSigner](./setsigner/) | 获取或设置签署人。 |
| [GetTitle](./gettitle/) | 获取或设置歌手的标题。 |
| [SetTitle](./settitle/) | 获取或设置歌手的标题。 |
| [GetEmail](./getemail/) | 获取或设置歌手的电子邮件。 |
| [SetEmail](./setemail/) | 获取或设置歌手的电子邮件。 |
| [IsLine](./isline/) | 指示它是否为签名行。 |
| [SetIsLine](./setisline/) | 指示它是否为签名行。 |
| [GetAllowComments](./getallowcomments/) | 指示是否可以附加评论。 |
| [SetAllowComments](./setallowcomments/) | 指示是否可以附加评论。 |
| [GetShowSignedDate](./getshowsigneddate/) | 指示是否显示签署日期。 |
| [SetShowSignedDate](./setshowsigneddate/) | 指示是否显示签署日期。 |
| [GetInstructions](./getinstructions/) | 获取或设置签署时向用户显示的文本。 |
| [SetInstructions](./setinstructions/) | 获取或设置签署时向用户显示的文本。 |
| [GetSignatureLineType](./getsignaturelinetype/) | 获取或设置签名类型。Default - 当设置为默认值时，相应的 ProviderId 值固定为 {0000000000-0000-0000-0000-0000000000}。Stamp - 当值为 Stamp 时，相应的 ProviderId 值通常为 {000CD6A4-0000-0000-C000-000000000046}。Custom - 当值为 Custom 时，相应的 ProviderId 值通常需要用户设置。它应从随提供程序提供的文档中获取。 |
| [SetSignatureLineType](./setsignaturelinetype/) | 获取或设置签名类型。Default - 当设置为默认值时，相应的 ProviderId 值固定为 {0000000000-0000-0000-0000-0000000000}。Stamp - 当值为 Stamp 时，相应的 ProviderId 值通常为 {000CD6A4-0000-0000-C000-000000000046}。Custom - 当值为 Custom 时，相应的 ProviderId 值通常需要用户设置。它应从随提供程序提供的文档中获取。 |
