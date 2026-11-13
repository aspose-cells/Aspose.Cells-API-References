---
title: IGridJsService.AddImage
second_title: Aspose.Cells for .NET API Reference
description: IGridJsService method. Applies the add image from local file operation taking the image bytes directly
type: docs
url: /net/aspose.cells.gridjs/igridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Applies the add image from local file operation, taking the image bytes directly.

```csharp
public string AddImage(string p, string uid, string iscontrol, byte[] fileBytes)
```

| Parameter | Type | Description |
| --- | --- | --- |
| p | String | The JSON string parameter |
| uid | String | The unique id for the file cache. |
| iscontrol | String | Specify whether it is a control. |
| fileBytes | Byte[] | The raw bytes of the image file |

### Return Value

The JSON string result

### See Also

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Applies the add image from local file operation, taking the uploaded form files.

```csharp
public string AddImage(string p, string uid, string iscontrol, IFormFileCollection files)
```

| Parameter | Type | Description |
| --- | --- | --- |
| p | String | The JSON string parameter |
| uid | String | The unique id for the file cache. |
| iscontrol | String | Specify whether it is a control. |
| files | IFormFileCollection | The form file of the image |

### Return Value

The JSON string result

### See Also

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


