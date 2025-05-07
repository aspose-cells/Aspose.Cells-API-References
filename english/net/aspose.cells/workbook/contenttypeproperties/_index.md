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
// Called: ContentTypePropertyCollection ctps = wb.ContentTypeProperties;
[Test]
        public void Property_ContentTypeProperties()
        {
            Workbook wb = new Workbook(Constants.openPivottablePath + "mm.xlsx");
            ContentTypePropertyCollection ctps = wb.ContentTypeProperties;
            //ContentTypeProperty ctp = new ContentTypeProperty(ctps);
            //ctp.Name = "dddd";
            //ctp.Value = "gggg";
            ctps.Add("dddd", "gggg");
            wb.Save(Constants.savePivottablePath + "wangtao.xlsx");
            wb = new Workbook(Constants.openPivottablePath + "AfterUpload.xlsx");
            wb.Save(Constants.savePivottablePath + "40590.xlsx");
        }
```

### See Also

* class [ContentTypePropertyCollection](../../../aspose.cells.properties/contenttypepropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


