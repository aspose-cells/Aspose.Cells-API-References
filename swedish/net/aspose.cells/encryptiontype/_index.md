---
title: "Enum EncryptionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.EncryptionType enum. Krypteringstyp. Endast använd av excel2003. Vi kommer att kryptera 2007/2010-arbetsboken med SHA AES på samma sätt som Excel gör och denna EncryptionType kommer att ignoreras."
type: docs
url: /sv/net/aspose.cells/encryptiontype/
---
## EncryptionType enumeration

Krypteringstyp. Endast använd av excel2003. Vi kommer att kryptera 2007/2010‑arbetsboken med SHA AES på samma sätt som Excel gör, och denna EncryptionType kommer att ignoreras.

```csharp
public enum EncryptionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| XOR | `0` | XOR-krypteringsalgoritm. |
| Compatible | `1` | Kompatibel med Office 97/2000. |
| EnhancedCryptographicProviderV1 | `2` | Förbättrad kryptering. |
| StrongCryptographicProvider | `3` | Stark krypteringsalgoritm. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EncryptionTypeDemo
    {
        public static void EncryptionTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Ställ in krypteringsalternativ för arbetsboken
            EncryptionType encryptionType = EncryptionType.EnhancedCryptographicProviderV1;
            int keyLength = 128; // Key length can be 40, 128, or 256 bits

            // Tillämpa krypteringsinställningar
            workbook.SetEncryptionOptions(encryptionType, keyLength);

            // Skydda arbetsboken med ett lösenord
            string password = "securePassword";
            workbook.Protect(ProtectionType.All, password);

            // Spara arbetsboken
            workbook.Save("EncryptedWorkbook.xlsx");
            workbook.Save("EncryptedWorkbook.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


