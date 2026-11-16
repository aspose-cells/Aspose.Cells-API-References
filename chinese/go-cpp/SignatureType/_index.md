---
title: "SignatureType 枚举"
linktitle: "SignatureType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SignatureType 枚举。封装在 Go 中表示 signaturetype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/signaturetype/
---

## SignatureType Enum

指定签名类型。

```go

type SignatureType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Default](./default/) | 默认值，对应的 ProviderId 值固定为 {0000000000-0000-0000-0000-0000000000}。 |
| [Stamp](./stamp/) | 对应的 ProviderId 值通常为 {000CD6A4-0000-0000-C000-000000000046}。 |
| [Custom](./custom/) | 对应的 ProviderId 值通常需要用户设置。应从随提供程序提供的文档中获取。 |
