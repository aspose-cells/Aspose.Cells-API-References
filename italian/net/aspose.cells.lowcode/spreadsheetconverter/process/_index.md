---
title: "SpreadsheetConverter.Process"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SpreadsheetConverter. Converte il file modello fornito tra i formati di file di foglio di calcolo"
type: docs
url: /it/net/aspose.cells.lowcode/spreadsheetconverter/process/
---
## Process(string, string) {#process_1}

Converte il file modello fornito tra diversi formati di file foglio di calcolo.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| templateFile | String | Il file modello da convertire |
| resultFile | String | Il file risultante |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            SpreadsheetConverter.Process("file1.xlsx", "SpreadsheetConverterMethodProcessWithStringStringDemo.xlsb");
        }
    }
}
```

### Vedi anche

* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Converte tra diversi formati di file foglio di calcolo.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Opzioni per l'input e il caricamento |
| saveOptions | LowCodeSaveOptions | Opzioni per l'output e il salvataggio |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento con il file di input
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "file1.xlsx";

            // Crea opzioni di salvataggio con il file di output
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo.xlsx";

            // Esegui la conversione
            SpreadsheetConverter.Process(loadOptions, saveOptions);
        }
    }
}
```

### Vedi anche

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


