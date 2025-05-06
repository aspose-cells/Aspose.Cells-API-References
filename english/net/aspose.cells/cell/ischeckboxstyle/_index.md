---
title: Cell.IsCheckBoxStyle
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether setting this cell as a check box
type: docs
url: /net/aspose.cells/cell/ischeckboxstyle/
---
## Cell.IsCheckBoxStyle property

Indicates whether setting this cell as a check box.

```csharp
public bool IsCheckBoxStyle { get; set; }
```

### Examples

```csharp
// Called: wb.Worksheets[0].Cells[&amp;quot;C12&amp;quot;].IsCheckBoxStyle = true;
[Test]
        public void Property_IsCheckBoxStyle()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSNET-56445.xlsx&quot;);
            wb.Save(_destFilesPath + &quot;CELLSNET-56445.html&quot;, new HtmlSaveOptions()); 
            wb = new Workbook(_destFilesPath + &quot;CELLSNET-56445.html&quot;);
            wb.Worksheets[0].Cells[&quot;C12&quot;].IsCheckBoxStyle = true;
            wb.Worksheets[0].Cells[&quot;F12&quot;].Value = true;
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


