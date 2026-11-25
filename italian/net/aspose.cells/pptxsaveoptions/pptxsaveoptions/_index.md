---
title: "PptxSaveOptions.PptxSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore di PptxSaveOptions. Rappresenta le opzioni di salvataggio pptx"
type: docs
url: /it/net/aspose.cells/pptxsaveoptions/pptxsaveoptions/
---
## PptxSaveOptions() {#constructor}

Rappresenta le opzioni di salvataggio pptx.

```csharp
public PptxSaveOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Visible Data");
            worksheet.Cells["A2"].PutValue("Hidden Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // Nascondi la seconda riga
            worksheet.Cells.Rows[1].IsHidden = true;

            // Crea PptxSaveOptions usando il costruttore
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;

            // Salva la cartella di lavoro in PPTX con le opzioni
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved to PPTX with hidden rows ignored.");
        }
    }
}
```

### Vedi anche

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PptxSaveOptions(bool) {#constructor_1}

Rappresenta le opzioni di salvataggio del file .pptx.

```csharp
public PptxSaveOptions(bool saveAsImage)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveAsImage | Booleano | Se True, la cartella di lavoro verrà convertita in alcune immagini del file .pptx. Se False, la cartella di lavoro verrà convertita in alcune tabelle del file .pptx. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slides;
    using System;

    public class PptxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            try
            {
                // Chiama il metodo #ctor con un parametro booleano
                bool saveAsImage = true;
                PptxSaveOptions options = new PptxSaveOptions(saveAsImage);

                // Imposta proprietà aggiuntive
                options.IgnoreHiddenRows = true;
                options.ExportViewType = SlideViewType.View;

                // Salva la cartella di lavoro con le opzioni PPTX
                workbook.Save("PptxSaveOptionsCtorDemo.pptx", options);

                Console.WriteLine("PptxSaveOptions constructor executed successfully with parameter: " + saveAsImage);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PptxSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


