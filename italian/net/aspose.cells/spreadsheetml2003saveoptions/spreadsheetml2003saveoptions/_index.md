---
title: "SpreadsheetML2003SaveOptions.SpreadsheetML2003SaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore SpreadsheetML2003SaveOptions. Crea le opzioni per salvare un file Excel 2003 spreadml"
type: docs
url: /it/net/aspose.cells/spreadsheetml2003saveoptions/spreadsheetml2003saveoptions/
---
## SpreadsheetML2003SaveOptions() {#constructor}

Crea le opzioni per salvare un file spreadml Excel 2003.

```csharp
public SpreadsheetML2003SaveOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // Crea SpreadsheetML2003SaveOptions con il costruttore
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            
            // Imposta le opzioni
            saveOptions.LimitAsXls = true;
            saveOptions.ExportColumnIndexOfCell = true;

            // Salva con le opzioni
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with SpreadsheetML2003SaveOptions");
        }
    }
}
```

### Vedi anche

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SpreadsheetML2003SaveOptions(SaveFormat) {#constructor_1}

Crea le opzioni per salvare un file spreadml Excel 2003.

```csharp
[Obsolete("Use SpreadsheetML2003SaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SpreadsheetML2003SaveOptions(SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | SaveFormat | Il formato di salvataggio. |

### Osservazioni

NOTA: Questo costruttore è ora obsoleto. Invece, si prega di utilizzare il costruttore SpreadsheetML2003SaveOptions(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SpreadsheetML2003SaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);

            try
            {
                // Chiama il metodo #ctor con il parametro SaveFormat
                SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();

                // Imposta alcune proprietà delle opzioni di salvataggio
                saveOptions.IsIndentedFormatting = true;
                saveOptions.LimitAsXls = false;
                saveOptions.ExportColumnIndexOfCell = true;

                Console.WriteLine("SpreadsheetML2003SaveOptions created successfully with SaveFormat parameter");

                // Salva la cartella di lavoro usando le opzioni di salvataggio create
                workbook.Save("SpreadsheetML2003Output.xml", saveOptions);
                Console.WriteLine("Workbook saved successfully with SpreadsheetML2003SaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SpreadsheetML2003SaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


