---
title: "OoxmlSaveOptions.EmbedOoxmlAsOleObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OoxmlSaveOptions. Indica se incorporare i file Ooxml di OleObject come oggetto ole"
type: docs
url: /it/net/aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/
---
## OoxmlSaveOptions.EmbedOoxmlAsOleObject property

Indica se incorporare i file Ooxml di OleObject come oggetto OLE.

```csharp
public bool EmbedOoxmlAsOleObject { get; set; }
```

### Osservazioni

Solo per OleObject.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyEmbedOoxmlAsOleObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OLE Object Embedding");
            
            // Crea le opzioni di salvataggio OOXML e imposta EmbedOoxmlAsOleObject
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EmbedOoxmlAsOleObject = true;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML embedded as OLE object.");
        }
    }
}
```

### Vedi anche

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


