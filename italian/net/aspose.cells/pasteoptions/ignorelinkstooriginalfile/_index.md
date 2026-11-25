---
title: "PasteOptions.IgnoreLinksToOriginalFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PasteOptions. Ignora i collegamenti al file originale"
type: docs
url: /it/net/aspose.cells/pasteoptions/ignorelinkstooriginalfile/
---
## PasteOptions.IgnoreLinksToOriginalFile property

Ignora i collegamenti al file originale.

```csharp
public bool IgnoreLinksToOriginalFile { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyIgnoreLinksToOriginalFileDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet src = workbook.Worksheets[0];
            
            // Crea dati di esempio con formule che potrebbero collegarsi al file originale
            src.Cells["A1"].PutValue("Header1");
            src.Cells["B1"].PutValue("Header2");
            src.Cells["A2"].PutValue(100);
            src.Cells["B2"].PutValue("=A2*2");  // Simple formula
            src.Cells["A3"].PutValue(200);
            src.Cells["B3"].PutValue("=A3*2");

            // Crea foglio di lavoro di destinazione e intervallo
            Worksheet dst = workbook.Worksheets.Add("Destination");
            Aspose.Cells.Range srcRange = src.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range dstRange = dst.Cells.CreateRange("A1:B3");

            // Configura le opzioni di incolla per ignorare i collegamenti al file originale
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.All;
            pasteOptions.IgnoreLinksToOriginalFile = true;

            // Copia con le opzioni di incolla specificate
            dstRange.Copy(srcRange, pasteOptions);

            // Salva la cartella di lavoro
            workbook.Save("PasteOptions_IgnoreLinksToOriginalFile_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


