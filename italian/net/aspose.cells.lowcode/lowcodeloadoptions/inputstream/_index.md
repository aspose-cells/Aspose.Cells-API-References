---
title: "LowCodeLoadOptions.InputStream"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeLoadOptions. Ottiene e imposta lo Stream del modello"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodeloadoptions/inputstream/
---
## LowCodeLoadOptions.InputStream property

Ottiene e imposta lo Stream del modello.

```csharp
public Stream InputStream { get; set; }
```

### Osservazioni

Quando si imposta uno Stream non nullo per questa proprietà, il valore precedentemente impostato per [`InputFile`](../inputfile/) verrà ignorato.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeLoadOptionsPropertyInputStreamDemo
    {
        public static void Run()
        {
            // Crea dati di esempio in uno stream di memoria
            byte[] data = { 0x48, 0x65, 0x6C, 0x6C, 0x6F }; // "Hello" in bytes
            using (MemoryStream stream = new MemoryStream(data))
            {
                // Crea opzioni di caricamento con InputStream
                var loadOptions = new LowCodeLoadOptions() { InputStream = stream };

                // Crea una nuova cartella di lavoro usando lo stream
                using (Workbook workbook = new Workbook(stream))
                {
                    // Accedi al primo foglio di lavoro
                    Worksheet worksheet = workbook.Worksheets[0];
                    
                    // Dimostra che il contenuto è stato caricato
                    Console.WriteLine("First cell value: " + worksheet.Cells["A1"].Value);
                }
            }
        }
    }
}
```

### Vedi anche

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


