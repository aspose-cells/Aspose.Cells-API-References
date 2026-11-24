---
title: "OoxmlSaveOptions.EmbedOoxmlAsOleObject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OoxmlSaveOptions‑Eigenschaft. Gibt an, ob Ooxml‑Dateien von OleObject als Ole‑Objekt eingebettet werden"
type: docs
url: /de/net/aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/
---
## OoxmlSaveOptions.EmbedOoxmlAsOleObject property

Gibt an, ob Ooxml-Dateien von OleObject als OLE-Objekt eingebettet werden.

```csharp
public bool EmbedOoxmlAsOleObject { get; set; }
```

### Hinweise

Nur für OleObject.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyEmbedOoxmlAsOleObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OLE Object Embedding");
            
            // Erstelle OOXML‑Speicheroptionen und setze EmbedOoxmlAsOleObject
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EmbedOoxmlAsOleObject = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML embedded as OLE object.");
        }
    }
}
```

### Siehe auch

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


