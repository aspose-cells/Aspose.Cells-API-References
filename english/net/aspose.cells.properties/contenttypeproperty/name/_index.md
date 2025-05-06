---
title: ContentTypeProperty.Name
second_title: Aspose.Cells for .NET API Reference
description: ContentTypeProperty property. Returns or sets the name of the object
type: docs
url: /net/aspose.cells.properties/contenttypeproperty/name/
---
## ContentTypeProperty.Name property

Returns or sets the name of the object.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.ContentTypeProperties[0].Name, &amp;quot;ss&amp;quot;);
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook();
            workbook.ContentTypeProperties.Add(&quot;ss&quot;, &quot;bb&quot;, &quot;text&quot;);
            workbook.Save(Constants.destPath + &quot;Cellsnet43279.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Cellsnet43279.xls&quot;);
            Assert.AreEqual(workbook.ContentTypeProperties[0].Name, &quot;ss&quot;);
            workbook.Save(Constants.destPath + &quot;Cellsnet43279.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;Cellsnet43279.xlsx&quot;);
            Assert.AreEqual(workbook.ContentTypeProperties[0].Name, &quot;ss&quot;);
        }
```

### See Also

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


