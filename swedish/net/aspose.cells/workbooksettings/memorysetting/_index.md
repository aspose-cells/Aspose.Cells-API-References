---
title: "WorkbookSettings.MemorySetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings property. Hämtar eller anger minnesanvändningsalternativen. Det nya alternativet kommer att tas som standardalternativ för nysskapade arbetsblad men påverkar inte befintliga arbetsblad"
type: docs
url: /sv/net/aspose.cells/workbooksettings/memorysetting/
---
## WorkbookSettings.MemorySetting property

Hämtar eller anger minnesanvändningsalternativen. Det nya alternativet kommer att användas som standardalternativ för nysskapade arbetsblad men påverkar inte befintliga arbetsblad.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Anmärkningar

För mer information om minnesläge, se [`MemorySetting`](../../cells/memorysetting/).

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med minnesinställning
            Workbook wb = new Workbook();
            wb.Settings.MemorySetting = MemorySetting.MemoryPreference;
            
            // Öppna det första kalkylbladet och lägg till data
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Memory Setting Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Spara till minnesström med PDF-format
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Pdf);
                Console.WriteLine("Workbook saved to PDF with MemoryPreference setting");
            }
        }
    }
}
```

### Se även

* enum [MemorySetting](../../memorysetting/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


