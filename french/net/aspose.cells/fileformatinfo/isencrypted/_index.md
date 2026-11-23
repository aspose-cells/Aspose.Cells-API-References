---
title: "FileFormatInfo.IsEncrypted"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FileFormatInfo. Retourne vrai si le document est chiffré et nécessite un mot de passe pour l'ouvrir"
type: docs
url: /fr/net/aspose.cells/fileformatinfo/isencrypted/
---
## FileFormatInfo.IsEncrypted property

Renvoie true si le document est chiffré et nécessite un mot de passe pour l'ouvrir.

```csharp
public bool IsEncrypted { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // Détecter le format de fichier d'un fichier non chiffré
            FileFormatInfo fileInfo = FileFormatUtil.DetectFileFormat("example.xlsx");
            Console.WriteLine("Is file encrypted? " + fileInfo.IsEncrypted);

            // Détecter le format de fichier d'un fichier chiffré
            FileFormatInfo encryptedFileInfo = FileFormatUtil.DetectFileFormat("encrypted.xlsx");
            Console.WriteLine("Is encrypted file encrypted? " + encryptedFileInfo.IsEncrypted);

            // Charger le fichier chiffré avec le mot de passe
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.Password = "password";
            Workbook workbook = new Workbook("encrypted.xlsx", loadOptions);
            Console.WriteLine("Encrypted file loaded successfully");
        }
    }
}
```

### Voir aussi

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


