---
title: "HtmlSaveOptions.SaveAsSingleFile"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob das HTML als einzelne Datei gespeichert wird. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/saveassinglefile/
---
## HtmlSaveOptions.SaveAsSingleFile property

Gibt an, ob die HTML als einzelne Datei gespeichert wird. Der Standardwert ist false.

```csharp
public bool SaveAsSingleFile { get; set; }
```

### Hinweise

Wenn das Arbeitsbuch mehrere Arbeitsblätter oder andere erforderliche Ressourcen wie Bilder enthält, müssen diese Arbeitsblätter und Ressourcen in der Regel in separaten Dateien gespeichert werden. Für einige Szenarien benötigt der Benutzer möglicherweise nur eine einzige Ergebnisdatei, beispielsweise zum bequemen Transfer. In diesem Fall kann der Benutzer diese Eigenschaft auf true setzen.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertySaveAsSingleFileDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // HTML‑Speicheroptionen initialisieren
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.SaveAsSingleFile = true;
            saveOptions.ExportPageHeaders = true;
            
            // Speichern Sie das Arbeitsbuch als einzelne HTML-Datei
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            // Überprüfen Sie, ob die Ausgabedatei existiert
            if (File.Exists(outputPath))
            {
                Console.WriteLine("HTML saved as single file successfully.");
            }
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


