---
title: "Enum LoadNumbersTableType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Numbers.LoadNumbersTableType Enum. Gibt den Typ des Ladens von Tabellen an, wenn sich mehrere Tabellen in einem Blatt befinden"
type: docs
url: /de/net/aspose.cells.numbers/loadnumberstabletype/
---
## LoadNumbersTableType enumeration

Gibt den Typ des Ladens von Tabellen an, wenn mehrere Tabellen in einem Blatt vorhanden sind.

```csharp
public enum LoadNumbersTableType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| OneTablePerSheet | `1` |  |
| OverrideOtherTables | `2` |  |
| TileTables | `4` |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Numbers;
    using System;

    public class LoadNumbersTableTypeDemo
    {
        public static void LoadNumbersTableTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt erstellen
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Instanz von NumbersLoadOptions erstellen
            NumbersLoadOptions loadOptions = new NumbersLoadOptions();

            // Setzen Sie die Eigenschaft LoadNumbersTableType
            loadOptions.LoadTableType = LoadNumbersTableType.OneTablePerSheet;

            // Laden Sie eine Numbers‑Datei mit den angegebenen Ladeoptionen
            workbook = new Workbook("LoadNumbersTableTypeExample_original.numbers", loadOptions);

            // Speichere die Arbeitsmappe in einer Excel‑Datei
            workbook.Save("LoadNumbersTableTypeExample.xlsx");

            Console.WriteLine("Workbook loaded and saved successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)


