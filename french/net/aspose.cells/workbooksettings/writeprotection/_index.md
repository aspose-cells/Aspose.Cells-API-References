---
title: "WorkbookSettings.WriteProtection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Fournit l'accès aux options de protection en écriture du classeur"
type: docs
url: /fr/net/aspose.cells/workbooksettings/writeprotection/
---
## WorkbookSettings.WriteProtection property

Fournit l'accès aux options de protection en écriture du classeur.

```csharp
public WriteProtection WriteProtection { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWriteProtectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Définir les propriétés de protection en écriture
            workbook.Settings.WriteProtection.Password = "test123";
            workbook.Settings.WriteProtection.Author = "John Doe";
            workbook.Settings.WriteProtection.RecommendReadOnly = true;

            // Enregistrez le classeur
            string outputPath = "WriteProtectionDemo.xlsx";
            workbook.Save(outputPath);

            // Chargez le classeur enregistré pour vérifier les propriétés
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Afficher les propriétés de protection en écriture
            Console.WriteLine("Author: " + loadedWorkbook.Settings.WriteProtection.Author);
            Console.WriteLine("ReadOnly Recommended: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
        }
    }
}
```

### Voir aussi

* class [WriteProtection](../../writeprotection/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


