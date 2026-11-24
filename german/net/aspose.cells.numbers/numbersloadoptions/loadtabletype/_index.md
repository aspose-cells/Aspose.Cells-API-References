---
title: "NumbersLoadOptions.LoadTableType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NumbersLoadOptions-Eigenschaft. Ruft den Typ des Ladens mehrerer Tabellen in einem Arbeitsblatt ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.numbers/numbersloadoptions/loadtabletype/
---
## NumbersLoadOptions.LoadTableType property

Liest und setzt den Typ des Ladens mehrerer Tabellen in einem Arbeitsblatt.

```csharp
public LoadNumbersTableType LoadTableType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsPropertyLoadTableTypeDemo
    {
        public static void Run()
        {
            // Eine Instanz von NumbersLoadOptions erstellen
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Demonstriert die Verwendung der LoadTableType-Eigenschaft
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                
                // Weitere minimal erforderliche Eigenschaften
                Password = "password123",
                ParsingFormulaOnOpen = true
            };

            // Laden Sie eine Numbers‑Datei mit den angegebenen Ladeoptionen
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Speichern Sie die Arbeitsmappe im XLSX‑Format
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [LoadNumbersTableType](../../loadnumberstabletype/)
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


