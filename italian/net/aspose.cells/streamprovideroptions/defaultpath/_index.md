---
title: "StreamProviderOptions.DefaultPath"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StreamProviderOptions. L'URL del percorso predefinito salvato nel file HTML generato per la fonte di riferimento. Per esempio i dati del foglio salvati in xxx_files/sheet001.htm, l'URL utilizzato nel file HTML principale dovrebbe essere simile a srcxxx_files/sheet001.htm"
type: docs
url: /it/net/aspose.cells/streamprovideroptions/defaultpath/
---
## StreamProviderOptions.DefaultPath property

Il percorso predefinito (URL) salvato nel file html generato per la sorgente di riferimento. Ad esempio, i dati del foglio salvati in xxx_files/sheet001.htm, l'url usato nel file html principale dovrebbe essere così \"src=\\\"xxx_files/sheet001.htm\\\"\"

```csharp
public string DefaultPath { get; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyDefaultPathDemo
    {
        public static void Run()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();
            
            // Crea StreamProviderOptions con ResourceLoadingType e DefaultPath
            StreamProviderOptions options = new StreamProviderOptions(ResourceLoadingType.Default, "1.DefaultPathExample");
            
            // Dimostra l'uso di DefaultPath
            Console.WriteLine("StreamProviderOptions DefaultPath: " + options.DefaultPath);
            
            // Esempio di utilizzo delle opzioni con uno stream (dimostrazione semplificata)
            using (MemoryStream stream = new MemoryStream())
            {
                options.Stream = stream;
                
                if (options.DefaultPath.IndexOf("1.") >= 0)
                {
                    Console.WriteLine("Processing stream for path: " + options.DefaultPath);
                    // Esegui operazioni con lo stream
                    workbook.Save(stream, SaveFormat.Xlsx);
                }
            }
        }
    }
}
```

### Vedi anche

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


