---
title: Enum CheckValueType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.CheckValueType enum. Represents the check value type of the check box
type: docs
url: /net/aspose.cells.drawing/checkvaluetype/
---
## CheckValueType enumeration

Represents the check value type of the check box.

```csharp
public enum CheckValueType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| UnChecked | `0` | UnChecked |
| Checked | `1` | Checked |
| Mixed | `2` | Mixed |

### Examples

```csharp
// Called: box1.CheckedValue = (CheckValueType.Checked);
[Test]
        public void Type_CheckValueType()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            CheckBox box1 = sheet.Shapes.AddCheckBox(5, 5, 5, 5, 20, 20);
            box1.CheckedValue = (CheckValueType.Checked);
            wb.Save(Constants.destPath + &quot;CellsNet55495.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CellsNet55495.xlsx&quot;);
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.destPath + &quot;CellsNet55495.xlsx&quot;, &quot;xl/drawings/drawing1.xml&quot;, new string[] { &quot;mc:AlternateContent&quot; }, true));

        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


