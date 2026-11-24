---
title: "CopyOptions.ReferToDestinationSheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CopyOptions-Eigenschaft. Beim Kopieren des Bereichs in derselben Datei und wenn das Diagramm auf das Quellblatt verweist, bedeutet False, dass die Datenquelle des kopierten Diagramms nicht geändert wird. True bedeutet, dass die Datenquelle des kopierten Diagramms auf das Zielblatt verweist."
type: docs
url: /de/net/aspose.cells/copyoptions/refertodestinationsheet/
---
## CopyOptions.ReferToDestinationSheet property

Beim Kopieren des Bereichs in derselben Datei und wenn das Diagramm auf das Quellblatt verweist, bedeutet False, dass die Datenquelle des kopierten Diagramms nicht geändert wird. True bedeutet, dass die Datenquelle des kopierten Diagramms auf das Zielblatt verweist.

```csharp
public bool ReferToDestinationSheet { get; set; }
```

### Hinweise

Der Standardwert ist false, es funktioniert wie MS Excel. Zum Beispiel: Wenn ein Diagramm mit der Datenquelle "sheet1!A1:B10" von Arbeitsblatt "sheet1" in ein anderes Arbeitsblatt "sheet2" kopiert wird, wird die Datenquelle zu "sheet2!A1:B10" geändert.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToDestinationSheetDemo
    {
        public static void Run()
        {
            // Erstelle eine Quell-Arbeitsmappe mit Beispieldaten.
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B1"].PutValue(100);
            sourceSheet.Cells["A2"].PutValue("=SUM(B1)");

            // Erstelle Ziel‑Arbeitsbuch
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets.Add("DestinationSheet");

            // Setze Kopieroptionen mit ReferToDestinationSheet.
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ReferToDestinationSheet = true;

            // Arbeitsblatt mit den Optionen kopieren.
            destSheet.Copy(sourceSheet, copyOptions);

            // Ergebnis speichern
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


