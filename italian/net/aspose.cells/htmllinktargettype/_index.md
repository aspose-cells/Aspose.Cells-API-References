---
title: "Enum HtmlLinkTargetType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.HtmlLinkTargetType. Rappresenta il tipo di attributo target nel tag HTML"
type: docs
url: /it/net/aspose.cells/htmllinktargettype/
---
## HtmlLinkTargetType enumeration

Rappresenta il tipo di attributo target nel tag HTML.

```csharp
public enum HtmlLinkTargetType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Blank | `0` | Apre il documento collegato in una nuova finestra o scheda |
| Parent | `1` | Apre il documento collegato nel frame genitore |
| Self | `2` | Apre il documento collegato nello stesso frame in cui è stato cliccato (questo è il valore predefinito) |
| Top | `3` | Apre il documento collegato nell'intero corpo della finestra |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLinkTargetTypeDemo
    {
        public static void HtmlLinkTargetTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Click here to visit Aspose");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Crea HtmlSaveOptions e imposta il LinkTargetType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank; // Opens the link in a new window or tab

            // Salva la cartella di lavoro in formato HTML
            workbook.Save("HtmlLinkTargetTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with link target type set to '_blank'.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


