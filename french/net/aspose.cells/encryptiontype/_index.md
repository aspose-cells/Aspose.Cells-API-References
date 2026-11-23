---
title: "Enum EncryptionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.EncryptionType enum. Type de chiffrement. Utilisé uniquement par excel2003. Nous chiffrerons le classeur 2007/2010 en utilisant SHA AES comme le fait Excel et ce EncryptionType sera ignoré"
type: docs
url: /fr/net/aspose.cells/encryptiontype/
---
## EncryptionType enumeration

Type de chiffrement. Utilisé uniquement par excel2003. Nous chiffrerons les classeurs 2007/2010 en utilisant SHA AES de la même manière qu'Excel le fait, et ce EncryptionType sera ignoré.

```csharp
public enum EncryptionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| XOR | `0` | Algorithme de chiffrement XOR. |
| Compatible | `1` | Compatible Office 97/2000. |
| EnhancedCryptographicProviderV1 | `2` | Chiffrement amélioré. |
| StrongCryptographicProvider | `3` | Algorithme de chiffrement fort. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EncryptionTypeDemo
    {
        public static void EncryptionTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Définir les options de chiffrement pour le classeur
            EncryptionType encryptionType = EncryptionType.EnhancedCryptographicProviderV1;
            int keyLength = 128; // Key length can be 40, 128, or 256 bits

            // Appliquer les paramètres de chiffrement
            workbook.SetEncryptionOptions(encryptionType, keyLength);

            // Protéger le classeur avec un mot de passe
            string password = "securePassword";
            workbook.Protect(ProtectionType.All, password);

            // Enregistrez le classeur
            workbook.Save("EncryptedWorkbook.xlsx");
            workbook.Save("EncryptedWorkbook.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


