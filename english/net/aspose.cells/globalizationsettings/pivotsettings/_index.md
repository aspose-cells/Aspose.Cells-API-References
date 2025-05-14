---
title: GlobalizationSettings.PivotSettings
second_title: Aspose.Cells for .NET API Reference
description: GlobalizationSettings property. Gets or sets the globalization settings for pivot table
type: docs
url: /net/aspose.cells/globalizationsettings/pivotsettings/
---
## GlobalizationSettings.PivotSettings property

Gets or sets the globalization settings for pivot table.

```csharp
public PivotGlobalizationSettings PivotSettings { get; set; }
```

### Examples

```csharp
// Called: wb.Settings.GlobalizationSettings.PivotSettings = (settings);
public void GlobalizationSettings_Property_PivotSettings()
{
    Workbook wb = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    //Setting Custom Pivot Table Globalization Settings
    CustomPivotTableGlobalizationSettings settings = new CustomPivotTableGlobalizationSettings();
    //settings.SetTestMode(testMode);
    wb.Settings.GlobalizationSettings.PivotSettings = (settings);
    Assert.AreEqual("Values2", settings.GetTextOfProtectedName("Values"));
    //Hide first worksheet that contains the data of the pivot table
    //  wb.getWorksheets().get(0).setVisible(false);

    //Access second worksheet
    Worksheet ws = wb.Worksheets[1];

    //Access the pivot table, refresh and calculate its data
    PivotTable pt = ws.PivotTables[0];
    pt.RefreshData();
    pt.CalculateData();
    pt.RefreshDataOnOpeningFile = false;

    Assert.AreEqual("DataCaption", ws.Cells["C5"].StringValue);
}
```

### See Also

* class [PivotGlobalizationSettings](../../../aspose.cells.settings/pivotglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


