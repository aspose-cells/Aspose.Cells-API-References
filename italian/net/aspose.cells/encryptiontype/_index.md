---
title: "Enum EncryptionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.EncryptionType. Tipo di crittografia. Utilizzato solo da excel2003. Cripteremo la cartella di lavoro 2007/2010 usando SHA AES come fa Excel e questo EncryptionType verrà ignorato."
type: docs
url: /it/net/aspose.cells/encryptiontype/
---
## EncryptionType enumeration

Tipo di crittografia. Utilizzato solo da excel2003. Cripteremo la cartella di lavoro 2007/2010 usando SHA AES come fa Excel, e questo EncryptionType verrà ignorato.

```csharp
public enum EncryptionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| XOR | `0` | Algoritmo di crittografia XOR. |
| Compatible | `1` | Compatibile con Office 97/2000. |
| EnhancedCryptographicProviderV1 | `2` | Crittografia avanzata. |
| StrongCryptographicProvider | `3` | Algoritmo di crittografia forte. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EncryptionTypeDemo
    {
        public static void EncryptionTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta le opzioni di crittografia per la cartella di lavoro
            EncryptionType encryptionType = EncryptionType.EnhancedCryptographicProviderV1;
            int keyLength = 128; // Key length can be 40, 128, or 256 bits

            // Applica le impostazioni di crittografia
            workbook.SetEncryptionOptions(encryptionType, keyLength);

            // Proteggi la cartella di lavoro con una password
            string password = "securePassword";
            workbook.Protect(ProtectionType.All, password);

            // Salva la cartella di lavoro
            workbook.Save("EncryptedWorkbook.xlsx");
            workbook.Save("EncryptedWorkbook.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


