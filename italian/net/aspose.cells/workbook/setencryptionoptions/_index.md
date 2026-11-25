---
title: "Workbook.SetEncryptionOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Imposta le Opzioni di Cifratura"
type: docs
url: /it/net/aspose.cells/workbook/setencryptionoptions/
---
## Workbook.SetEncryptionOptions method

Imposta le opzioni di crittografia.

```csharp
public void SetEncryptionOptions(EncryptionType encryptionType, int keyLength)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| encryptionType | EncryptionType | Il tipo di cifratura. |
| keyLength | Int32 | La lunghezza della chiave. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetEncryptionOptionsWithEncryptionTypeInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni dati al worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Encryption");
            
            // Imposta la password e le opzioni di cifratura
            workbook.Settings.Password = "1234";
            workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
            
            // Salva il workbook cifrato
            workbook.Save("EncryptedWorkbook.xls", SaveFormat.Excel97To2003);
            
            // Verifica caricando il workbook cifrato
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "1234";
            Workbook encryptedWorkbook = new Workbook("EncryptedWorkbook.xls", loadOptions);
            
            Console.WriteLine("Workbook encrypted and loaded successfully.");
        }
    }
}
```

### Vedi anche

* enum [EncryptionType](../../encryptiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


