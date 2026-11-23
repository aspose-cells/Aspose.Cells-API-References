---
title: "WorkbookSettings.IsProtected"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient une valeur qui indique si la structure ou la fenêtre du classeur est protégée"
type: docs
url: /fr/net/aspose.cells/workbooksettings/isprotected/
---
## WorkbookSettings.IsProtected property

Obtient une valeur indiquant si la structure ou la fenêtre du Workbook est protégée.

```csharp
public bool IsProtected { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;
            
            // Vérifier si le classeur est protégé
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Protéger le classeur avec un mot de passe
            settings.Password = "password123";
            
            // Vérifiez l'état de protection
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Enregistrez le classeur protégé
            workbook.Save("ProtectedWorkbook.xlsx", SaveFormat.Xlsx);
            
            // Ouvrir le classeur protégé
            Workbook protectedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            
            // Vérifier l'état de protection du classeur chargé
            Console.WriteLine("Loaded workbook is protected: " + protectedWorkbook.Settings.IsProtected);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


