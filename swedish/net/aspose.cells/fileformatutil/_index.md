---
title: "Klass FileFormatUtil"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FileFormatUtil-klass. Tillhandahåller hjälpfunktioner för att konvertera filformat‑enum till strängar eller filändelser och tillbaka"
type: docs
url: /sv/net/aspose.cells/fileformatutil/
---
## FileFormatUtil class

Tillhandahåller hjälpfunktioner för att konvertera filformat‑enum till strängar eller filändelser och tillbaka.

```csharp
public class FileFormatUtil
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat)(Stream) | Detekterar och returnerar information om ett Excel-format som lagras i en ström. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_2)(string) | Detekterar och returnerar information om ett Excel-format som lagras i en fil. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_1)(Stream, string) | Detekterar och returnerar information om ett Excel-format som lagras i en ström. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_3)(string, string) | Detekterar och returnerar information om ett Excel-format som lagras i en fil. |
| static [ExtensionToSaveFormat](../../aspose.cells/fileformatutil/extensiontosaveformat/)(string) | Konverterar en filnamnsändelse till ett SaveFormat‑värde. |
| static [FileFormatToSaveFormat](../../aspose.cells/fileformatutil/fileformattosaveformat/)(FileFormatType) | Konverterar filformat till sparaformat. |
| static [IsTemplateFormat](../../aspose.cells/fileformatutil/istemplateformat/)(string) | Returnerar true om ändelsen är .xlt, .xltX, .xltm, .ots. |
| static [LoadFormatToExtension](../../aspose.cells/fileformatutil/loadformattoextension/)(LoadFormat) | Konverterar ett LoadFormat‑enumererat värde till en filändelse. |
| static [LoadFormatToSaveFormat](../../aspose.cells/fileformatutil/loadformattosaveformat/)(LoadFormat) | Konverterar ett LoadFormat‑värde till ett SaveFormat‑värde om möjligt. |
| static [SaveFormatToExtension](../../aspose.cells/fileformatutil/saveformattoextension/)(SaveFormat) | Konverterar ett SaveFormat‑enumererat värde till en filändelse. |
| static [SaveFormatToLoadFormat](../../aspose.cells/fileformatutil/saveformattoloadformat/)(SaveFormat) | Konverterar ett SaveFormat‑värde till ett LoadFormat‑värde om möjligt. |
| static [VerifyPassword](../../aspose.cells/fileformatutil/verifypassword/)(Stream, string) | Detekterar och returnerar information om ett Excel-format som lagras i en ström. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFileFormatUtilDemo
    {
        public static void Run()
        {
            string filePath = "example.xlt";
            
            // Detektera filformat
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            Console.WriteLine("Detected file format: " + info.FileFormatType);
            
            // Verifiera filformat med Workbook
            Workbook workbook = new Workbook(filePath);
            Console.WriteLine("Workbook file format: " + workbook.FileFormat);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


