---
title: Style.ParentStyle
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets the parent style of this style
type: docs
url: /net/aspose.cells/style/parentstyle/
---
## Style.ParentStyle property

Gets the parent style of this style.

```csharp
public Style ParentStyle { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(style.ParentStyle.Name, &amp;quot;Hyperlink&amp;quot;);
[Test]
        public void Property_ParentStyle()
        {
            //Instantiate a new Workbook object. 
            Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook();
            //Get the First sheet. 
            Aspose.Cells.Worksheet worksheet = workbook.Worksheets[0];

            //Define A1 Cell. 
            Aspose.Cells.Cell cell = worksheet.Cells[&quot;A1&quot;];
            //Add a hyperlink to it. 
            int index = worksheet.Hyperlinks.Add(&quot;A1&quot;, 1, 1, &quot;http://www.aspose.com/&quot;);
            worksheet.Hyperlinks[index].TextToDisplay = &quot;Aspose Site!&quot;;
            worksheet.Hyperlinks[index].ScreenTip = &quot;Click to go to Aspose site&quot;;

            Style style = cell.GetStyle();
            Assert.AreEqual(style.ParentStyle.Name, &quot;Hyperlink&quot;);
            //Save the excel file. 
            workbook.Save(Constants.destPath + &quot;CELLSNET45008.xlsx&quot;);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


