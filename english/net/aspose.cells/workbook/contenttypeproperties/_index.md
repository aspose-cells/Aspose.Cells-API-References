---
title: Workbook.ContentTypeProperties
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the list of ContentTypeProperty objects in the workbook
type: docs
url: /net/aspose.cells/workbook/contenttypeproperties/
---
## Workbook.ContentTypeProperties property

Gets the list of [`ContentTypeProperty`](../../../aspose.cells.properties/contenttypeproperty/) objects in the workbook.

```csharp
public ContentTypePropertyCollection ContentTypeProperties { get; }
```

### Examples

```csharp
// Called: workbook.ContentTypeProperties[index].IsNillable = true;
public void Workbook_Property_ContentTypeProperties()
{
    Workbook workbook = new Workbook(FileFormatType.Xlsx);
    int index = workbook.ContentTypeProperties.Add("MK31", "Simple Data");
    workbook.ContentTypeProperties[index].IsNillable = true;
    //index= workbook.ContentTypeProperties.Add("MK32", "2019-10-17T16:00:00+00:00", "DateTime");
    index = workbook.ContentTypeProperties.Add("MK32",
        DateTime.Now.ToString("yyyy-MM-dd'T'hh:mm:ss"), "DateTime");
    workbook.ContentTypeProperties[index].IsNillable = true;
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ContentTypePropertyCollection](../../../aspose.cells.properties/contenttypepropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


