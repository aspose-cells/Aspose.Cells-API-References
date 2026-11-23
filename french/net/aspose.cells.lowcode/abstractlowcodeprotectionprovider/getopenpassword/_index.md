---
title: "AbstractLowCodeProtectionProvider.GetOpenPassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractLowCodeProtectionProvider. Obtient le mot de passe pour ouvrir le fichier de feuille de calcul"
type: docs
url: /fr/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/
---
## AbstractLowCodeProtectionProvider.GetOpenPassword method

Obtient le mot de passe pour ouvrir le fichier de feuille de calcul.

```csharp
public virtual string GetOpenPassword()
```

### Valeur de retour

Mot de passe pour ouvrir le fichier de feuille de calcul. Vide signifie aucune protection pour l'ouverture du fichier.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetOpenPasswordDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une instance de fournisseur de protection
                var protectionProvider = new DemoProtectionProvider();

                // Appeler la méthode GetOpenPassword pour récupérer le mot de passe
                string password = protectionProvider.GetOpenPassword();

                // Créer un nouveau classeur et appliquer le mot de passe
                Workbook workbook = new Workbook("sample.xlsx");
                workbook.Settings.Password = password;

                // Enregistrer le classeur protégé par mot de passe
                workbook.Save("MethodGetOpenPasswordDemo.xlsx");

                Console.WriteLine($"Workbook protected with open password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }
    }

    public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetOpenPassword()
        {
            return "AsposeDemo123!";
        }
    }
}
```

### Voir aussi

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


