---
title: "SpreadsheetConverter.Process"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SpreadsheetConverter-Methode. Konvertiert die angegebene Vorlagendatei zwischen Tabellenkalkulationsdateiformaten"
type: docs
url: /de/net/aspose.cells.lowcode/spreadsheetconverter/process/
---
## Process(string, string) {#process_1}

Konvertiert die angegebene Vorlagendatei zwischen Tabellenkalkulationsdateiformaten.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| templateFile | String | Die zu konvertierende Vorlagendatei |
| resultFile | String | Die resultierende Datei |

### Beispiele

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

### Siehe auch

* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Konvertiert zwischen verschiedenen Tabellenkalkulationsdateiformaten.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Optionen für Eingabe und Laden |
| saveOptions | LowCodeSaveOptions | Optionen für Ausgabe und Speichern |

### Beispiele

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
            // Ladeoptionen mit Eingabedatei erstellen
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "file1.xlsx";

            // Speicheroptionen mit Ausgabedatei erstellen
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo.xlsx";

            // Konvertierung ausführen
            SpreadsheetConverter.Process(loadOptions, saveOptions);
        }
    }
}
```

### Siehe auch

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


