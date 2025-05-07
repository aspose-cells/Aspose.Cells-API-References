---
title: OleObject.AutoUpdate
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Specifies whether the link to the OleObject is automatically updated or not
type: docs
url: /net/aspose.cells.drawing/oleobject/autoupdate/
---
## OleObject.AutoUpdate property

Specifies whether the link to the OleObject is automatically updated or not.

```csharp
public bool AutoUpdate { get; set; }
```

### Examples

```csharp
// Called: oleObject.AutoUpdate = false;
public static void Property_AutoUpdate()
        {
            // Instantiate a new Workbook.
            Workbook workbook = new Workbook();
            // Get the first worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            // Define a string variable to store the image path.
            string imageUrl = "OleObjectExample.jpg";
            // Get the picture into the streams.
            FileStream fs = new FileStream(imageUrl, FileMode.Open);
            // Define a byte array.
            byte[] imageData = new byte[fs.Length];
            // Obtain the picture into the array of bytes from streams.
            fs.Read(imageData, 0, imageData.Length);
            // Close the stream.
            fs.Close();

            // Get an excel file path in a variable.
            string path = "OleObjectExample.xls";
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
            oleObject.ImageSourceFullName = "OleObjectExample.jpg";
            oleObject.ProgID = "Excel.Sheet.8";
            oleObject.FileFormatType = FileFormatType.Excel97To2003;
            oleObject.ObjectSourceFullName = "OleObjectExample.xls";
            oleObject.Label = "Embedded Excel File";
            oleObject.SourceFullName = "OleObjectExample.xls";
            oleObject.AutoUpdate = false;
            oleObject.AutoLoad = true;
            oleObject.MacroName = "DoWork()";
            oleObject.ZOrderPosition = 3;
            oleObject.Name = "OleObject1";
            oleObject.AlternativeText = "Embedded Excel File";
            oleObject.Title = "Embedded Excel File";
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
            oleObject.LinkedCell = "A1";
            oleObject.InputRange = "A1:A10";
            oleObject.TextShapeType = AutoShapeType.Rectangle;
            oleObject.Text = "This is a test.";
            oleObject.HtmlText = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            oleObject.TextVerticalOverflow = TextOverflowType.Overflow;
            oleObject.TextHorizontalOverflow = TextOverflowType.Overflow;
            oleObject.IsTextWrapped = true;
            oleObject.TextOrientationType = TextOrientationType.TopToBottom;
            oleObject.TextHorizontalAlignment = TextAlignmentType.Center;
            oleObject.TextVerticalAlignment = TextAlignmentType.Center;
            oleObject.TextDirection = TextDirectionType.LeftToRight;

            // Save the excel file
            workbook.Save("OleObjectExample.xlsx");
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


