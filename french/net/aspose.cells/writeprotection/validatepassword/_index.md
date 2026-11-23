---
title: "WriteProtection.ValidatePassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WriteProtection. Retourne true si le mot de passe spécifié est identique au mot de passe de protection en écriture avec lequel le fichier a été protégé"
type: docs
url: /fr/net/aspose.cells/writeprotection/validatepassword/
---
## WriteProtection.ValidatePassword method

Renvoie vrai si le mot de passe spécifié est identique au mot de passe de protection en écriture avec lequel le fichier a été protégé.

```csharp
public bool ValidatePassword(string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| mot de passe | String | Le mot de passe spécifié. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir le mot de passe de protection en écriture
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Valider le mot de passe
            Console.WriteLine("Password '1234' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            Console.WriteLine("Password 'wrong' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("wrong"));
        }
    }
}
```

### Voir aussi

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


