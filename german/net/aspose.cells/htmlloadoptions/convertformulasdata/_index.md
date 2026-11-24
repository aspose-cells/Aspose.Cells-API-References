---
title: "HtmlLoadOptions.ConvertFormulasData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlLoadOptions-Eigenschaft. Wenn true, wird ein String in eine Formel konvertiert, wenn der Stringwert mit einem Zeichen beginnt; der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmlloadoptions/convertformulasdata/
---
## HtmlLoadOptions.ConvertFormulasData property

Wenn true, wird ein String in eine Formel konvertiert, wenn der Stringwert mit dem Zeichen '=', beginnt; der Standardwert ist false.

```csharp
[Obsolete("Use HtmlLoadOptions.HasFormula property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ConvertFormulasData { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Stattdessen verwenden Sie bitte die HtmlLoadOptions.HasFormula-Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit März 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyConvertFormulasDataDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // ConvertFormulasData-Eigenschaft auf true setzen
            options.ConvertFormulasData = true;

            // Laden Sie eine HTML-Datei in ein Arbeitsbuch mit den angegebenen Optionen
            Workbook workbook = new Workbook("input.html", options);

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Zellwerte anzeigen, um die Formelkonvertierung zu demonstrieren
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell B1 formula: " + worksheet.Cells["B1"].Formula);

            // Speichere die Arbeitsmappe in einer Excel‑Datei
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


