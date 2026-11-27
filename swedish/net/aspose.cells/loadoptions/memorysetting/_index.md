---
title: "LoadOptions.MemorySetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions-egenskap. Hämtar eller anger minnesläget för den inlästa arbetsboken"
type: docs
url: /sv/net/aspose.cells/loadoptions/memorysetting/
---
## LoadOptions.MemorySetting property

Hämtar eller anger minnesläget för den laddade Workbook.

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
    public class LoadOptionsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Skapa inläsningsalternativ med minnespreferensinställning
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;

            // Läs in arbetsbok med minnesoptimerade inställningar
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Kom åt kalkylbladet och lägg till lite exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Memory Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Spara arbetsboken
            workbook.Save("MemorySettingDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with MemoryPreference setting.");
        }
    }
}
```

### Se även

* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


