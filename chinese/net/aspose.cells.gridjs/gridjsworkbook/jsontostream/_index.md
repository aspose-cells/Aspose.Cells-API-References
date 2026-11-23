---
title: "GridJsWorkbook.JsonToStream"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GridJsWorkbook 方法。生成 JSON 从内存中的工作簿并写入指定的流。可选地缓存生成的 JSON，以加快后续检索。与 JsonToStreamByUid 的关键区别：此方法使用当前内存中的工作簿状态 wb 字段；JsonToStreamByUid 会从磁盘上的 .cells 缓存文件重新加载工作簿。当您想在修改后导出当前工作簿状态时使用此方法；当需要从先前缓存的文件状态重新生成 JSON 时使用 JsonToStreamByUid。缓存行为（提供 uid 时）：在生成前检查 JSON 缓存（L1 内存，L2 磁盘）；如果缓存未命中，则从内存工作簿生成 JSON；将生成的 JSON 存入缓存以供未来请求。"
type: docs
url: /zh/net/aspose.cells.gridjs/gridjsworkbook/jsontostream/
---
## GridJsWorkbook.JsonToStream method

从内存中的工作簿生成 JSON 并写入指定的流。可选地缓存生成的 JSON，以加快后续检索。与 JsonToStreamByUid 的关键区别：- 此方法使用当前内存中的工作簿状态（wb 字段） - JsonToStreamByUid 从磁盘上的 .cells 缓存文件重新加载工作簿 - 当您想在修改后导出当前工作簿状态时使用此方法 - 当需要从先前缓存的文件状态重新生成 JSON 时使用 JsonToStreamByUid 缓存行为（提供 uid 时）：- 在生成前检查 JSON 缓存（L1 内存 + L2 磁盘） - 如果缓存未命中，则从内存工作簿生成 JSON - 将生成的 JSON 存入缓存以供未来请求

```csharp
public void JsonToStream(Stream stream, string filename, string uid = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 用于写入 JSON 数据的输出流 |
| 文件名 | String | 在 JSON 中指定文件名。如果设置为 null，默认文件名为：book1。 |
| uid | String | 可选的 JSON 缓存唯一标识符。提供后，可启用缓存查找和存储。 |

### 另请参见

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


