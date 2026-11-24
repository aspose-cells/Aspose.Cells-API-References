---
title: "Klasse FileFormatUtil"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FileFormatUtil-Klasse. Stellt Hilfsmethoden zum Konvertieren von Dateiformat-Enums in Zeichenketten oder Dateierweiterungen und zurück bereit."
type: docs
url: /de/net/aspose.cells/fileformatutil/
---
## FileFormatUtil class

Stellt Hilfsmethoden zum Konvertieren von Dateiformat‑Enums in Zeichenketten oder Dateierweiterungen und zurück bereit.

```csharp
public class FileFormatUtil
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat)(Stream) | Erkennt und gibt die Informationen über das Format einer in einem Stream gespeicherten Excel-Datei zurück. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_2)(string) | Erkennt und gibt die Informationen über das Format einer in einer Datei gespeicherten Excel-Datei zurück. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_1)(Stream, string) | Erkennt und gibt die Informationen über das Format einer in einem Stream gespeicherten Excel-Datei zurück. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_3)(string, string) | Erkennt und gibt die Informationen über das Format einer in einer Datei gespeicherten Excel-Datei zurück. |
| static [ExtensionToSaveFormat](../../aspose.cells/fileformatutil/extensiontosaveformat/)(string) | Konvertiert eine Dateinamenerweiterung in einen SaveFormat-Wert. |
| static [FileFormatToSaveFormat](../../aspose.cells/fileformatutil/fileformattosaveformat/)(FileFormatType) | Konvertiert das Dateiformat in das Speicherformat. |
| static [IsTemplateFormat](../../aspose.cells/fileformatutil/istemplateformat/)(string) | Gibt true zurück, wenn die Erweiterung .xlt, .xltX, .xltm oder .ots ist. |
| static [LoadFormatToExtension](../../aspose.cells/fileformatutil/loadformattoextension/)(LoadFormat) | Konvertiert einen LoadFormat-Enum-Wert in eine Dateierweiterung. |
| static [LoadFormatToSaveFormat](../../aspose.cells/fileformatutil/loadformattosaveformat/)(LoadFormat) | Konvertiert einen LoadFormat-Wert, falls möglich, in einen SaveFormat-Wert. |
| static [SaveFormatToExtension](../../aspose.cells/fileformatutil/saveformattoextension/)(SaveFormat) | Konvertiert einen SaveFormat-Enum-Wert in eine Dateierweiterung. |
| static [SaveFormatToLoadFormat](../../aspose.cells/fileformatutil/saveformattoloadformat/)(SaveFormat) | Konvertiert einen SaveFormat-Wert, falls möglich, in einen LoadFormat-Wert. |
| static [VerifyPassword](../../aspose.cells/fileformatutil/verifypassword/)(Stream, string) | Erkennt und gibt die Informationen über das Format einer in einem Stream gespeicherten Excel-Datei zurück. |

### Beispiele

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
            
            // Dateiformat erkennen
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            Console.WriteLine("Detected file format: " + info.FileFormatType);
            
            // Dateiformat mit Arbeitsmappe überprüfen
            Workbook workbook = new Workbook(filePath);
            Console.WriteLine("Workbook file format: " + workbook.FileFormat);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


