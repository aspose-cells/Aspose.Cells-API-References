---
title: "Enum EncryptionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.EncryptionType-Enum. Verschlüsselungstyp. Wird nur von Excel2003 verwendet. Wir verschlüsseln die Arbeitsmappe 2007/2010 mit SHA AES, wie Excel es tut, und dieser EncryptionType wird ignoriert"
type: docs
url: /de/net/aspose.cells/encryptiontype/
---
## EncryptionType enumeration

Verschlüsselungstyp. Nur von Excel2003 verwendet. Wir verschlüsseln Arbeitsmappen 2007/2010 mit SHA‑AES, wie Excel es tut, und dieser Verschlüsselungstyp wird ignoriert.

```csharp
public enum EncryptionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| XOR | `0` | XOR-Verschlüsselungsalgorithmus. |
| Compatible | `1` | Kompatibel mit Office 97/2000. |
| EnhancedCryptographicProviderV1 | `2` | Erweiterte Verschlüsselung. |
| StrongCryptographicProvider | `3` | Starker Verschlüsselungsalgorithmus. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EncryptionTypeDemo
    {
        public static void EncryptionTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Verschlüsselungsoptionen für die Arbeitsmappe festlegen
            EncryptionType encryptionType = EncryptionType.EnhancedCryptographicProviderV1;
            int keyLength = 128; // Key length can be 40, 128, or 256 bits

            // Verschlüsselungseinstellungen anwenden
            workbook.SetEncryptionOptions(encryptionType, keyLength);

            // Die Arbeitsmappe mit einem Passwort schützen
            string password = "securePassword";
            workbook.Protect(ProtectionType.All, password);

            // Speichere die Arbeitsmappe
            workbook.Save("EncryptedWorkbook.xlsx");
            workbook.Save("EncryptedWorkbook.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


