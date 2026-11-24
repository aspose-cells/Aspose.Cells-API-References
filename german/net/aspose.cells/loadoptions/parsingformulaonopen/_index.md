---
title: "LoadOptions.ParsingFormulaOnOpen"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Gibt an, ob die Formel beim Lesen der Datei geparst wird"
type: docs
url: /de/net/aspose.cells/loadoptions/parsingformulaonopen/
---
## LoadOptions.ParsingFormulaOnOpen property

Gibt an, ob Formeln beim Lesen der Datei geparst werden.

```csharp
public bool ParsingFormulaOnOpen { get; set; }
```

### Hinweise

Gilt nur für Excel‑Dateien Xlsx, Xltx, Xltm und Xlsm, da die Formeln in den Dateien als Zeichenkettenformel gespeichert sind.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingFormulaOnOpenDemo
    {
        public static void Run()
        {
            // Ladeoptionen erstellen
            LoadOptions loadOptions = new LoadOptions();
            
            // Setze ParsingFormulaOnOpen auf false, um das Parsen von Formeln beim Laden zu überspringen
            loadOptions.ParsingFormulaOnOpen = false;
            
            // Laden Sie die Arbeitsmappe mit den angegebenen Optionen
            Workbook workbook = new Workbook("example.xlsm", loadOptions);
            
            // Arbeitsblatt öffnen und zeigen, dass das Parsen von Formeln übersprungen wurde
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Console.WriteLine("Cell A1 formula: " + cell.Formula);
            Console.WriteLine("Cell A1 value: " + cell.Value);
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


