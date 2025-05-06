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
// Called: oleObject.TextVerticalOverflow = TextOverflowType.Overflow;
public static void Type_TextOverflowType()
        {
            // Instantiate a new Workbook.
            Workbook workbook = new Workbook();
            // Get the first worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            // Define a string variable to store the image path.
            string imageUrl = &quot;OleObjectExample.jpg&quot;;
            // Get the picture into the streams.
            FileStream fs = new FileStream(imageUrl, FileMode.Open);
            // Define a byte array.
            byte[] imageData = new byte[fs.Length];
            // Obtain the picture into the array of bytes from streams.
            fs.Read(imageData, 0, imageData.Length);
            // Close the stream.
            fs.Close();

            // Get an excel file path in a variable.
            string path = &quot;OleObjectExample.xls&quot;;
            // Get the file into the streams.
            fs = new FileStream(path, FileMode.Open);
            // Define an array of bytes.
            byte[] objectData = new byte[fs.Length];
            // Store the file from streams.
            fs.Read(objectData, 0, objectData.Length);
            // Close the stream.
            fs.Close();

            // Add an Ole object into the worksheet with the image shown in MS Excel.
            int oleObjectIndex = sheet.OleObjects.Add(14, 3, 200, 220, imageData);
            OleObject oleObject = sheet.OleObjects[oleObjectIndex];
            // Set embedded ole object data.
            oleObject.ObjectData = objectData;

            // Setting properties
            oleObject.IsAutoSize = true;
            oleObject.IsLink = false;
            oleObject.DisplayAsIcon = true;
            oleObject.ImageSourceFullName = &quot;OleObjectExample.jpg&quot;;
            oleObject.ProgID = &quot;Excel.Sheet.8&quot;;
            oleObject.FileFormatType = FileFormatType.Excel97To2003;
            oleObject.ObjectSourceFullName = &quot;OleObjectExample.xls&quot;;
            oleObject.Label = &quot;Embedded Excel File&quot;;
            oleObject.SourceFullName = &quot;OleObjectExample.xls&quot;;
            oleObject.AutoUpdate = false;
            oleObject.AutoLoad = true;
            oleObject.MacroName = &quot;DoWork()&quot;;
            oleObject.ZOrderPosition = 3;
            oleObject.Name = &quot;OleObject1&quot;;
            oleObject.AlternativeText = &quot;Embedded Excel File&quot;;
            oleObject.Title = &quot;Embedded Excel File&quot;;
            oleObject.SoftEdges = 0.5d;
            oleObject.IsHidden = false;
            oleObject.IsLockAspectRatio = true;
            oleObject.RotationAngle = 45;
            oleObject.IsPrintable = true;
            oleObject.AutoShapeType = AutoShapeType.Rectangle;
            oleObject.AnchorType = ShapeAnchorType.TwoCellAnchor;
            oleObject.Placement = PlacementType.MoveAndSize;
            oleObject.UpperLeftRow = 14;
            oleObject.UpperLeftColumn = 3;
            oleObject.LowerRightRow = 20;
            oleObject.LowerRightColumn = 10;
            oleObject.Width = 200;
            oleObject.Height = 220;
            oleObject.Left = 50;
            oleObject.Top = 50;
            oleObject.WidthScale = 100;
            oleObject.HeightScale = 100;
            oleObject.RelativeToOriginalPictureSize = true;
            oleObject.LinkedCell = &quot;A1&quot;;
            oleObject.InputRange = &quot;A1:A10&quot;;
            oleObject.TextShapeType = AutoShapeType.Rectangle;
            oleObject.Text = &quot;This is a test.&quot;;
            oleObject.HtmlText = &quot;&lt;Font Style=&apos;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;&apos;&gt;This is a &lt;b&gt;test&lt;/b&gt;.&lt;/Font&gt;&quot;;
            oleObject.TextVerticalOverflow = TextOverflowType.Overflow;
            oleObject.TextHorizontalOverflow = TextOverflowType.Overflow;
            oleObject.IsTextWrapped = true;
            oleObject.TextOrientationType = TextOrientationType.TopToBottom;
            oleObject.TextHorizontalAlignment = TextAlignmentType.Center;
            oleObject.TextVerticalAlignment = TextAlignmentType.Center;
            oleObject.TextDirection = TextDirectionType.LeftToRight;

            // Save the excel file
            workbook.Save(&quot;OleObjectExample.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


