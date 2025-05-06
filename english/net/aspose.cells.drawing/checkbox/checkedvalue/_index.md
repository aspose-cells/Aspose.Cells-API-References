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
// Called: cb.CheckedValue = CheckValueType.Checked;
[Test]
        public void Property_CheckedValue()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET17607.xls&quot;);
            Worksheet sheet = workbook.Worksheets[0];
          //  MessageBox.Show(sheet.CheckBoxes.Count.ToString());    //3 - OK
            foreach (CheckBox cb in sheet.CheckBoxes)
            {
                cb.Value = true;
                cb.CheckedValue = CheckValueType.Checked;

            }
            Console.WriteLine(sheet.Cells[&quot;T40&quot;].Value);
         //   workbook.Save(@&quot;F:\fileTemp\dest.xls&quot;);
            Assert.AreEqual(sheet.Cells[&quot;T40&quot;].BoolValue, true);
            Assert.AreEqual(sheet.Cells[&quot;T41&quot;].BoolValue, true);
        }
```

### See Also

* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


