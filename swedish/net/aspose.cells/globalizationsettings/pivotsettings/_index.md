---
title: "GlobalizationSettings.PivotSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-egenskapen. Hämtar eller anger globaliseringsinställningarna för pivottabellen"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/pivotsettings/
---
## GlobalizationSettings.PivotSettings property

Hämtar eller anger globaliseringsinställningarna för pivottabellen.

```csharp
public PivotGlobalizationSettings PivotSettings { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfTotal()
        {
            return "Custom Total";
        }

        public override string GetTextOfGrandTotal()
        {
            return "Custom Grand Total";
        }

        public override string GetTextOfDataFieldHeader()
        {
            return "DataCaption";
        }

        public override string GetTextOfProtectedName(string protectedName)
        {
            return protectedName + "2";
        }
    }

    public class GlobalizationSettingsPropertyPivotSettingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("Apple");
            dataSheet.Cells["B2"].PutValue(1000);
            dataSheet.Cells["A3"].PutValue("Orange");
            dataSheet.Cells["B3"].PutValue(2000);

            // Skapa pivottabell
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            int index = pivotSheet.PivotTables.Add("A1", "A1:B3", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[index];
            
            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ange anpassade globaliseringsinställningar för pivottabellen
            CustomPivotGlobalizationSettings pivotSettings = new CustomPivotGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = new GlobalizationSettings();
            workbook.Settings.GlobalizationSettings.PivotSettings = pivotSettings;

            // Uppdatera pivottabellen för att tillämpa inställningarna
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotGlobalizationSettings](../../../aspose.cells.settings/pivotglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


