---
title: "StreamProviderOptions.StreamProviderOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StreamProviderOptions-Konstruktor. Erstellt eine neue Instanz der StreamProviderOptions-Klasse"
type: docs
url: /de/net/aspose.cells/streamprovideroptions/streamprovideroptions/
---
## StreamProviderOptions(ResourceLoadingType, string) {#constructor_1}

Erstellt eine neue Instanz der [`StreamProviderOptions`](../)-Klasse.

```csharp
public StreamProviderOptions(ResourceLoadingType loadingType, string defaultPath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loadingType | ResourceLoadingType | Der Typ, um die verknüpfte Ressource zu laden. |
| defaultPath | String | Der Standardpfad. |

### Beispiele

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

### Siehe auch

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## StreamProviderOptions() {#constructor}

Erstellt eine neue Instanz der [`StreamProviderOptions`](../)-Klasse.

```csharp
public StreamProviderOptions()
```

### Beispiele

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
                // Demonstration des parameterlosen Konstruktors
                StreamProviderOptions options = new StreamProviderOptions();
                Console.WriteLine("Parameterless constructor:");
                Console.WriteLine($"ResourceLoadingType: {options.ResourceLoadingType}");
                Console.WriteLine($"DefaultPath: {options.DefaultPath}");

                // Erstelle eine Arbeitsmappe und speichere sie mit Stream-Optionen
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

### Siehe auch

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


