---
title: Enum TextOverflowType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.TextOverflowType enum. Represents the way the text vertical or horizontal overflow
type: docs
url: /net/aspose.cells.drawing/textoverflowtype/
---
## TextOverflowType enumeration

Represents the way the text vertical or horizontal overflow.

```csharp
public enum TextOverflowType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Clip | `0` | Pay attention to top and bottom barriers. Provide no indication that there is text which is not visible. |
| Ellipsis | `1` | Pay attention to top and bottom barriers. Use an ellipsis to denote that there is text which is not visible. Only for vertical overflow. |
| Overflow | `2` | Overflow the text and pay no attention to top and bottom barriers. |

### Examples

```csharp
// Called: textBox.TextVerticalOverflow = TextOverflowType.Clip;
// http://www.aspose.com/community/forums/thread/251886.aspx
public void Drawing_Type_TextOverflowType()
{
    Console.WriteLine("Drawing_Type_TextOverflowType()");
    string infn = path + "Test_TxoTextOverflowType.xlsx";
    string outfn = Constants.destPath + "Test_TxoTextOverflowType_out.xlsx";

    Workbook book = new Workbook(infn);
    Worksheet sheet = book.Worksheets[0];
    Aspose.Cells.Charts.Chart chart = book.Worksheets[1].Charts[0];
    Aspose.Cells.Drawing.TextBox textBox = (Aspose.Cells.Drawing.TextBox)chart.Shapes[0];
    textBox.TextBody.TextAlignment.AutoSize = false;
    textBox.Text = "This is a long text";
    textBox.TextVerticalOverflow = TextOverflowType.Clip;
    book.Save(outfn);
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


