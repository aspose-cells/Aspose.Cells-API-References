---
title: "LoadOptions.MemorySetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Liest oder setzt den Speichermodus für das geladene Arbeitsbuch"
type: docs
url: /de/net/aspose.cells/loadoptions/memorysetting/
---
## LoadOptions.MemorySetting property

Liest oder legt den Speichermodus für die geladene Arbeitsmappe fest.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Hinweise

Weitere Details zum Speichermodus finden Sie unter [`MemorySetting`](../../cells/memorysetting/).

### Beispiele

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
            // Erstelle LoadOptions mit Speicherpräferenz-Einstellung
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;

            // Lade Workbook mit speicheroptimierten Einstellungen
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Zugriff auf das Arbeitsblatt und einige Beispieldaten hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Memory Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Speichere die Arbeitsmappe
            workbook.Save("MemorySettingDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with MemoryPreference setting.");
        }
    }
}
```

### Siehe auch

* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


