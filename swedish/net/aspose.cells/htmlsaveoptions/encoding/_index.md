---
title: "HtmlSaveOptions.Encoding"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Om inte angivet, använd Encoding.UTF8 som standardkodningstyp"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/encoding/
---
## HtmlSaveOptions.Encoding property

Om inte angivet, använd Encoding.UTF8 som standardkodningstyp.

```csharp
public Encoding Encoding { get; set; }
```

### Exempel

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
                // Initiering om behövs
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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata till kalkylblad
            workbook.Worksheets[0].Cells[0, 0].PutValue("Sample content in Sheet1");
            workbook.Worksheets.Add("Sheet2").Cells[0, 0].PutValue("Sample content in Sheet2");

            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Ställ in kodningen till UTF8
            saveOptions.Encoding = Encoding.UTF8;

            // Skapa minnesströmmar för utdata
            using (MemoryStream sheet1Stream = new MemoryStream())
            using (MemoryStream sheet2Stream = new MemoryStream())
            {
                // Skapa en strömleverantör för att hantera flera blad
                SheetStreamProvider streamProvider = new SheetStreamProvider(sheet1Stream, sheet2Stream);
                saveOptions.StreamProvider = streamProvider;

                // Spara arbetsboken med HTML-alternativ
                workbook.Save(new MemoryStream(), saveOptions);

                // Verifiera att innehållet sparades med UTF8-kodning
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

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


