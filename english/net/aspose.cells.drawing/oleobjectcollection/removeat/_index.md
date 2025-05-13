---
title: OleObjectCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: OleObjectCollection method. Removes the element at the specified index
type: docs
url: /net/aspose.cells.drawing/oleobjectcollection/removeat/
---
## OleObjectCollection.RemoveAt method

Removes the element at the specified index.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The specified index. |

### Examples

```csharp
// Called: sheet.OleObjects.RemoveAt(oleCounter);
public void OleObjectCollection_Method_RemoveAt()
{
    using (Workbook workbook = new Workbook(Constants.sourcePath + "example.xls",
           new Aspose.Cells.LoadOptions(Aspose.Cells.LoadFormat.Excel97To2003)))
    {
        foreach (Worksheet sheet in workbook.Worksheets)
        {

            int totalOleCounter = sheet.OleObjects.Count;
            for (int oleCounter = totalOleCounter - 1; oleCounter >= 0; --oleCounter)
            {
                OleObject embeddedObject = sheet.OleObjects[oleCounter];
                if (embeddedObject == null) continue;
                sheet.OleObjects.RemoveAt(oleCounter);
            }

            int numOfPictures = sheet.Pictures.Count;
            for (int imageCounter = numOfPictures - 1; imageCounter >= 0; --imageCounter)
            {
                Picture image = sheet.Pictures[imageCounter];
                if (image.Data == null) continue;
                sheet.Pictures.RemoveAt(imageCounter);
            }
        }
        workbook.RemoveMacro();
        workbook.Save(Constants.destPath + "example.xls", Aspose.Cells.SaveFormat.Excel97To2003);
    }
}
```

### See Also

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


