---
title: "HtmlLoadOptions.HasFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlLoadOptions-Eigenschaft. Gibt an, ob der Text eine Formel ist, wenn er beginnt mit"
type: docs
url: /de/net/aspose.cells/htmlloadoptions/hasformula/
---
## HtmlLoadOptions.HasFormula property

Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt.

```csharp
public bool HasFormula { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // HTML-Ladeoptionen erstellen
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Setze HasFormula auf false, um Formelzeichenketten als Klartext zu behandeln
            loadOptions.HasFormula = false;
            
            // Arbeitsmappe mit HTML-Datei und Ladeoptionen erstellen
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Einige Zellwerte anzeigen, um den HTML-Import zu demonstrieren
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            
            // Als XLSX speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


