---
title: "WarningInfo.CorrectedObject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WarningInfo. Obtient et définit l'objet corrigé"
type: docs
url: /fr/net/aspose.cells/warninginfo/correctedobject/
---
## WarningInfo.CorrectedObject property

Obtient et définit l'objet corrigé.

```csharp
public object CorrectedObject { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyCorrectedObjectDemo
    {
        public static void Run()
        {
            // Créez un classeur et déclenchez un avertissement
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez un nom qui déclencherait normalement un avertissement
            string originalName = "MyRange";
            worksheet.Cells.CreateRange(originalName);
            
            // Gérer le rappel d'avertissement
            workbook.Settings.WarningCallback = new WarningHandler();
            
            // Cette opération déclencherait le rappel d'avertissement
            worksheet.Cells.CreateRange(originalName); // Duplicate range name
        }
    }

    public class WarningHandler : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            if (warningInfo.WarningType == WarningType.DuplicateDefinedName)
            {
                // Démontrer l'utilisation de CorrectedObject
                warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                Console.WriteLine($"Warning handled. Original: {warningInfo.ErrorObject}, Corrected: {warningInfo.CorrectedObject}");
            }
        }
    }
}
```

### Voir aussi

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


