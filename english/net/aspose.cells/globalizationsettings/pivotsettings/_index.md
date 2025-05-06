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
[Test]
        public void Property_PivotSettings()
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSJAVA44999.xlsx&quot;);
            //Setting Custom Pivot Table Globalization Settings
            CustomPivotTableGlobalizationSettings settings = new CustomPivotTableGlobalizationSettings();
            //settings.SetTestMode(testMode);
            wb.Settings.GlobalizationSettings.PivotSettings = (settings);
            Assert.AreEqual(&quot;Values2&quot;, settings.GetTextOfProtectedName(&quot;Values&quot;));
            //Hide first worksheet that contains the data of the pivot table
            //  wb.getWorksheets().get(0).setVisible(false);

            //Access second worksheet
            Worksheet ws = wb.Worksheets[1];

            //Access the pivot table, refresh and calculate its data
            PivotTable pt = ws.PivotTables[0];
            pt.RefreshData();
            pt.CalculateData();
            pt.RefreshDataOnOpeningFile = false;

            Assert.AreEqual(&quot;DataCaption&quot;, ws.Cells[&quot;C5&quot;].StringValue);
        }
```

### See Also

* class [PivotGlobalizationSettings](../../../aspose.cells.settings/pivotglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


