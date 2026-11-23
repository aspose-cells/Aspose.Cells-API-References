---
title: "Protection.GetPasswordHash"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Protection. Obtient le hachage du mot de passe actuel"
type: docs
url: /fr/net/aspose.cells/protection/getpasswordhash/
---
## Protection.GetPasswordHash method

Obtient le hachage du mot de passe actuel.

```csharp
public int GetPasswordHash()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodGetPasswordHashDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir les paramètres de protection avec un mot de passe
            Protection protection = worksheet.Protection;
            protection.Password = "password123";
            protection.AllowDeletingColumn = true;
            protection.AllowFormattingCell = true;
            
            // Protéger la feuille de calcul
            worksheet.Protect(ProtectionType.All);

            try
            {
                // Obtenir le hachage du mot de passe
                int passwordHash = protection.GetPasswordHash();
                
                // Afficher le résultat
                Console.WriteLine($"Password hash: {passwordHash}");
                Console.WriteLine($"Is protected with password: {protection.IsProtectedWithPassword}");

                // Vérifier le mot de passe (démonstration de la fonctionnalité associée)
                bool isVerified = protection.VerifyPassword("password123");
                Console.WriteLine($"Password verification result: {isVerified}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPasswordHash method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("ProtectionMethodGetPasswordHashDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


