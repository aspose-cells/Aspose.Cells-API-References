---
title: "Classe FileFormatInfo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.FileFormatInfo. Contiene i dati restituiti dai metodi di rilevamento del formato file di FileFormatUtil"
type: docs
url: /it/net/aspose.cells/fileformatinfo/
---
## FileFormatInfo class

Contiene i dati restituiti dai metodi di rilevamento del formato file di [`FileFormatUtil`](../fileformatutil/).

```csharp
public class FileFormatInfo
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [FileFormatInfo](fileformatinfo/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FileFormatType](../../aspose.cells/fileformatinfo/fileformattype/) { get; } | Ottiene il formato file rilevato. |
| [IsEncrypted](../../aspose.cells/fileformatinfo/isencrypted/) { get; } | Restituisce true se il documento è crittografato e richiede una password per l'apertura. |
| [IsProtectedByRMS](../../aspose.cells/fileformatinfo/isprotectedbyrms/) { get; } | Indica se il file è protetto da Microsoft Rights Management Server. |
| [LoadFormat](../../aspose.cells/fileformatinfo/loadformat/) { get; } | Ottiene il formato di caricamento rilevato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatInfoDemo
    {
        public static void FileFormatInfoExample()
        {
            // Carica un file di esempio per rilevarne il formato
            string filePath = "sample.xlsx";
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat(filePath);

            // Visualizza le informazioni sul formato file
            Console.WriteLine("File Format Information:");
            Console.WriteLine($"Is Protected By RMS: {fileInfo.IsProtectedByRMS}");
            Console.WriteLine($"Is Encrypted: {fileInfo.IsEncrypted}");
            Console.WriteLine($"File Format Type: {fileInfo.FileFormatType}");
            Console.WriteLine($"Load Format: {fileInfo.LoadFormat}");

            // Salva le informazioni in un file di testo
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

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


