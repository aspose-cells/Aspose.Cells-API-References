---
title: "Enum ResourceLoadingType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ResourceLoadingType enum. Rappresenta come caricare la risorsa collegata"
type: docs
url: /it/net/aspose.cells/resourceloadingtype/
---
## ResourceLoadingType enumeration

Rappresenta come caricare la risorsa collegata.

```csharp
public enum ResourceLoadingType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Default | `0` | Carica questa risorsa come al solito. |
| Skip | `1` | Salta il caricamento di questa risorsa. |
| UserProvided | `2` | Usa lo stream fornito dall'utente |

### Esempi

```csharp
using Aspose.Cells;
using System;
using System.IO;

namespace AsposeCellsExamples
{
    public class ResourceLoadingTypeDemo
    {
        public static void ResourceLoadingTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Resource");
            worksheet.Cells["A2"].PutValue("Default");
            worksheet.Cells["A3"].PutValue("Skip");
            worksheet.Cells["A4"].PutValue("UserProvided");

            // Salva la cartella di lavoro in HTML con un provider di stream personalizzato
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                StreamProvider = new CustomStreamProvider()
            };

            workbook.Save("ResourceLoadingTypeExample.html", saveOptions);
        }
    }

    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Fornisci uno stream personalizzato per la risorsa
                options.Stream = new MemoryStream();
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Salta il caricamento della risorsa
                options.Stream = Stream.Null;
            }
            else
            {
                // Carica la risorsa come al solito
                options.Stream = new FileStream(options.DefaultPath, FileMode.Open, FileAccess.Read);
            }
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Chiudi lo stream se non è nullo
            options.Stream?.Close();
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


