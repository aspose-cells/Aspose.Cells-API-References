---
title: "SetExcludeUnusedStyles 方法"
linktitle: "SetExcludeUnusedStyles"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SetExcludeUnusedStyles 方法。封装了在 Go 中表示 setexcludeunusedstyles 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/ebooksaveoptions/setexcludeunusedstyles/
---

## SetExcludeUnusedStyles function

指示是否排除未使用的样式。对于生成的 html 文件，排除未使用的样式可以在不影响视觉效果的情况下减小文件大小。因此此属性的默认值为 true。如果用户需要在工作簿中保留所有样式以用于生成的 html（例如用户稍后需要从生成的 html 恢复工作簿的场景），请将此属性设为 false。

```go

func (instance *EbookSaveOptions) SetExcludeUnusedStyles(value bool)  error

```

## 备注


## 另请参阅

* Class [EbookSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
