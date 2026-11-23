---
title: "Classe AbstractLowCodeProtectionProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.AbstractLowCodeProtectionProvider. Implémentation pour fournir les paramètres de protection"
type: docs
url: /fr/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/
---
## AbstractLowCodeProtectionProvider class

Implémentation pour fournir les paramètres de protection.

```csharp
public class AbstractLowCodeProtectionProvider
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [AbstractLowCodeProtectionProvider](abstractlowcodeprotectionprovider/)() | Le constructeur par défaut. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [GetOpenPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/)() | Obtient le mot de passe pour ouvrir le fichier de feuille de calcul. |
| virtual [GetWorkbookPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookpassword/)() | Obtient le mot de passe pour protéger le classeur avec le type de protection spécifié. |
| virtual [GetWorkbookProtectionType](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookprotectiontype/)() | Obtient le type de protection pour protéger le classeur. |
| virtual [GetWorksheetPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/)(string) | Obtient le mot de passe pour protéger la feuille de calcul spécifiée. |
| virtual [GetWorksheetProtectionType](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetprotectiontype/)(string) | Obtient le type de protection pour protéger la feuille de calcul spécifiée. |
| virtual [GetWritePassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/)() | Obtient le mot de passe pour modifier le fichier de feuille de calcul. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeProtectionProviderDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et ajoutez des feuilles de calcul de test
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("AuditReport");

            // Créez une instance de fournisseur de protection personnalisé
            var protectionProvider = new CustomProtectionProvider();

            // Appliquez la protection du classeur
            workbook.Protect(
                protectionProvider.GetWorkbookProtectionType(),
                protectionProvider.GetWorkbookPassword()
            );

            // Appliquez la protection à toutes les feuilles de calcul
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                worksheet.Protect(
                    protectionProvider.GetWorksheetProtectionType(worksheet.Name),
                    null,  // Add null for oldPassword parameter
                    protectionProvider.GetWorksheetPassword(worksheet.Name)
                );
            }

            // Définissez les mots de passe d'accès au fichier
            workbook.Settings.Password = protectionProvider.GetOpenPassword();
            workbook.Settings.WriteProtection.Password = protectionProvider.GetWritePassword();

            // Enregistrez le classeur protégé
            workbook.Save("AbstractLowCodeProtectionProviderDemo.xlsx");
        }
    }

    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetOpenPassword() => "SecureOpen123";
        public override string GetWritePassword() => "EditPermission456";
        public override string GetWorkbookPassword() => "WorkbookLock789";
        
        public override ProtectionType GetWorkbookProtectionType() => 
            ProtectionType.Windows;  // Prevent window structure changes

        public override string GetWorksheetPassword(string sheetName) => 
            $"SheetLock_{sheetName}";  // Dynamic password per sheet

        public override ProtectionType GetWorksheetProtectionType(string sheetName) => 
            ProtectionType.Contents;  // Protect cell contents
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


