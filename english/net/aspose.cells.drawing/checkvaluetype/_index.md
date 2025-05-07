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
// Called: cb.CheckedValue = CheckValueType.Checked;
[Test]
        public void Type_CheckValueType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET17607.xls");
            Worksheet sheet = workbook.Worksheets[0];
          //  MessageBox.Show(sheet.CheckBoxes.Count.ToString());    //3 - OK
            foreach (CheckBox cb in sheet.CheckBoxes)
            {
                cb.Value = true;
                cb.CheckedValue = CheckValueType.Checked;

            }
            Console.WriteLine(sheet.Cells["T40"].Value);
         //   workbook.Save(@"F:\fileTemp\dest.xls");
            Assert.AreEqual(sheet.Cells["T40"].BoolValue, true);
            Assert.AreEqual(sheet.Cells["T41"].BoolValue, true);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


