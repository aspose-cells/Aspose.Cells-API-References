---
title: "PivotGlobalizationSettings.GetTextOfProtection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar skyddsnamnet i pivottabellen"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotection/
---
## PivotGlobalizationSettings.GetTextOfProtection method

Hämtar skyddsnamnet i pivottabellen.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfProtectedName(string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetTextOfProtection()
```

### Returvärde

Skyddsnamnet för pivottabellen

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället PivotGlobalizationSettings.GetTextOfProtectedName(string)-metoden. Denna egenskap kommer att tas bort 12 månader senare från och med mars 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfProtectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa globaliseringsinställningar och demonstrera GetTextOfProtection
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            Console.WriteLine("Protection Text: " + globalizationSettings.GetTextOfProtection());

            // Spara arbetsboken
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


