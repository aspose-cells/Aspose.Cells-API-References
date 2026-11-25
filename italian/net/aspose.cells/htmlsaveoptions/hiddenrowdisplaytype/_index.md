---
title: "HtmlSaveOptions.HiddenRowDisplayType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Riga nascosta: l'altezza di questa riga è 0 in Excel prima di salvarla in formato HTML; se HtmlHiddenRowDisplayType è Remove la riga nascosta non verrà esportata, se il valore è Hidden la riga verrà esportata ma rimarrà nascosta; il valore predefinito è Hidden"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/
---
## HtmlSaveOptions.HiddenRowDisplayType property

Riga nascosta (l'altezza di questa riga è 0) in Excel, prima di salvarla in formato HTML, se HtmlHiddenRowDisplayType è "Remove", la riga nascosta non verrà emessa, se il valore è "Hidden", la riga verrà emessa, ma sarà nascosta, il valore predefinito è "Hidden"

```csharp
public HtmlHiddenRowDisplayType HiddenRowDisplayType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenRowDisplayTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e nascondi una riga
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row");
            worksheet.Cells.HideRow(1); // Hide row 2 (0-based index 1)

            // Imposta le opzioni di salvataggio HTML con HiddenRowDisplayType
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;

            // Salva in HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with hidden rows handled according to HiddenRowDisplayType setting.");
        }
    }
}
```

### Vedi anche

* enum [HtmlHiddenRowDisplayType](../../htmlhiddenrowdisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


