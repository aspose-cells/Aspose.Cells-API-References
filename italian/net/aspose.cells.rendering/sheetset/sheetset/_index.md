---
title: "SheetSet.SheetSet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore di SheetSet. Crea un set di fogli basato su indici di foglio esatti"
type: docs
url: /it/net/aspose.cells.rendering/sheetset/sheetset/
---
## SheetSet(params int[]) {#constructor}

Crea un insieme di fogli basato su indici di foglio esatti.

```csharp
public SheetSet(params int[] sheetIndexes)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndexes | Int32[] | indici di foglio basati su zero. |

### Osservazioni

Se viene incontrato un foglio che non è nella cartella di lavoro, verrà sollevata un'eccezione durante il rendering.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithInt32ArrayDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con 3 fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Aggiungi testo di identificazione a ciascun foglio
            workbook.Worksheets[0].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets[1].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets[2].Cells["A1"].PutValue("This is Sheet 3");

            try
            {
                // Crea SheetSet con indici di foglio specifici (0 e 2)
                SheetSet sheetSet = new SheetSet(new int[] { 0, 2 });

                // Crea opzioni di salvataggio PDF con il nostro SheetSet
                PdfSaveOptions options = new PdfSaveOptions();
                options.SheetSet = sheetSet;

                // Salva la cartella di lavoro con i fogli selezionati
                workbook.Save("SheetSetDemo.pdf", options);
                Console.WriteLine("Created PDF containing Sheet 1 and Sheet 3");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid sheet index specified: {ex.Message}");
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

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SheetSet(params string[]) {#constructor_1}

Crea un insieme di fogli basato su nomi di foglio esatti.

```csharp
public SheetSet(params string[] sheetNames)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetNames | String[] | nomi dei fogli. |

### Osservazioni

Se viene incontrato un foglio che non è nella cartella di lavoro, verrà sollevata un'eccezione durante il rendering.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithStringArrayDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook e aggiungi fogli
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "First";
            workbook.Worksheets.Add("Second");
            workbook.Worksheets.Add("Third");

            workbook.Worksheets["First"].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets["Second"].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets["Third"].Cells["A1"].PutValue("This is Sheet 3");

            // Prepara i nomi dei fogli per SheetSet
            string[] selectedSheets = { "First", "Third" };

            try
            {
                // Crea SheetSet con parametro array di stringhe
                SheetSet sheetSet = new SheetSet(selectedSheets);

                // Configura le opzioni di salvataggio PDF con SheetSet creato
                PdfSaveOptions pdfOptions = new PdfSaveOptions();
                pdfOptions.SheetSet = sheetSet;

                // Salva il workbook in PDF con i fogli specificati
                workbook.Save("SheetSetOutput.pdf", pdfOptions);

                Console.WriteLine("Created PDF with sheets: " + string.Join(", ", selectedSheets));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating SheetSet: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


