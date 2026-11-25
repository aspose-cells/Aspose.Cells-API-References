---
title: "Enum MemorySetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.MemorySetting enum. Modalità di utilizzo della memoria per il modello di dati delle celle"
type: docs
url: /it/net/aspose.cells/memorysetting/
---
## MemorySetting enumeration

Modalità di utilizzo della memoria per il modello di dati delle celle.

```csharp
public enum MemorySetting
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Normal | `0` | Modalità predefinita per il modello di celle. |
| MemoryPreference | `1` | Prestazioni di memoria preferibili. |
| FileCache | `2` | Prestazioni di memoria preferibili e utilizzo di file invece della memoria per mantenere i dati delle celle. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MemorySettingDemo
    {
        public static void MemorySettingExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Imposta l'opzione di utilizzo della memoria su MemoryPreference
            settings.MemorySetting = MemorySetting.MemoryPreference;

            // Crea un foglio di lavoro e aggiungi alcuni dati
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);

            // Salva la cartella di lavoro
            workbook.Save("MemorySettingExample.xlsx");

            Console.WriteLine("Workbook saved with MemorySetting.MemoryPreference.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


