---
title: OleObject.ObjectData
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Represents embedded ole object data as byte array
type: docs
url: /net/aspose.cells.drawing/oleobject/objectdata/
---
## OleObject.ObjectData property

Represents embedded ole object data as byte array.

```csharp
public byte[] ObjectData { get; set; }
```

### Examples

```csharp
// Called: objData = frame.ObjectData;
[Test]
          public void Property_ObjectData()
          {

              Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET44708.xls&quot;);

              int upperLeftRow = 0;
              int upperLeftColumn = 0;
              int height = 0;
              int width = 0;
              byte[] imageData = null;
              int x = 0;
              int y = 0;
              byte[] objData = null;
              string progID = &quot;&quot;;
              FileFormatType fileFormatType = FileFormatType.Unknown;
              string sourceFullName = &quot;&quot;;
              System.Drawing.Color color = new Color();
              bool isDisplayAsIcon = false;
              byte[] classId = null;

              foreach (Worksheet sheet in workbook.Worksheets)
              {
                  for (int i = sheet.OleObjects.Count - 1; i &gt;= 0; --i)
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

              workbook.Save(Constants.destPath + &quot;CELLSNET44708.xls&quot;);
              Workbook workbook2 = new Workbook(Constants.destPath + &quot;CELLSNET44708.xls&quot;);
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

              workbook2.Save(Constants.destPath + &quot;CELLSNET44708.xls&quot;);
          }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


