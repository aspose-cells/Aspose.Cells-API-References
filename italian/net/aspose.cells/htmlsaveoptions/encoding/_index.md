---
title: "HtmlSaveOptions.Encoding"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Se non impostata, utilizza Encoding.UTF8 come tipo di codifica predefinito"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/encoding/
---
## HtmlSaveOptions.Encoding property

Se non impostato, utilizza Encoding.UTF8 come tipo di codifica predefinito.

```csharp
public Encoding Encoding { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyEncodingDemo
    {
        private class SheetStreamProvider : IStreamProvider
        {
            private readonly MemoryStream _sheet1Stream;
            private readonly MemoryStream _sheet2Stream;
            private int _currentIndex = 0;

            public SheetStreamProvider(MemoryStream sheet1Stream, MemoryStream sheet2Stream)
            {
                _sheet1Stream = sheet1Stream;
                _sheet2Stream = sheet2Stream;
            }

            public void InitStream(StreamProviderOptions options)
            {
                // Inizializzazione se necessaria
            }

            public Stream GetStream(string sheetName)
            {
                return _currentIndex++ == 0 ? _sheet1Stream : _sheet2Stream;
            }

            public void CloseStream(StreamProviderOptions options)
            {
                options.Stream?.Flush();
            }
        }

        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi dati di esempio ai fogli di lavoro
            workbook.Worksheets[0].Cells[0, 0].PutValue("Sample content in Sheet1");
            workbook.Worksheets.Add("Sheet2").Cells[0, 0].PutValue("Sample content in Sheet2");

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Imposta la codifica su UTF8
            saveOptions.Encoding = Encoding.UTF8;

            // Crea stream di memoria per l'output
            using (MemoryStream sheet1Stream = new MemoryStream())
            using (MemoryStream sheet2Stream = new MemoryStream())
            {
                // Crea un provider di stream per gestire più fogli
                SheetStreamProvider streamProvider = new SheetStreamProvider(sheet1Stream, sheet2Stream);
                saveOptions.StreamProvider = streamProvider;

                // Salva la cartella di lavoro con le opzioni HTML
                workbook.Save(new MemoryStream(), saveOptions);

                // Verifica che il contenuto sia stato salvato con codifica UTF8
                string sheet1Content = Encoding.UTF8.GetString(sheet1Stream.ToArray());
                string sheet2Content = Encoding.UTF8.GetString(sheet2Stream.ToArray());

                Console.WriteLine("Sheet1 content contains text: " + 
                    sheet1Content.Contains("Sample content in Sheet1"));
                Console.WriteLine("Sheet2 content contains text: " + 
                    sheet2Content.Contains("Sample content in Sheet2"));
            }
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


