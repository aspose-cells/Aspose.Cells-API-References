---
title: "Enum MemorySetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.MemorySetting enum. Minnesanvändningslägen för cellernas datamodell"
type: docs
url: /sv/net/aspose.cells/memorysetting/
---
## MemorySetting enumeration

Minnesanvändningslägen för cellernas datamodell.

```csharp
public enum MemorySetting
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Normal | `0` | Standardläge för cellmodellen. |
| MemoryPreference | `1` | Minnesprestanda föredras. |
| FileCache | `2` | Minnesprestanda föredras och använda fil istället för minne för att behålla cellernas data. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MemorySettingDemo
    {
        public static void MemorySettingExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Kom åt arbetsbokens inställningar
            WorkbookSettings settings = workbook.Settings;

            // Ställ in minnesanvändningsalternativet till MemoryPreference
            settings.MemorySetting = MemorySetting.MemoryPreference;

            // Skapa ett arbetsblad och lägg till lite data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);

            // Spara arbetsboken
            workbook.Save("MemorySettingExample.xlsx");

            Console.WriteLine("Workbook saved with MemorySetting.MemoryPreference.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


