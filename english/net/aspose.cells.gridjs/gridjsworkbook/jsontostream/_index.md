---
title: GridJsWorkbook.JsonToStream
second_title: Aspose.Cells for .NET API Reference
description: GridJsWorkbook method. Generate JSON from the inmemory Workbook and write it to the specified stream. Optionally caches the generated JSON for faster subsequent retrieval. Key differences from JsonToStreamByUid  This method uses the current inmemory Workbook state wb field  JsonToStreamByUid reloads the Workbook from .cells cache files on disk  Use this method when you want to export the current workbook state after modifications  Use JsonToStreamByUid when you need to regenerate JSON from a previously cached file state Caching behavior when uid is provided  Checks JSON cache before generating L1 memory  L2 disk  If cache miss generates JSON from inmemory workbook  Stores generated JSON in cache for future requests
type: docs
url: /net/aspose.cells.gridjs/gridjsworkbook/jsontostream/
---
## GridJsWorkbook.JsonToStream method

Generate JSON from the in-memory Workbook and write it to the specified stream. Optionally caches the generated JSON for faster subsequent retrieval. Key differences from JsonToStreamByUid: - This method uses the current in-memory Workbook state (wb field) - JsonToStreamByUid reloads the Workbook from .cells cache files on disk - Use this method when you want to export the current workbook state after modifications - Use JsonToStreamByUid when you need to regenerate JSON from a previously cached file state Caching behavior (when uid is provided): - Checks JSON cache before generating (L1 memory + L2 disk) - If cache miss, generates JSON from in-memory workbook - Stores generated JSON in cache for future requests

```csharp
public void JsonToStream(Stream stream, string filename, string uid = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The output stream to write JSON data to |
| filename | String | Specifies the file name in the JSON. If set to null,the default filename is: book1. |
| uid | String | Optional unique identifier for JSON caching. When provided, enables cache lookup and storage. |

### See Also

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


