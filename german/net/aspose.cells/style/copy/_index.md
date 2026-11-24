---
title: "Style.Copy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Methode. Kopiert Daten aus einem anderen Style-Objekt"
type: docs
url: /de/net/aspose.cells/style/copy/
---
## Style.Copy method

Kopiert Daten von einem anderen Stilobjekt

```csharp
public void Copy(Style style)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Quell-Style-Objekt |

### Hinweise

Diese Methode kopiert den Namen des Styles nicht. Wenn Sie den Namen kopieren möchten, rufen Sie bitte nach dem Kopieren des Styles den folgenden Code auf: destStyle.Name = style.Name.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCopyWithStyleDemo
    {
        public static void Run()
        {
            // Erstelle eine Quell-Arbeitsmappe mit Beispieldaten.
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Sample Text");
            Style srcStyle = srcWorkbook.CreateStyle();
            srcStyle.Font.Name = "Arial";
            srcStyle.Font.Size = 14;
            srcSheet.Cells["A1"].SetStyle(srcStyle);

            // Erstelle Ziel‑Arbeitsbuch
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Kopieren Sie den Style von der Quelle zum Ziel.
            Style destStyle = destWorkbook.CreateStyle();
            destStyle.Copy(srcStyle);
            
            // Wenden Sie den kopierten Style an.
            destSheet.Cells["B2"].PutValue("Copied Style Text");
            destSheet.Cells["B2"].SetStyle(destStyle);

            // Ergebnis speichern
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


