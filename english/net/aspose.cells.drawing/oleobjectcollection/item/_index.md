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
// Called: OleObject objOle = workbook.Worksheets[0].OleObjects[idxOle];
public void OleObjectCollection_Property_Item()
{
    Workbook workbook = new Workbook();
    byte[] binaryImg = File.ReadAllBytes(Constants.sourcePath + "image1.png");
    //converting attachment data into bytes

    //In real we will get the documents from blob storage, azure
    //Stream stream = DownloadStreamFromBlob(info.StoragePath.Split("/")[0].ToString(), Path.Combine(info.StoragePath.Split("/")[1].ToString(), info.DocumentBlobId));
    //byte[] binaryXlsx = ReadFully(stream);

    int idxOle = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, binaryImg);
    OleObject objOle = workbook.Worksheets[0].OleObjects[idxOle];
    objOle.SetEmbeddedObject(false, File.ReadAllBytes(Constants.sourcePath + "example.xlsx"), "aaaaaaaaaa", true, "abcd", false);
  //  Assert.AreEqual(binaryImg[300], objOle.ImageData[300]);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual("oleObject1.xlsx", workbook.Worksheets[0].OleObjects[0].ObjectSourceFullName);
}
```

### See Also

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


