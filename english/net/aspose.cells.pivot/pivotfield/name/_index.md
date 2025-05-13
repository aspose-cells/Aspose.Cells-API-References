---
title: PivotField.Name
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the name of PivotField
type: docs
url: /net/aspose.cells.pivot/pivotfield/name/
---
## PivotField.Name property

Represents the name of PivotField.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("MyYears", pt.RowFields[0].Name);
public void PivotField_Property_Name()
{
    Workbook wb = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    wb.CalculateFormula();
    wb.Worksheets.RefreshAll();
    //Setting Custom Pivot Table Globalization Settings
    CustomPivotTableGlobalizationSettings settings = new CustomPivotTableGlobalizationSettings();
    //settings.SetTestMode(testMode);
    wb.Settings.GlobalizationSettings.PivotSettings = (settings);

    PivotTable pt = wb.Worksheets[0].PivotTables[0];
    DateTime start = new DateTime(2024,1,1);
    DateTime end = new DateTime(2024, 1, 15);
    //ArrayList groupTypeList = new ArrayList();
    //groupTypeList.Add(PivotGroupByType.Months);
    //groupTypeList.Add(PivotGroupByType.Years);
    // pivot.SetManualGroupField(dateBaseField, start, end, groupTypeList, 1);
    pt.RowFields[0].GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, true);
    wb.Save(Constants.PivotTableDestPath + "example.xlsx");
    Assert.AreEqual("MyYears", pt.RowFields[0].Name);
    Assert.AreEqual("MyMonths", pt.RowFields[1].Name);
    //   pt.CalculateData();
    Assert.AreEqual(start.Year.ToString(), wb.Worksheets[0].Cells["F10"].StringValue);
    Assert.AreEqual("Jan", wb.Worksheets[0].Cells["F11"].StringValue);
         

}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


