---
title: "AbstractLowCodeProtectionProvider.GetWritePassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractLowCodeProtectionProvider. Obtient le mot de passe pour modifier le fichier de feuille de calcul"
type: docs
url: /fr/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/
---
## AbstractLowCodeProtectionProvider.GetWritePassword method

Obtient le mot de passe pour modifier le fichier de feuille de calcul.

```csharp
public virtual string GetWritePassword()
```

### Valeur de retour

Mot de passe pour modifier le fichier de feuille de calcul. Vide signifie aucune protection pour la modification du fichier.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWritePasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Créez une instance de fournisseur de protection personnalisé
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                // Appeler explicitement GetWritePassword et afficher le résultat
                string writePassword = protectionProvider.GetWritePassword();
                Console.WriteLine($"Retrieved write password: {writePassword}");

                // Enregistrer le classeur - appliquer directement la protection en écriture
                workbook.Settings.WriteProtection.Password = writePassword;
                workbook.Save("MethodGetWritePasswordDemo.xlsx");
                Console.WriteLine("Workbook saved with write protection password.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWritePassword method: {ex.Message}");
            }
        }

    }

    // Implémentation personnalisée du fournisseur de protection
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetWritePassword()
        {
            return "AsposeTestPassword123!";
        }

        // Implémenter les autres méthodes requises avec des valeurs de retour par défaut
        public override string GetOpenPassword() => null;
        public override string GetWorkbookPassword() => null;
        public override ProtectionType GetWorkbookProtectionType() => ProtectionType.None;
        public override string GetWorksheetPassword(string sheetName) => null;
        public override ProtectionType GetWorksheetProtectionType(string sheetName) => ProtectionType.None;
    }
}
```

### Voir aussi

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


