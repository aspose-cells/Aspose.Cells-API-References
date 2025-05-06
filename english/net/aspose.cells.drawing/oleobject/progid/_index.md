---
title: OleObject.ProgID
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Gets or sets the ProgID of the OLE object
type: docs
url: /net/aspose.cells.drawing/oleobject/progid/
---
## OleObject.ProgID property

Gets or sets the ProgID of the OLE object.

```csharp
public string ProgID { get; set; }
```

### Examples

```csharp
// Called: progID = frame.ProgID;
[Test]
        public void Property_ProgID()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet44639.xls&quot;);

            int upperLeftRow = 0;
            int upperLeftColumn = 0;
            int height = 0;
            int width = 0;
            byte[] imageData = null;
            int x = 0;
            int y = 0;
            byte[] objData = null;
            string progID = &quot;&quot;;
            string sourceFullName = &quot;&quot;;
            FileFormatType fileFormatType = FileFormatType.Unknown;


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
                    fileFormatType = frame.FileFormatType;
                    sheet.OleObjects.RemoveAt(i);
                }
            }

            workbook.Save(Constants.destPath + &quot;CellsNet44639.xls&quot;);
            Workbook workbook2 = new Workbook(Constants.destPath + &quot;CellsNet44639.xls&quot;);
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
            workbook2.Save(Constants.destPath + &quot;CellsNet44639.xls&quot;); 
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


