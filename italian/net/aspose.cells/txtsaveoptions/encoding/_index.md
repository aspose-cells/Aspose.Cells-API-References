---
title: "TxtSaveOptions.Encoding"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtSaveOptions. Ottiene e imposta la codifica predefinita"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/encoding/
---
## TxtSaveOptions.Encoding property

Ottiene e imposta la codifica predefinita.

```csharp
public Encoding Encoding { get; set; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            
            // Crea le opzioni di salvataggio TXT con codifica ASCII
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                Separator = '\t'
            };
            
            // Salva la cartella di lavoro con la codifica specificata
            workbook.Save("output.txt", saveOptions);
            
            Console.WriteLine("File saved with ASCII encoding");
        }
    }
}
```

### Vedi anche

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


