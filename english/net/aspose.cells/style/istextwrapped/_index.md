---
title: Style.IsTextWrapped
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets a value indicating whether the text within a cell is wrapped
type: docs
url: /net/aspose.cells/style/istextwrapped/
---
## Style.IsTextWrapped property

Gets or sets a value indicating whether the text within a cell is wrapped.

```csharp
public bool IsTextWrapped { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(B3Style.IsTextWrapped);
[Test]
        public void Property_IsTextWrapped() 
        {
            string path = Constants.sourcePath + "CELLSNET-55186/";
            Workbook wb = new Workbook(path + "Template.xlsx");
            wb.ImportXml(path + "xml.xml", wb.Worksheets[0].Name, 1, 1);

            Cell B2Cell = wb.Worksheets[0].Cells["B2"];
            Style B2Style = B2Cell.GetStyle();
            Assert.IsTrue(B2Style.IsTextWrapped);
            Regex newLineRegex = new Regex(@"\n");
            Assert.GreaterOrEqual(newLineRegex.Matches(B2Cell.StringValue).Count, 2);

            Cell B3Cell = wb.Worksheets[0].Cells["B3"];
            Style B3Style = B3Cell.GetStyle();
            Assert.IsTrue(B3Style.IsTextWrapped);
            Assert.GreaterOrEqual(newLineRegex.Matches(B3Cell.StringValue).Count, 11);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


