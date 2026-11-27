---
title: "OoxmlSaveOptions.EmbedOoxmlAsOleObject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OoxmlSaveOptions egenskap. Anger om Ooxml-filer för OleObject ska bäddas in som ole-objekt"
type: docs
url: /sv/net/aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/
---
## OoxmlSaveOptions.EmbedOoxmlAsOleObject property

Anger om Ooxml‑filer för OleObject bäddas in som OLE‑objekt.

```csharp
public bool EmbedOoxmlAsOleObject { get; set; }
```

### Anmärkningar

Endast för OleObject.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyEmbedOoxmlAsOleObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OLE Object Embedding");
            
            // Skapa OOXML-sparalternativ och sätt EmbedOoxmlAsOleObject
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EmbedOoxmlAsOleObject = true;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML embedded as OLE object.");
        }
    }
}
```

### Se även

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


