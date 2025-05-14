---
title: OleObject.ImageData
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. Represents image of ole object as byte array
type: docs
url: /net/aspose.cells.drawing/oleobject/imagedata/
---
## OleObject.ImageData property

Represents image of ole object as byte array.

```csharp
public byte[] ImageData { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(binaryImg[300], objOle.ImageData[300]);
public void OleObject_Property_ImageData()
{
    Workbook workbook = new Workbook();
    byte[] binaryImg = File.ReadAllBytes(Constants.sourcePath + "image1.png");
    //converting attachment data into bytes

    //In real we will get the documents from blob storage, azure
    //Stream stream = DownloadStreamFromBlob(info.StoragePath.Split("/")[0].ToString(), Path.Combine(info.StoragePath.Split("/")[1].ToString(), info.DocumentBlobId));
    //byte[] binaryXlsx = ReadFully(stream);

    int idxOle = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, binaryImg);
    OleObject objOle = workbook.Worksheets[0].OleObjects[idxOle];
    objOle.SetEmbeddedObject(false, binaryImg, Constants.sourcePath + "image1.png", true, "abcd",false);
    Assert.AreEqual(binaryImg[300], objOle.ImageData[300]);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


