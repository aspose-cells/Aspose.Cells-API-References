---
title: Font.Size
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets the size of the font
type: docs
url: /net/aspose.cells/font/size/
---
## Font.Size property

Gets or sets the size of the font.

```csharp
public int Size { get; set; }
```

### Examples

```csharp
// Called: style.Font.Size = 8;
[Test]
        public void Property_Size()
        {
            Workbook wb = new Workbook();
            string strText = &quot;Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. &quot;;
   // strText += vbLf &amp; vbLf
            strText += &quot;Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.&quot;;

            Worksheet ws = wb.Worksheets[&quot;Sheet1&quot;];
            Cells cells = ws.Cells;
            Cell cell = cells[0, 0];
            cell.PutValue(strText);
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            style.Font.Size = 8;
            style.VerticalAlignment = Aspose.Cells.TextAlignmentType.Bottom;
            cell.SetStyle(style);

           ws.Cells.SetColumnWidth(0, 50);
           ws.AutoFitRows();
           wb.Save(Constants.destPath + &quot;Test_159487_1.xls&quot;);

            Assert.AreEqual(cells.GetRowHeight(0), 78.75, 0.01);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


