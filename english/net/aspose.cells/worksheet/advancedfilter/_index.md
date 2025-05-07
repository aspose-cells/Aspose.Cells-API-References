---
title: Worksheet.AdvancedFilter
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Filters data using complex criteria
type: docs
url: /net/aspose.cells/worksheet/advancedfilter/
---
## Worksheet.AdvancedFilter method

Filters data using complex criteria.

```csharp
public void AdvancedFilter(bool isFilter, string listRange, string criteriaRange, string copyTo, 
    bool uniqueRecordOnly)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isFilter | Boolean | Indicates whether filtering the list in place. |
| listRange | String | The list range. |
| criteriaRange | String | The criteria range. |
| copyTo | String | The range where copying data to. |
| uniqueRecordOnly | Boolean | Only displaying or copying unique rows. |

### Examples

```csharp
// Called: workbook.Worksheets[0].AdvancedFilter(false, "A4:F13", "A1:F3", null, false);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "AutoFilter/AdvancedFilter001.xlsx");

            workbook.Worksheets[0].AdvancedFilter(false, "A4:F13", "A1:F3", null, true);
            Assert.AreEqual("Apple",workbook.Worksheets[0].Cells["A18"].StringValue);
            Assert.AreEqual("", workbook.Worksheets[0].Cells["A19"].StringValue);
            Util.ReSave(workbook, SaveFormat.Xlsx);//.Save(Constants.destPath + "AdvancedFilter001.xlsx");

            workbook = new Workbook(Constants.sourcePath + "AutoFilter/AdvancedFilter001.xlsx");
            workbook.Worksheets[0].AdvancedFilter(false, "A4:F13", "A1:F3", null, false);
            Assert.AreEqual("Apple", workbook.Worksheets[0].Cells["A18"].StringValue);
            Assert.AreEqual("Apple", workbook.Worksheets[0].Cells["A19"].StringValue);
            Util.ReSave(workbook, SaveFormat.Xlsx);//.Save(Constants.destPath + "AdvancedFilter001.xlsx");
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


