---
title: "Enum JsonExportHyperlinkType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Json.JsonExportHyperlinkType enum. Rappresenta il tipo di esportazione dei collegamenti ipertestuali in json"
type: docs
url: /it/net/aspose.cells.json/jsonexporthyperlinktype/
---
## JsonExportHyperlinkType enumeration

Rappresenta il tipo di esportazione dei collegamenti ipertestuali in json.

```csharp
public enum JsonExportHyperlinkType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DisplayString | `0` | Esporta stringa di visualizzazione |
| Address | `1` | Esporta URL |
| HtmlString | `2` | Esporta come stringa HTML. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Json;
    using System;

    public class JsonExportHyperlinkTypeDemo
    {
        public static void JsonExportHyperlinkTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio con collegamenti ipertestuali
            worksheet.Cells["A1"].PutValue("Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.google.com");

            worksheet.Cells["A2"].PutValue("Aspose");
            worksheet.Hyperlinks.Add("A2", 1, 1, "http://www.aspose.com");

            // Crea JsonSaveOptions e imposta ExportHyperlinkType
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.DisplayString;

            // Salva la cartella di lavoro in formato JSON
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksDisplayString.json", saveOptions);

            // Modifica ExportHyperlinkType in Address e salva di nuovo
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.Address;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksAddress.json", saveOptions);

            // Modifica ExportHyperlinkType in HtmlString e salva di nuovo
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksHtmlString.json", saveOptions);

            Console.WriteLine("Workbooks saved with different hyperlink export types.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Json](../../aspose.cells.json/)
* assembly [Aspose.Cells](../../)


