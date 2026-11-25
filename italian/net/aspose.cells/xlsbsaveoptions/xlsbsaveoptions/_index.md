---
title: "XlsbSaveOptions.XlsbSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore XlsbSaveOptions. Crea opzioni di salvataggio per file xlsb"
type: docs
url: /it/net/aspose.cells/xlsbsaveoptions/xlsbsaveoptions/
---
## XlsbSaveOptions() {#constructor}

Crea le opzioni di salvataggio del file xlsb.

```csharp
public XlsbSaveOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Test Value");

            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.ExportAllColumnIndexes = true;

            workbook.Save("output.xlsb", saveOptions);
        }
    }
}
```

### Vedi anche

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsbSaveOptions(SaveFormat) {#constructor_1}

Crea le opzioni di salvataggio del file xlsb.

```csharp
[Obsolete("Use XlsbSaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public XlsbSaveOptions(SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | SaveFormat | Il formato di salvataggio. Deve essere xlsb. |

### Osservazioni

NOTA: Questo costruttore è ora obsoleto. Invece, si prega di utilizzare il costruttore XlsbSaveOptions(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsbSaveOptionsMethodSharpctorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Using XlsbSaveOptions";

            try
            {
                // Crea XlsbSaveOptions usando il costruttore con il parametro SaveFormat
                XlsbSaveOptions saveOptions = new XlsbSaveOptions(SaveFormat.Xlsb);

                // Imposta proprietà aggiuntive se necessario
                saveOptions.ExportAllColumnIndexes = true;

                // Salva la cartella di lavoro con le opzioni di salvataggio specificate
                workbook.Save("XlsbSaveOptionsDemo.xlsb", saveOptions);

                Console.WriteLine("Workbook saved successfully with XlsbSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


