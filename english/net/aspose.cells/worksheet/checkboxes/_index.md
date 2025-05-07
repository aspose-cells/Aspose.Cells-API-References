---
title: Worksheet.CheckBoxes
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets a CheckBox collection
type: docs
url: /net/aspose.cells/worksheet/checkboxes/
---
## Worksheet.CheckBoxes property

Gets a [`CheckBox`](../../../aspose.cells.drawing/checkbox/) collection.

```csharp
public CheckBoxCollection CheckBoxes { get; }
```

### Examples

```csharp
// Called: ws.CheckBoxes[0].Name = ("Paper");
[Test]
        public void Property_CheckBoxes()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsJava42481.xlsx");

            Worksheet ws = wb.Worksheets["Sheet1"];

            ws.CheckBoxes[0].Name = ("Paper");

            wb.Save(Constants.destPath + "CellsJava42481.xlsx");
            wb = new Workbook(Constants.destPath + "CellsJava42481.xlsx");
            Assert.AreEqual("Paper", wb.Worksheets[0].Shapes[0].Name);
        }
```

### See Also

* class [CheckBoxCollection](../../../aspose.cells.drawing/checkboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


