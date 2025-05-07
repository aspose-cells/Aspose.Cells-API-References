---
title: ContentTypePropertyCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ContentTypePropertyCollection method. Adds content type property information
type: docs
url: /net/aspose.cells.properties/contenttypepropertycollection/add/
---
## Add(string, string) {#add}

Adds content type property information.

```csharp
public int Add(string name, string value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the content type property. |
| value | String | The value of the content type property. |

### Examples

```csharp
// Called: int index = workbook.ContentTypeProperties.Add("MK31", "Simple Data");
[Test]
        public void Method_String_()
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

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_1}

Adds content type property information.

```csharp
public int Add(string name, string value, string type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the content type property. |
| value | String | The value of the content type property. |
| type | String | The type of the content type property. |

### Examples

```csharp
// Called: workbook.ContentTypeProperties.Add("ss", "bb", "text");
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            workbook.ContentTypeProperties.Add("ss", "bb", "text");
            workbook.Save(Constants.destPath + "CellsNet43276.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet43276.xlsx");
        }
```

### See Also

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


