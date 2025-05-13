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
// Called: ctps.Add("dddd", "gggg");
public void ContentTypePropertyCollection_Method_Add()
{
    Workbook wb = new Workbook(Constants.openPivottablePath + "mm.xlsx");
    ContentTypePropertyCollection ctps = wb.ContentTypeProperties;
    //ContentTypeProperty ctp = new ContentTypeProperty(ctps);
    //ctp.Name = "dddd";
    //ctp.Value = "gggg";
    ctps.Add("dddd", "gggg");
    wb.Save(Constants.savePivottablePath + "wangtao.xlsx");
    wb = new Workbook(Constants.openPivottablePath + "AfterUpload.xlsx");
    wb.Save(Constants.savePivottablePath + "example.xlsx");
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
public void ContentTypePropertyCollection_Method_Add()
{
    Workbook workbook = new Workbook();
    workbook.ContentTypeProperties.Add("ss", "bb", "text");
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


