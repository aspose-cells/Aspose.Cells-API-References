---
title: "IGridJsService.AddImage"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "IGridJsService 方法。执行从本地文件添加图像的操作，直接使用图像字节"
type: docs
url: /zh/net/aspose.cells.gridjs/igridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

执行从本地文件添加图像的操作，直接使用图像字节。

```csharp
public string AddImage(string p, string uid, string iscontrol, byte[] fileBytes)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| p | String | JSON 字符串参数 |
| uid | String | 文件缓存的唯一 ID。 |
| iscontrol | String | 指定它是否为控件。 |
| fileBytes | Byte[] | 图像文件的原始字节 |

### 返回值

JSON 字符串结果

### 另请参见

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

执行从本地文件添加图像的操作，使用上传的表单文件。

```csharp
public string AddImage(string p, string uid, string iscontrol, IFormFileCollection files)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| p | String | JSON 字符串参数 |
| uid | String | 文件缓存的唯一 ID。 |
| iscontrol | String | 指定它是否为控件。 |
| files | IFormFileCollection | 图像的表单文件 |

### 返回值

JSON 字符串结果

### 另请参见

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


