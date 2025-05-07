---
title: LoadOptions.CheckDataValid
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Check whether data is valid in the template file
type: docs
url: /net/aspose.cells/loadoptions/checkdatavalid/
---
## LoadOptions.CheckDataValid property

Check whether data is valid in the template file.

```csharp
public bool CheckDataValid { get; set; }
```

### Examples

```csharp
// Called: new TxtLoadOptions() { CheckDataValid = false, CheckExcelRestriction = false });
[Test]
        public void Property_CheckDataValid()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.CheckExcelRestriction = false;
            workbook.Worksheets[0].Cells["A1"].PutValue(new string('a', 40000));
            workbook = Util.ReSave(workbook, new TxtSaveOptions(),
                new TxtLoadOptions() { CheckDataValid = false, CheckExcelRestriction = false });
            Assert.AreEqual(40000, workbook.Worksheets[0].Cells["A1"].StringValue.Length, "Long string exceeds liimit");
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


