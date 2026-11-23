---
title: "WorkbookSettings.Password"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Représente le mot de passe de chiffrement du fichier du classeur"
type: docs
url: /fr/net/aspose.cells/workbooksettings/password/
---
## WorkbookSettings.Password property

Représente le mot de passe de chiffrement du fichier du classeur.

```csharp
public string Password { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Accédez à la première feuille de calcul et ajoutez des données
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["C6"].PutValue("test encrypt.");
            
            // Définir le mot de passe pour protéger le classeur
            wb.Settings.Password = "xixi";
            
            // Enregistrez le classeur
            wb.Save("output_with_password.ods");
            
            // Créer des options de chargement avec le mot de passe pour ouvrir le classeur protégé
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "xixi";
            
            // Ouvrir le classeur protégé par mot de passe
            Workbook wbProtected = new Workbook("output_with_password.ods", loadOptions);
            
            // Vérifier les données
            Console.WriteLine("Cell value: " + wbProtected.Worksheets[0].Cells["C6"].Value);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


