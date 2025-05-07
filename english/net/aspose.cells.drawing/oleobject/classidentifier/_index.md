---
title: OleObject.ClassIdentifier
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Gets and sets the class identifier of the embedded object. It means which application opens the embedded file
type: docs
url: /net/aspose.cells.drawing/oleobject/classidentifier/
---
## OleObject.ClassIdentifier property

Gets and sets the class identifier of the embedded object. It means which application opens the embedded file.

```csharp
public byte[] ClassIdentifier { get; set; }
```

### Examples

```csharp
// Called: classId = frame.ClassIdentifier;
[Test]
          public void Property_ClassIdentifier()
          {

              Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET44708.xls");

              int upperLeftRow = 0;
              int upperLeftColumn = 0;
              int height = 0;
              int width = 0;
              byte[] imageData = null;
              int x = 0;
              int y = 0;
              byte[] objData = null;
              string progID = "";
              FileFormatType fileFormatType = FileFormatType.Unknown;
              string sourceFullName = "";
              System.Drawing.Color color = new Color();
              bool isDisplayAsIcon = false;
              byte[] classId = null;

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
                      color = frame.FillFormat.ForeColor;
                      isDisplayAsIcon = frame.DisplayAsIcon;
                      classId = frame.ClassIdentifier;
                      sheet.OleObjects.RemoveAt(i);
                  }
              }

              workbook.Save(Constants.destPath + "CELLSNET44708.xls");
              Workbook workbook2 = new Workbook(Constants.destPath + "CELLSNET44708.xls");
              int oleNumber = workbook2.Worksheets[0].OleObjects.Add(upperLeftRow, upperLeftColumn, height, width, imageData);
              OleObject embeddedObject = workbook2.Worksheets[0].OleObjects[oleNumber];


              embeddedObject.X = x;
              embeddedObject.Y = y;
              embeddedObject.ObjectData = objData;
              embeddedObject.ProgID = progID;
              //embeddedObject.FileFormatType = fileFormatType; 
              //    embeddedObject.Fill.ForeColor = color;
              embeddedObject.DisplayAsIcon = isDisplayAsIcon;
              embeddedObject.ObjectSourceFullName = sourceFullName;
              embeddedObject.IsAutoSize = false;
              if (classId != null)
              {
                  embeddedObject.ClassIdentifier = classId;
              }

              workbook2.Save(Constants.destPath + "CELLSNET44708.xls");
          }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


