---
title: "Classe FileFormatUtil"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.FileFormatUtil. Fornisce metodi di utilità per convertire gli enum di formato file in stringhe o estensioni di file e viceversa"
type: docs
url: /it/net/aspose.cells/fileformatutil/
---
## FileFormatUtil class

Fornisce metodi di utilità per convertire gli enum di formato file in stringhe o estensioni di file e viceversa.

```csharp
public class FileFormatUtil
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat)(Stream) | Rileva e restituisce le informazioni sul formato di un file Excel memorizzato in uno stream. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_2)(string) | Rileva e restituisce le informazioni sul formato di un file Excel memorizzato in un file. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_1)(Stream, string) | Rileva e restituisce le informazioni sul formato di un file Excel memorizzato in uno stream. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_3)(string, string) | Rileva e restituisce le informazioni sul formato di un file Excel memorizzato in un file. |
| static [ExtensionToSaveFormat](../../aspose.cells/fileformatutil/extensiontosaveformat/)(string) | Converte l'estensione del nome file in un valore SaveFormat. |
| static [FileFormatToSaveFormat](../../aspose.cells/fileformatutil/fileformattosaveformat/)(FileFormatType) | Conversione del formato file in formato di salvataggio. |
| static [IsTemplateFormat](../../aspose.cells/fileformatutil/istemplateformat/)(string) | Restituisce true se l'estensione è .xlt, .xltX, .xltm, .ots. |
| static [LoadFormatToExtension](../../aspose.cells/fileformatutil/loadformattoextension/)(LoadFormat) | Converte un valore enumerato di LoadFormat in un'estensione di file. |
| static [LoadFormatToSaveFormat](../../aspose.cells/fileformatutil/loadformattosaveformat/)(LoadFormat) | Converte un valore LoadFormat in un valore SaveFormat, se possibile. |
| static [SaveFormatToExtension](../../aspose.cells/fileformatutil/saveformattoextension/)(SaveFormat) | Converte un valore enumerato di SaveFormat in un'estensione di file. |
| static [SaveFormatToLoadFormat](../../aspose.cells/fileformatutil/saveformattoloadformat/)(SaveFormat) | Converte un valore SaveFormat in un valore LoadFormat, se possibile. |
| static [VerifyPassword](../../aspose.cells/fileformatutil/verifypassword/)(Stream, string) | Rileva e restituisce le informazioni sul formato di un file Excel memorizzato in uno stream. |

### Esempi

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
            
            // Rileva il formato del file
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            Console.WriteLine("Detected file format: " + info.FileFormatType);
            
            // Verifica il formato del file con Workbook
            Workbook workbook = new Workbook(filePath);
            Console.WriteLine("Workbook file format: " + workbook.FileFormat);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


