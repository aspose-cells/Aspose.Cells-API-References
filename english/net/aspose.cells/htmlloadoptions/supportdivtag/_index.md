---
title: HtmlLoadOptions.SupportDivTag
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions property. Indicates whether support the layout of div tag when the html file contains it. The default value is false
type: docs
url: /net/aspose.cells/htmlloadoptions/supportdivtag/
---
## HtmlLoadOptions.SupportDivTag property

Indicates whether support the layout of `<div>` tag when the html file contains it. The default value is false.

```csharp
public bool SupportDivTag { get; set; }
```

### Examples

```csharp
// Called: htmlLoadOptions.SupportDivTag = true;
[Test]
        public void Property_SupportDivTag()
        {
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions(LoadFormat.Html);
            htmlLoadOptions.AutoFitColsAndRows = true;
            htmlLoadOptions.ConvertNumericData = false;
            htmlLoadOptions.SupportDivTag = true;

            Workbook wb = new Workbook(Constants.HtmlPath + "CELLSJAVA-44496.html", htmlLoadOptions);
            wb.Save(Constants.destPath + "JAVA44496.xlsx");
            Cell cell = wb.Worksheets[0].Cells["A1"];
            Assert.AreEqual("Sample caption", cell.StringValue);
            Assert.IsTrue(cell.GetStyle().Font.IsBold);
        }
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


