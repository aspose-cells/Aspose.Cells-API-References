---
title: Validation.InCellDropDown
second_title: Aspose.Cells for .NET API Reference
description: Validation property. Indicates whether data validation displays a dropdown list that contains acceptable values
type: docs
url: /net/aspose.cells/validation/incelldropdown/
---
## Validation.InCellDropDown property

Indicates whether data validation displays a drop-down list that contains acceptable values.

```csharp
public bool InCellDropDown { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(i == 3, vldt.InCellDropDown, ((char)('A' + i)) + ".GetValidation().InCellDropDown");
[Test]
        public void Property_InCellDropDown()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "Validation/InCellDropDown.xlsx");
            for (int i = 0; i < 4; i++)
            {
                Validation vldt = wb.Worksheets[0].Cells[1, i].GetValidation();
                Assert.AreEqual(i == 3, vldt.InCellDropDown, ((char)('A' + i)) + ".GetValidation().InCellDropDown");
            }
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


