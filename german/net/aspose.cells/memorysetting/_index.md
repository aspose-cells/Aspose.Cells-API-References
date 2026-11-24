---
title: "Enum MemorySetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.MemorySetting enum. Speicherverbrauchsmodi für das Zellen-Datenmodell"
type: docs
url: /de/net/aspose.cells/memorysetting/
---
## MemorySetting enumeration

Speichernutzungsmodi für das Zellen-Datenmodell.

```csharp
public enum MemorySetting
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Normal | `0` | Standardmodus für das Zellenmodell. |
| MemoryPreference | `1` | Speicher‑Performance bevorzugt. |
| FileCache | `2` | Speicher‑Performance bevorzugt und Verwendung einer Datei anstelle des Speichers zur Verwaltung der Zellen­daten. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MemorySettingDemo
    {
        public static void MemorySettingExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf die Arbeitsmappeneinstellungen zu
            WorkbookSettings settings = workbook.Settings;

            // Setzen Sie die Speicherverbrauchsoption auf MemoryPreference
            settings.MemorySetting = MemorySetting.MemoryPreference;

            // Erstellen Sie ein Arbeitsblatt und fügen Sie einige Daten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);

            // Speichere die Arbeitsmappe
            workbook.Save("MemorySettingExample.xlsx");

            Console.WriteLine("Workbook saved with MemorySetting.MemoryPreference.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


