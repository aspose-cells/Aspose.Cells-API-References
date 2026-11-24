---
title: "Klasse FileFormatInfo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FileFormatInfo-Klasse. Enthält Daten, die von den Dateiformat-Erkennungsmethoden der FileFormatUtil zurückgegeben werden."
type: docs
url: /de/net/aspose.cells/fileformatinfo/
---
## FileFormatInfo class

Enthält Daten, die von den Dateiformat-Erkennungsmethoden von [`FileFormatUtil`](../fileformatutil/) zurückgegeben werden.

```csharp
public class FileFormatInfo
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [FileFormatInfo](fileformatinfo/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FileFormatType](../../aspose.cells/fileformatinfo/fileformattype/) { get; } | Ermittelt das erkannte Dateiformat. |
| [IsEncrypted](../../aspose.cells/fileformatinfo/isencrypted/) { get; } | Gibt true zurück, wenn das Dokument verschlüsselt ist und ein Passwort zum Öffnen benötigt. |
| [IsProtectedByRMS](../../aspose.cells/fileformatinfo/isprotectedbyrms/) { get; } | Gibt an, ob die Datei durch den Microsoft Rights Management Server geschützt ist. |
| [LoadFormat](../../aspose.cells/fileformatinfo/loadformat/) { get; } | Ermittelt das erkannte Ladeformat. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatInfoDemo
    {
        public static void FileFormatInfoExample()
        {
            // Lade eine Beispieldatei, um ihr Format zu erkennen
            string filePath = "sample.xlsx";
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat(filePath);

            // Dateiformatinformationen anzeigen
            Console.WriteLine("File Format Information:");
            Console.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
            Console.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
            Console.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
            Console.WriteLine($"Load Format: {fileInfo.LoadFormat}");

            // Speichere die Informationen in einer Textdatei
            string outputFilePath = "FileFormatInfo.txt";
            using (System.IO.StreamWriter writer = new System.IO.StreamWriter(outputFilePath))
            {
                writer.WriteLine("File Format Information:");
                writer.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
                writer.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
                writer.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
                writer.WriteLine($"Load Format: {fileInfo.LoadFormat}");
            }

            Console.WriteLine($"File format information saved to {outputFilePath}");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


