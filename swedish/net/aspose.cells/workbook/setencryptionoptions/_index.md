---
title: "Workbook.SetEncryptionOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Ställ in krypteringsalternativ"
type: docs
url: /sv/net/aspose.cells/workbook/setencryptionoptions/
---
## Workbook.SetEncryptionOptions method

Ställ in krypteringsalternativ.

```csharp
public void SetEncryptionOptions(EncryptionType encryptionType, int keyLength)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| encryptionType | EncryptionType | Krypteringstypen. |
| keyLength | Int32 | Nyckellängden. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetEncryptionOptionsWithEncryptionTypeInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till lite data i kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Encryption");
            
            // Ange lösenord och krypteringsalternativ
            workbook.Settings.Password = "1234";
            workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
            
            // Spara den krypterade arbetsboken
            workbook.Save("EncryptedWorkbook.xls", SaveFormat.Excel97To2003);
            
            // Verifiera genom att läsa in den krypterade arbetsboken
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "1234";
            Workbook encryptedWorkbook = new Workbook("EncryptedWorkbook.xls", loadOptions);
            
            Console.WriteLine("Workbook encrypted and loaded successfully.");
        }
    }
}
```

### Se även

* enum [EncryptionType](../../encryptiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


