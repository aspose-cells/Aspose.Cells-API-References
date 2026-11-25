---
title: "XpsSaveOptions.XpsSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore XpsSaveOptions. Crea le opzioni per salvare il file xps"
type: docs
url: /it/net/aspose.cells/xpssaveoptions/xpssaveoptions/
---
## XpsSaveOptions() {#constructor}

Crea le opzioni per salvare il file xps.

```csharp
public XpsSaveOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XpsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("XPS Save Options Demo");

            // Inizializza XpsSaveOptions usando il costruttore
            XpsSaveOptions saveOptions = new XpsSaveOptions();

            // Configura le opzioni di salvataggio
            saveOptions.OnePagePerSheet = true;
            saveOptions.DefaultFont = "Arial";
            saveOptions.PageIndex = 0;
            saveOptions.PageCount = 1;

            // Salva la cartella di lavoro con le opzioni
            workbook.Save("XpsSaveOptionsDemo.xps", saveOptions);
        }
    }
}
```

### Vedi anche

* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XpsSaveOptions(SaveFormat) {#constructor_1}

Crea le opzioni per salvare il file xps.

```csharp
[Obsolete("Use XpsSaveOptions() constructor instead.")]
public XpsSaveOptions(SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | SaveFormat | Il formato di salvataggio, deve essere il formato xps. |

### Osservazioni

NOTA: Questo costruttore è ora obsoleto. Invece, si prega di utilizzare il costruttore XpsSaveOptions(). Questa proprietà sarà rimossa tra 12 mesi a partire da agosto 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XpsSaveOptionsMethodSharpctorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "XPS Save Options Demo";
            worksheet.Cells["B1"].Value = "Using SaveFormat parameter";

            try
            {
                // Crea XpsSaveOptions usando il costruttore con il parametro SaveFormat.
                XpsSaveOptions saveOptions = new XpsSaveOptions(SaveFormat.Xps);

                // Salva la cartella di lavoro con le opzioni specificate
                workbook.Save("XpsSaveOptionsWithSaveFormatDemo.xps", saveOptions);

                Console.WriteLine("XpsSaveOptions created successfully with SaveFormat parameter");
                Console.WriteLine("Workbook saved as XPS format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating XpsSaveOptions or saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


