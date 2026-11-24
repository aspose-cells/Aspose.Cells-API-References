---
title: "PasteOptions.IgnoreLinksToOriginalFile"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PasteOptions-Eigenschaft. Ignoriere Links zur Originaldatei"
type: docs
url: /de/net/aspose.cells/pasteoptions/ignorelinkstooriginalfile/
---
## PasteOptions.IgnoreLinksToOriginalFile property

Ignoriere Links zur Originaldatei.

```csharp
public bool IgnoreLinksToOriginalFile { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyIgnoreLinksToOriginalFileDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet src = workbook.Worksheets[0];
            
            // Beispieldaten mit Formeln erstellen, die möglicherweise auf die Originaldatei verweisen
            src.Cells["A1"].PutValue("Header1");
            src.Cells["B1"].PutValue("Header2");
            src.Cells["A2"].PutValue(100);
            src.Cells["B2"].PutValue("=A2*2");  // Simple formula
            src.Cells["A3"].PutValue(200);
            src.Cells["B3"].PutValue("=A3*2");

            // Zielarbeitsblatt und -bereich erstellen
            Worksheet dst = workbook.Worksheets.Add("Destination");
            Aspose.Cells.Range srcRange = src.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range dstRange = dst.Cells.CreateRange("A1:B3");

            // Paste-Optionen konfigurieren, um Links zur Originaldatei zu ignorieren
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.All;
            pasteOptions.IgnoreLinksToOriginalFile = true;

            // Kopieren mit den angegebenen Paste-Optionen
            dstRange.Copy(srcRange, pasteOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("PasteOptions_IgnoreLinksToOriginalFile_Output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


