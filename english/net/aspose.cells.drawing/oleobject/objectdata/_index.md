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
// Called: Console.WriteLine(objOle.ObjectData.ToString());
[Test]
        public void Property_ObjectData()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet47752.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            int idxOle = 0;
            OleObject objOle = worksheet.OleObjects[idxOle];
            Console.WriteLine(objOle.ObjectData.ToString());
            Console.WriteLine(objOle.ProgID);
            Console.WriteLine(objOle.ObjectSourceFullName);
            Console.WriteLine(objOle.Label);
            Console.WriteLine(objOle.Text);
            Assert.AreEqual(FileFormatType.Pdf, objOle.FileFormatType);

            idxOle = 1;
            objOle = worksheet.OleObjects[idxOle];
            Console.WriteLine(objOle.ObjectData.ToString());
            Console.WriteLine(objOle.ProgID);
            Console.WriteLine(objOle.ObjectSourceFullName);
            Console.WriteLine(objOle.Label);
            Console.WriteLine(objOle.Text);
            workbook.Save(Constants.destPath + "CellsNet47752.xlsx");
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


