---
title: "WarningInfo.WarningType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WarningInfo. Obtient le type d'avertissement"
type: docs
url: /fr/net/aspose.cells/warninginfo/warningtype/
---
## WarningInfo.WarningType property

Obtenez le type d'avertissement.

```csharp
[Obsolete("Use WarningInfo.Type property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public WarningType WarningType { get; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété WarningInfo.Type. Cette propriété sera supprimée 12 mois après décembre 2024. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyWarningTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur et déclenchez un avertissement
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Cela déclenchera un avertissement lors de l'enregistrement avec des fonctionnalités non prises en charge
            workbook.Settings.WarningCallback = new WarningCallback();
            
            // Enregistrez avec un format qui pourrait provoquer des avertissements
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    internal class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Démontrez l'utilisation de la propriété WarningType
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
            
            // Gérez des types d'avertissement spécifiques
            if (warningInfo.WarningType == WarningType.UnsupportedFileFormat)
            {
                Console.WriteLine("Unsupported format warning detected!");
            }
        }
    }
}
```

### Voir aussi

* enum [WarningType](../../warningtype/)
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


