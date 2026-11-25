---
title: "StreamProviderOptions.StreamProviderOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore di StreamProviderOptions. Inizializza una nuova istanza della classe StreamProviderOptions"
type: docs
url: /it/net/aspose.cells/streamprovideroptions/streamprovideroptions/
---
## StreamProviderOptions(ResourceLoadingType, string) {#constructor_1}

Inizializza una nuova istanza della classe [`StreamProviderOptions`](../).

```csharp
public StreamProviderOptions(ResourceLoadingType loadingType, string defaultPath)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadingType | ResourceLoadingType | Il tipo per caricare la risorsa collegata. |
| defaultPath | String | Il percorso predefinito. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Microsoft.VisualBasic;
    using System;

    public class StreamProviderOptionsMethodCtorWithResourceLoadingTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("file1.xlsx");
            workbook.Settings.ResourceProvider = new StreamProvider();
            foreach (Shape shape in workbook.Worksheets[0].Shapes)
            {
                shape.ToImage("out.png", null);
            }            
        }
    }

    class StreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            options.Stream = File.OpenRead("example.jpg");
            options.ResourceLoadingType = ResourceLoadingType.UserProvided;
        }
        public void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
            }
        }
    }
}
```

### Vedi anche

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## StreamProviderOptions() {#constructor}

Inizializza una nuova istanza della classe [`StreamProviderOptions`](../).

```csharp
public StreamProviderOptions()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class StreamProviderOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Dimostra il costruttore senza parametri
                StreamProviderOptions options = new StreamProviderOptions();
                Console.WriteLine("Parameterless constructor:");
                Console.WriteLine($"ResourceLoadingType: {options.ResourceLoadingType}");
                Console.WriteLine($"DefaultPath: {options.DefaultPath}");

                // Crea una cartella di lavoro e salva con le opzioni di stream
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].PutValue("StreamProviderOptions Demo");
                
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                string outputDir = "custom_path/";
                saveOptions.StreamProvider = new ExportStreamProvider(outputDir);
                
                workbook.Save("StreamProviderOptionsDemo.html", saveOptions);
                Console.WriteLine("\nWorkbook saved with custom stream options");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StreamProviderOptions constructor demo: {ex.Message}");
            }
        }
    }

    internal class ExportStreamProvider : IStreamProvider
    {
        private string outputDir;

        public ExportStreamProvider(string dir)
        {
            outputDir = dir;
        }

        public void InitStream(StreamProviderOptions options)
        {
            if (options.DefaultPath == null)
            {
                options.Stream = new MemoryStream();
            }
            else
            {
                string path = outputDir + Path.GetFileName(options.DefaultPath);
                options.CustomPath = path;
                Directory.CreateDirectory(Path.GetDirectoryName(path));
                options.Stream = File.Create(path);
            }
        }

        public void CloseStream(StreamProviderOptions options)
        {
            if (options != null && options.Stream != null)
            {
                options.Stream.Close();
            }
        }
    }
}
```

### Vedi anche

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


