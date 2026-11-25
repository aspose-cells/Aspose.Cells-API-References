---
title: "EbookSaveOptions.EbookSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore EbookSaveOptions. Crea le opzioni per salvare il file ebook"
type: docs
url: /it/net/aspose.cells.saving/ebooksaveoptions/ebooksaveoptions/
---
## EbookSaveOptions() {#constructor}

Crea opzioni per salvare il file ebook.

```csharp
public EbookSaveOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class EbookSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi contenuto di esempio
            worksheet.Cells["A1"].PutValue("Ebook Test");
            worksheet.Cells["A2"].PutValue("This is a test for EbookSaveOptions");
            
            // Crea EbookSaveOptions usando il costruttore
            EbookSaveOptions saveOptions = new EbookSaveOptions();
            
            // Salva la cartella di lavoro con EbookSaveOptions (salva automaticamente come EPUB)
            workbook.Save("output.epub", saveOptions);
            
            Console.WriteLine("Ebook saved successfully with EbookSaveOptions constructor.");
        }
    }
}
```

### Vedi anche

* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)

---

## EbookSaveOptions(SaveFormat) {#constructor_1}

Crea opzioni per salvare il file ebook.

```csharp
public EbookSaveOptions(SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | SaveFormat | Il formato file. Deve essere Epub o Azw3. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Sample Ebook Content");
            
            try
            {
                // Chiama il metodo #ctor con il parametro SaveFormat
                EbookSaveOptions saveOptions = new EbookSaveOptions(SaveFormat.Epub);
                
                // Imposta proprietà aggiuntive se necessario
                saveOptions.Encoding = System.Text.Encoding.UTF8;
                
                Console.WriteLine("EbookSaveOptions constructor executed successfully with SaveFormat.Epub");
                
                // Salva la cartella di lavoro con le opzioni create
                workbook.Save("EbookSaveOptionsDemo.epub", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


