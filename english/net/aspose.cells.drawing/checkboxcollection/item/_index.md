---
title: CheckBoxCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: CheckBoxCollection property. Gets the CheckBox element at the specified index
type: docs
url: /net/aspose.cells.drawing/checkboxcollection/item/
---
## CheckBoxCollection indexer

Gets the [`CheckBox`](../../checkbox/) element at the specified index.

```csharp
public CheckBox this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: CheckBox checkBox = ws.CheckBoxes[idxCheckBox];
[Test]
        public void Property_Int32_()
            {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];
            int idxCheckBox = ws.CheckBoxes.Add(0, 1, 17, 17);
            CheckBox checkBox = ws.CheckBoxes[idxCheckBox];
            checkBox.Name = (&quot;Importer_Ligne_&quot; + (0 + 1));
            workbook.Save(Constants.destPath + &quot;CELLSJAVA41542.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSJAVA41542.xlsx&quot;);
            checkBox = workbook.Worksheets[0].CheckBoxes[0];
            Assert.AreEqual((&quot;Importer_Ligne_&quot; + (0 + 1)), checkBox.Name);

        }
```

### See Also

* class [CheckBox](../../checkbox/)
* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


