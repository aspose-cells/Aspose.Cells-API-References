---
title: "HtmlSaveOptions.CellNameAttribute"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt das Attribut an, das den zu schreibenden CellName angibt. z. B. Wenn der Wert id ist, wird für Zelle A1 die Ausgabe td idA1 sein. Der Standardwert ist null."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/cellnameattribute/
---
## HtmlSaveOptions.CellNameAttribute property

Gibt das Attribut an, das den zu schreibenden Zellnamen kennzeichnet. (z. B. Wenn der Wert "id" ist, wird für die Zelle "A1" die Ausgabe &lt;td id='A1'&gt; sein). Der Standardwert ist null.

```csharp
public string CellNameAttribute { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using System.Text.RegularExpressions;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellNameAttributeDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch mit einigen Daten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["B2"].PutValue(123);

            // Setze HTML-Speicheroptionen mit CellNameAttribute
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellNameAttribute = "id";
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.ExportActiveWorksheetOnly = true;

            // In HTML-Datei speichern
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            // Überprüfe, ob die HTML-Ausgabe Zell-IDs enthält
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains A1 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='A1'"));
            Console.WriteLine("HTML contains B2 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='B2'"));
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


