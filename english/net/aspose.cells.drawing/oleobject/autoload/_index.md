---
title: OleObject.AutoLoad
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Specifies whether the host application for the embedded object shall be called to load the object data automatically when the parent workbook is opened
type: docs
url: /net/aspose.cells.drawing/oleobject/autoload/
---
## OleObject.AutoLoad property

Specifies whether the host application for the embedded object shall be called to load the object data automatically when the parent workbook is opened.

```csharp
public bool AutoLoad { get; set; }
```

### Examples

```csharp
// Called: workbook2.Worksheets[0].OleObjects[oleNumber].AutoLoad = true;
public void OleObject_Property_AutoLoad()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");

    int upperLeftRow = 0;
    int upperLeftColumn = 0;
    int height = 0;
    int width = 0;
    byte[] imageData = null;
    int x = 0;
    int y = 0;
    byte[] objData = null;
    string progID = "";
    string sourceFullName = "";
    FileFormatType fileFormatType = FileFormatType.Unknown;


    foreach (Worksheet sheet in workbook.Worksheets)
    {
        for (int i = sheet.OleObjects.Count - 1; i >= 0; --i)
        {
            OleObject frame = sheet.OleObjects[i];
            if (frame == null)
            {
                continue;
            }

            upperLeftRow = frame.UpperLeftRow;
            upperLeftColumn = frame.UpperLeftColumn;
            height = frame.Height;
            width = frame.Width;
            imageData = frame.ImageData;
            x = frame.X;
            y = frame.Y;
            objData = frame.ObjectData;
            progID = frame.ProgID;
            fileFormatType = frame.FileFormatType;
            sourceFullName = frame.ObjectSourceFullName;
            fileFormatType = frame.FileFormatType;
            sheet.OleObjects.RemoveAt(i);
        }
    }

    workbook.Save(Constants.destPath + "example.xls");
    Workbook workbook2 = new Workbook(Constants.destPath + "example.xls");
    int oleNumber = workbook2.Worksheets[0].OleObjects.Add(upperLeftRow, upperLeftColumn, height, width, imageData);
    workbook2.Worksheets[0].OleObjects[oleNumber].X = x;
    workbook2.Worksheets[0].OleObjects[oleNumber].Y = y;
    workbook2.Worksheets[0].OleObjects[oleNumber].ObjectData = objData;
    workbook2.Worksheets[0].OleObjects[oleNumber].ProgID = progID;
    workbook2.Worksheets[0].OleObjects[oleNumber].FileFormatType = fileFormatType;
    workbook2.Worksheets[0].OleObjects[oleNumber].ObjectSourceFullName = sourceFullName;

    var fillFormat = workbook2.Worksheets[0].OleObjects[oleNumber].FillFormat;
    fillFormat.ForeColor = Color.White;
    workbook2.Worksheets[0].OleObjects[oleNumber].AutoLoad = true;
    workbook2.Save(Constants.destPath + "example.xls"); 
}
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


