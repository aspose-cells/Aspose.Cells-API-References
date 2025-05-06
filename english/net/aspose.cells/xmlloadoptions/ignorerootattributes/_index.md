---
title: XmlLoadOptions.IgnoreRootAttributes
second_title: Aspose.Cells for .NET API Reference
description: XmlLoadOptions property. Indicates whether ignore attributes of the root element
type: docs
url: /net/aspose.cells/xmlloadoptions/ignorerootattributes/
---
## XmlLoadOptions.IgnoreRootAttributes property

Indicates whether ignore attributes of the root element.

```csharp
public bool IgnoreRootAttributes { get; set; }
```

### Examples

```csharp
// Called: options.IgnoreRootAttributes = true;
[Test]
        public void Property_IgnoreRootAttributes()
        {
            XmlLoadOptions options = new XmlLoadOptions();
            options.IgnoreRootAttributes = true;
            Workbook lc_WorkBook = new Aspose.Cells.Workbook(Constants.sourcePath + &quot;CELLSNET53551.xml&quot;, options);
            Assert.AreEqual(&quot;Capital subscris varsat&quot;, lc_WorkBook.Worksheets[0].Cells[&quot;AH8&quot;].StringValue);
            lc_WorkBook.Save(Constants.destPath + &quot;CELLSNET53551.xlsx&quot;);
        }
```

### See Also

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


