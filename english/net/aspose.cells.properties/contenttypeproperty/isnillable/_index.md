---
title: ContentTypeProperty.IsNillable
second_title: Aspose.Cells for .NET API Reference
description: ContentTypeProperty property. Indicates whether the value could be empty
type: docs
url: /net/aspose.cells.properties/contenttypeproperty/isnillable/
---
## ContentTypeProperty.IsNillable property

Indicates whether the value could be empty.

```csharp
public bool IsNillable { get; set; }
```

### Examples

```csharp
// Called: workbook.ContentTypeProperties[index].IsNillable = true;
[Test]
        public void Property_IsNillable()
        {
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            int index = workbook.ContentTypeProperties.Add("MK31", "Simple Data");
            workbook.ContentTypeProperties[index].IsNillable = true;
            //index= workbook.ContentTypeProperties.Add("MK32", "2019-10-17T16:00:00+00:00", "DateTime");
            index = workbook.ContentTypeProperties.Add("MK32",
                DateTime.Now.ToString("yyyy-MM-dd'T'hh:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index].IsNillable = true;
            workbook.Save(Constants.destPath + "CellsNet46903.xlsx");
        }
```

### See Also

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


