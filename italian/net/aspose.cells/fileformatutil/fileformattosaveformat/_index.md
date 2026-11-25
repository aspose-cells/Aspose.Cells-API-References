---
title: "FileFormatUtil.FileFormatToSaveFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FileFormatUtil. Conversione del formato file al formato di salvataggio."
type: docs
url: /it/net/aspose.cells/fileformatutil/fileformattosaveformat/
---
## FileFormatUtil.FileFormatToSaveFormat method

Conversione del formato file in formato di salvataggio.

```csharp
public static SaveFormat FileFormatToSaveFormat(FileFormatType format)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formato | FileFormatType | Il tipo di formato file. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodFileFormatToSaveFormatWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test FileFormatToSaveFormat");

            // Ottieni il tipo di formato file della cartella di lavoro
            FileFormatType originalFormat = workbook.FileFormat;

            // Converti FileFormatType in SaveFormat
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(originalFormat);

            // Salva la cartella di lavoro usando il SaveFormat convertito
            string outputPath = "Output_" + saveFormat.ToString() + ".xlsx";
            workbook.Save(outputPath, saveFormat);

            Console.WriteLine("File saved successfully with SaveFormat: " + saveFormat);
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* enum [FileFormatType](../../fileformattype/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


