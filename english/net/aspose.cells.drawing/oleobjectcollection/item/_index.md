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
// Called: Assert.AreEqual(sheet.OleObjects[0].FileFormatType, FileFormatType.Docx);
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath +"Embedded.xls");
            Worksheet sheet = workbook.Worksheets["DOC + DOCX"];
            Assert.AreEqual(sheet.OleObjects[0].FileFormatType, FileFormatType.Docx);
            Assert.AreEqual(sheet.OleObjects[1].FileFormatType, FileFormatType.Doc);
            workbook.Save(Constants.destPath + "dest.xls");
        }
```

### See Also

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


