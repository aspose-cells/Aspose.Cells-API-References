---
title: GridJsWorkbook.InsertImage
second_title: Aspose.Cells for .NET API Reference
description: GridJsWorkbook method. insert image in the worksheet
type: docs
url: /net/aspose.cells.gridjs/gridjsworkbook/insertimage/
---
## GridJsWorkbook.InsertImage method

insert image in the worksheet

```csharp
public string InsertImage(string uid, string p, Stream s, string imageUrl)
```

| Parameter | Type | Description |
| --- | --- | --- |
| uid | String | the unique id for the sheet file |
| p | String | specify the cell location ,json parameter contains sheet name,upper left row,upper left column for the image，etc {name:'sheet1',ri:1,ci:1} |
| s | Stream | stream of the image file |
| imageUrl | String | the url of the image file,if the imageUrl is null, will save the image in cache,otherwise will not save the image |

### Return Value

the json of the image

### See Also

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


