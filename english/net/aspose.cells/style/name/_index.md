---
title: Style.Name
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets the name of the style
type: docs
url: /net/aspose.cells/style/name/
---
## Style.Name property

Gets or sets the name of the style.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: style.Name = (&amp;quot;Style1&amp;quot;);
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Style style = workbook.CreateStyle();
            style.Font.Color = (Color.Red);
            style.Name = (&quot;Style1&quot;);
            StyleFlag flag = new StyleFlag();
            flag.All = (true);
            Cells mycells = sheet.Cells;
            Cell mycell = mycells[&quot;A1&quot;];
            mycell.PutValue(&quot;Tekst&quot;);
            mycell.SetStyle(style, flag);
            //Saving the Excel file 
            workbook.Save(Constants.destPath + &quot;CELLSJAVA41659.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSJAVA41659.xlsx&quot;);
            style = workbook.Worksheets[0].Cells[&quot;A1&quot;].GetStyle();
            Assert.AreEqual(style.ParentStyle.Name, &quot;Style1&quot;);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


