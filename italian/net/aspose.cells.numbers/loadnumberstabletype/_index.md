---
title: "Enum LoadNumbersTableType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Numbers.LoadNumbersTableType. Indica il tipo di caricamento delle tabelle quando alcune tabelle sono in un foglio"
type: docs
url: /it/net/aspose.cells.numbers/loadnumberstabletype/
---
## LoadNumbersTableType enumeration

Indica il tipo di caricamento delle tabelle quando alcune tabelle sono in un foglio.

```csharp
public enum LoadNumbersTableType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| OneTablePerSheet | `1` |  |
| OverrideOtherTables | `2` |  |
| TileTables | `4` |  |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un nuovo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions();

            // Imposta la proprietà LoadNumbersTableType
            loadOptions.LoadTableType = LoadNumbersTableType.OneTablePerSheet;

            // Carica un file Numbers con le opzioni di caricamento specificate
            workbook = new Workbook("LoadNumbersTableTypeExample_original.numbers", loadOptions);

            // Salva la cartella di lavoro in un file Excel
            workbook.Save("LoadNumbersTableTypeExample.xlsx");

            Console.WriteLine("Workbook loaded and saved successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)


