---
title: CustomFilter.FilterOperatorType
second_title: Aspose.Cells for .NET API Reference
description: CustomFilter property. Gets and sets the filter operator type
type: docs
url: /net/aspose.cells/customfilter/filteroperatortype/
---
## CustomFilter.FilterOperatorType property

Gets and sets the filter operator type.

```csharp
public FilterOperatorType FilterOperatorType { get; set; }
```

### Examples

```csharp
// Called: c.FilterOperatorType = FilterOperatorType.EndsWith;
[Test]
        public void Property_FilterOperatorType()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "AutoFilter/CellsNet46319.xlsx");
            AutoFilter filter = wb.Worksheets[0].AutoFilter;
            CustomFilter c = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];
            Assert.AreEqual(FilterOperatorType.Contains, c.FilterOperatorType);
            Assert.AreEqual("e", (string)c.Criteria);
            c.FilterOperatorType = FilterOperatorType.EndsWith;
            Assert.AreEqual("e", (string)c.Criteria);
            Util.ReSave(wb, SaveFormat.Xlsx);//.Save(Constants.destPath + "CellsNet46319_1.xlsx");

            wb = new Workbook(Constants.sourcePath + "AutoFilter/CellsNet46319.xlsx");
            filter = wb.Worksheets[0].AutoFilter;
            filter.Custom(0, FilterOperatorType.NotContains, "e");
            //wb.Save(Constants.destPath + "CellsNet46319_2.xlsx");
            wb = Util.ReSave(wb, SaveFormat.Xlsx);// new Workbook(Constants.destPath + "CellsNet46319_2.xlsx");
            filter = wb.Worksheets[0].AutoFilter;
            c = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];
            Assert.AreEqual(FilterOperatorType.NotContains, c.FilterOperatorType);
            Assert.AreEqual("e", (string)c.Criteria);
        }
```

### See Also

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


