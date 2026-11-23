---
title: "FileFormatUtil.VerifyPassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FileFormatUtil. Détecte et retourne les informations sur le format d'un fichier Excel stocké dans un stream"
type: docs
url: /fr/net/aspose.cells/fileformatutil/verifypassword/
---
## FileFormatUtil.VerifyPassword method

Détecte et renvoie les informations sur le format d'un Excel stocké dans un flux.

```csharp
public static bool VerifyPassword(Stream stream, string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream |  |
| mot de passe | String | Le mot de passe pour les fichiers ooxml chiffrés. |

### Valeur de retour

Renvoie si le mot de passe est correct.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodVerifyPasswordWithStreamStringDemo
    {
        public static void Run()
        {
            string filePath = "example.xlsx";
            string correctPassword = "test";
            string wrongPassword = "1234";

            using (Stream stream = File.OpenRead(filePath))
            {
                bool isValid = FileFormatUtil.VerifyPassword(stream, correctPassword);
                Console.WriteLine($"Password '{correctPassword}' is valid: {isValid}");
            }

            using (Stream stream = File.OpenRead(filePath))
            {
                bool isValid = FileFormatUtil.VerifyPassword(stream, wrongPassword);
                Console.WriteLine($"Password '{wrongPassword}' is valid: {isValid}");
            }
        }
    }
}
```

### Voir aussi

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


