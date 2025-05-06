---
title: OleObjectCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: OleObjectCollection property. Gets the OleObject element at the specified index
type: docs
url: /net/aspose.cells.drawing/oleobjectcollection/item/
---
## OleObjectCollection indexer

Gets the [`OleObject`](../../oleobject/) element at the specified index.

```csharp
public OleObject this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: sheet.OleObjects[0].ObjectData = objectData;
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook();
            //Get the first worksheet. 
            Worksheet sheet = workbook.Worksheets[0];
            //Define a string variable to store the image path.
           
            //Get an excel file path in a variable.
            string path = Constants.sourcePath + &quot;updatedWithAspose.ppt&quot;;
            //Get the file into the streams.
           FileStream fs = File.OpenRead(path);
            //Define an array of bytes. 
            byte[] objectData = new Byte[fs.Length];
            //Store the file from streams.
            fs.Read(objectData, 0, objectData.Length);
            //Close the stream.
            fs.Close();
            //Add an Ole object into the worksheet with the image
            //shown in MS Excel.
            sheet.OleObjects.Add(14, 3, 200, 220, null);
            //Set embedded ole object data.     
            sheet.OleObjects[0].ObjectData = objectData;
            sheet.OleObjects[0].DisplayAsIcon = true;

          
            sheet.OleObjects[0].ObjectSourceFullName = path;
            sheet.OleObjects[0].Label = Path.GetFileName(path);
            Assert.IsNotNull(sheet.OleObjects[0].ImageData);
            //Save the excel file
            workbook.Save(Constants.destPath + &quot;CellsCore90.xlsx&quot;);
        }
```

### See Also

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


