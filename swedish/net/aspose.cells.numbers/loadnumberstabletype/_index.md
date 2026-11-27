---
title: "Enum LoadNumbersTableType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Numbers.LoadNumbersTableType enum. Anger typen av inläsning av tabeller när vissa tabeller finns i ett blad"
type: docs
url: /sv/net/aspose.cells.numbers/loadnumberstabletype/
---
## LoadNumbersTableType enumeration

Anger typen av inläsning av tabeller när vissa tabeller finns i ett blad.

```csharp
public enum LoadNumbersTableType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| OneTablePerSheet | `1` |  |
| OverrideOtherTables | `2` |  |
| TileTables | `4` |  |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett nytt arbetsblad
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions();

            // Ange egenskapen LoadNumbersTableType
            loadOptions.LoadTableType = LoadNumbersTableType.OneTablePerSheet;

            // Läs in en Numbers-fil med de angivna inläsningsalternativen
            workbook = new Workbook("LoadNumbersTableTypeExample_original.numbers", loadOptions);

            // Spara arbetsboken till en Excel-fil
            workbook.Save("LoadNumbersTableTypeExample.xlsx");

            Console.WriteLine("Workbook loaded and saved successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)


