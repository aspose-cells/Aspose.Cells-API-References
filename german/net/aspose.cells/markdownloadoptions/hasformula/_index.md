---
title: "MarkdownLoadOptions.HasFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MarkdownLoadOptions-Eigenschaft. Gibt an, ob der Text eine Formel ist, wenn er mit"
type: docs
url: /de/net/aspose.cells/markdownloadoptions/hasformula/
---
## MarkdownLoadOptions.HasFormula property

Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt.

```csharp
public bool HasFormula { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Eine Instanz von MarkdownLoadOptions erstellen
                MarkdownLoadOptions options = new MarkdownLoadOptions();

                // Zeigen Sie den Standardwert von HasFormula an
                Console.WriteLine($"Default HasFormula value: {options.HasFormula}");

                // Setzen Sie HasFormula auf true
                options.HasFormula = true;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Setzen Sie HasFormula auf false
                options.HasFormula = false;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Erstellen Sie eine Arbeitsmappe mit Beispiel-Markdown-Inhalt
                Workbook workbook = new Workbook();

                // Speichern Sie die Arbeitsmappe, um zu demonstrieren, dass die Optionen verwendet werden können
                workbook.Save("HasFormulaDemo.xlsx");

                Console.WriteLine("HasFormula property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [MarkdownLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


