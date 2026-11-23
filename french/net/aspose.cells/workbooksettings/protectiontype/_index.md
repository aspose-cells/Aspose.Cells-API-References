---
title: "WorkbookSettings.ProtectionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient le type de protection du classeur"
type: docs
url: /fr/net/aspose.cells/workbooksettings/protectiontype/
---
## WorkbookSettings.ProtectionType property

Obtient le type de protection du classeur.

```csharp
public ProtectionType ProtectionType { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyProtectionTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Protéger le classeur avec le type de protection Windows
            workbook.Protect(ProtectionType.Windows, "password123");
            
            // Démontrer la propriété ProtectionType
            Console.WriteLine("Workbook protection type: " + workbook.Settings.ProtectionType);
            
            // Enregistrez le classeur
            workbook.Save("ProtectedWorkbook.xlsx");
            
            // Charger le classeur enregistré pour vérifier que le type de protection persiste
            Workbook loadedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            Console.WriteLine("Loaded workbook protection type: " + loadedWorkbook.Settings.ProtectionType);
        }
    }
}
```

### Voir aussi

* enum [ProtectionType](../../protectiontype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


