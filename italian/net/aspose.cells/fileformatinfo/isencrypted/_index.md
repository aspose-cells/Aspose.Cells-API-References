---
title: "FileFormatInfo.IsEncrypted"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FileFormatInfo. Restituisce true se il documento è crittografato e richiede una password per l'apertura"
type: docs
url: /it/net/aspose.cells/fileformatinfo/isencrypted/
---
## FileFormatInfo.IsEncrypted property

Restituisce true se il documento è crittografato e richiede una password per l'apertura.

```csharp
public bool IsEncrypted { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // Rileva il formato del file non crittografato
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat("example.xlsx");
            Console.WriteLine("Is file encrypted? " + fileInfo.IsEncrypted);

            // Rileva il formato del file crittografato
            FileFormatInfo encryptedFileInfo = FileFormatUtil.DetectFileFormat("encrypted.xlsx");
            Console.WriteLine("Is encrypted file encrypted? " + encryptedFileInfo.IsEncrypted);

            // Carica il file crittografato con password
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.Password = "password";
            Workbook workbook = new Workbook("encrypted.xlsx", loadOptions);
            Console.WriteLine("Encrypted file loaded successfully");
        }
    }
}
```

### Vedi anche

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


