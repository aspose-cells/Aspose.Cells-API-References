---
title: CheckBox.CheckedValue
second_title: Aspose.Cells for .NET API Reference
description: CheckBox property. Gets or set checkbox value
type: docs
url: /net/aspose.cells.drawing/checkbox/checkedvalue/
---
## CheckBox.CheckedValue property

Gets or set checkbox' value.

```csharp
public CheckValueType CheckedValue { get; set; }
```

### Examples

```csharp
// Called: box1.CheckedValue = (CheckValueType.Checked);
[Test]
        public void Property_CheckedValue()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            CheckBox box1 = sheet.Shapes.AddCheckBox(5, 5, 5, 5, 20, 20);
            box1.CheckedValue = (CheckValueType.Checked);
            wb.Save(Constants.destPath + "CellsNet55495.xlsx");
            wb = new Workbook(Constants.destPath + "CellsNet55495.xlsx");
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + "CellsNet55495.xlsx", "xl/drawings/drawing1.xml", new string[] { "mc:AlternateContent" }, true));

        }
```

### See Also

* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


