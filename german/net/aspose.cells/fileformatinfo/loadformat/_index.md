---
title: "FileFormatInfo.LoadFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FileFormatInfo Eigenschaft. Gibt das erkannte Ladeformat zurück"
type: docs
url: /de/net/aspose.cells/fileformatinfo/loadformat/
---
## FileFormatInfo.LoadFormat property

Ermittelt das erkannte Ladeformat.

```csharp
public LoadFormat LoadFormat { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // Der Pfad zum Dokumentenverzeichnis.
            string filePath = "data/";
            
            // Dateiformat erkennen
            string fileName = "SAMPLE_XLS_ISSUE.XLS";
            var fileFormatInfo = FileFormatUtil.DetectFileFormat(filePath + fileName);
            Console.WriteLine("Detected LoadFormat: " + fileFormatInfo.LoadFormat);

            // Datei mit dem korrekten Format laden
            LoadOptions loadOptions = new LoadOptions(LoadFormat.MHtml);
            var workbook = new Workbook(filePath + fileName, loadOptions);
            
            // Arbeitsmappe verarbeiten
            workbook.Worksheets[0].AutoFitColumns();
            workbook.Save(filePath + "output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [LoadFormat](../../loadformat/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


