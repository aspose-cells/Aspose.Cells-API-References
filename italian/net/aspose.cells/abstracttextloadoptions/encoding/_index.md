---
title: "AbstractTextLoadOptions.Encoding"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractTextLoadOptions. Ottiene e imposta la codifica predefinita. Si applica solo ai file csv"
type: docs
url: /it/net/aspose.cells/abstracttextloadoptions/encoding/
---
## AbstractTextLoadOptions.Encoding property

Ottiene e imposta la codifica predefinita. Si applica solo ai file csv.

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
    public class AbstractTextLoadOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Crea dati CSV di esempio con codifica ASCII
            MemoryStream ms = new MemoryStream();
            byte[] data = Encoding.ASCII.GetBytes("Name,Age\nJohn,30\nJane,25");
            ms.Write(data, 0, data.Length);
            ms.Seek(0, SeekOrigin.Begin);

            // Carica la cartella di lavoro con la codifica ASCII specificata
            Workbook wb = new Workbook(ms, new TxtLoadOptions() { Encoding = Encoding.ASCII });
            Cells cells = wb.Worksheets[0].Cells;

            // Visualizza i dati caricati
            Console.WriteLine($"A1: {cells[0, 0].StringValue}");
            Console.WriteLine($"B1: {cells[0, 1].StringValue}");
            Console.WriteLine($"A2: {cells[1, 0].StringValue}");
            Console.WriteLine($"B2: {cells[1, 1].IntValue}");

            // Aggiungi del testo Unicode
            cells[2, 0].PutValue("日本語のテキスト");
            
            // Salva con codifica UTF-8
            MemoryStream outputStream = new MemoryStream();
            wb.Save(outputStream, new TxtSaveOptions() { Encoding = Encoding.UTF8 });
            
            // Mostra i primi byte per visualizzare il BOM UTF-8
            byte[] outputBytes = outputStream.ToArray();
            Console.WriteLine($"First 3 bytes: {BitConverter.ToString(outputBytes, 0, 3)}");
        }
    }
}
```

### Vedi anche

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


