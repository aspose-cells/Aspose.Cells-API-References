---
title: "Protection.VerifyPassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Protection. Vérifie le mot de passe"
type: docs
url: /fr/net/aspose.cells/protection/verifypassword/
---
## Protection.VerifyPassword method

Vérifie le mot de passe.

```csharp
public bool VerifyPassword(string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| mot de passe | String | Le mot de passe. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodVerifyPasswordWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Protéger la feuille de calcul avec un mot de passe
            worksheet.Protection.AllowDeletingColumn = false;
            worksheet.Protection.AllowDeletingRow = false;
            worksheet.Protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            try
            {
                // Vérifier le mot de passe
                bool isPasswordCorrect = worksheet.Protection.VerifyPassword("password123");
                
                Console.WriteLine($"Password verification result: {isPasswordCorrect}");
                
                if (isPasswordCorrect)
                {
                    Console.WriteLine("The provided password matches the worksheet protection password.");
                }
                else
                {
                    Console.WriteLine("The provided password does not match the worksheet protection password.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing VerifyPassword method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("ProtectionMethodVerifyPasswordWithStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


