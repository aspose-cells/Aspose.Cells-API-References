---
title: PivotTable.ShowReportFilterPageByName
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Show all the report filter pages according to PivotFields name the PivotField must be located in the PageFields
type: docs
url: /net/aspose.cells.pivot/pivottable/showreportfilterpagebyname/
---
## PivotTable.ShowReportFilterPageByName method

Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields.

```csharp
public void ShowReportFilterPageByName(string fieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | String | The name of PivotField |

### Examples

```csharp
// Called: pt.ShowReportFilterPageByName(pt.PageFields[0].Name);
[Test]
        public void Method_String_()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET46429_";
            Workbook wb = new Workbook(filePath + "a.xlsx");
            PivotTable pt = wb.Worksheets[1].PivotTables[0];
            pt.ShowReportFilterPage(pt.PageFields[0]);
            pt.ShowReportFilterPage(pt.PageFields[0]);
            pt.ShowReportFilterPage(pt.PageFields[0]);
            pt.ShowReportFilterPageByIndex(pt.PageFields[0].Position);
            pt.ShowReportFilterPageByName(pt.PageFields[0].Name);
            wb.Save(Constants.PivotTableDestPath + "NET46429.xlsx");
            Assert.AreEqual(wb.Worksheets.Count, 17);
            Assert.AreEqual(wb.Worksheets[15].Name.EndsWith("(5)"), true);
            Assert.AreEqual(wb.Worksheets[12].Name.EndsWith("(4)"), true);
            Assert.AreEqual(wb.Worksheets[9].Name.EndsWith("(3)"), true);
            Assert.AreEqual(wb.Worksheets[6].Name.EndsWith("(2)"), true);

            Assert.AreEqual("18", wb.Worksheets[1].Cells["A4"].StringValue);
            Assert.AreEqual("22", wb.Worksheets[2].Cells["A4"].StringValue);
            Assert.AreEqual("18", wb.Worksheets[3].Cells["A4"].StringValue);


        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


