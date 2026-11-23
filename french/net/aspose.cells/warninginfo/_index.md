---
title: "Classe WarningInfo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.WarningInfo. Informations d'avertissement"
type: docs
url: /fr/net/aspose.cells/warninginfo/
---
## WarningInfo class

Informations d'avertissement

```csharp
public class WarningInfo
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CorrectedObject](../../aspose.cells/warninginfo/correctedobject/) { get; set; } | Obtient et définit l'objet corrigé. |
| [Description](../../aspose.cells/warninginfo/description/) { get; } | Obtenir la description des informations d'avertissement. |
| [ErrorObject](../../aspose.cells/warninginfo/errorobject/) { get; } | L'objet d'erreur. |
| [Type](../../aspose.cells/warninginfo/type/) { get; } | Obtenez le type d'avertissement. |
| [WarningType](../../aspose.cells/warninginfo/warningtype/) { get; } | (**Obsolète.**) Obtenez le type d'avertissement. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassWarningInfoDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définissez le rappel d'avertissement
            workbook.Settings.WarningCallback = new WarningHandler();

            // Déclenchez différents types d'avertissement
            worksheet.Cells["A1"].PutValue("InvalidName"); // Will trigger DefinedName warning
            worksheet.Cells["A2"].PutValue(DateTime.MaxValue); // May trigger other warnings

            Console.WriteLine("Warning demo completed.");
        }
    }

    public class WarningHandler : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            switch (warningInfo.WarningType)
            {
                case WarningType.DuplicateDefinedName:
                    warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                    Console.WriteLine($"DefinedName warning handled. Corrected to: {warningInfo.CorrectedObject}");
                    break;
                case WarningType.FontSubstitution:
                    Console.WriteLine($"Font warning: {warningInfo.Description}");
                    break;
                case WarningType.UnsupportedFileFormat:
                    Console.WriteLine($"File format warning: {warningInfo.Description}");
                    break;
                case WarningType.IO:
                    Console.WriteLine($"IO warning: {warningInfo.Description}");
                    break;
                case WarningType.InvalidData:
                case WarningType.Limitation:
                    Console.WriteLine($"Warning: {warningInfo.Description}");
                    break;
                default:
                    Console.WriteLine($"Unknown warning type: {warningInfo.Description}");
                    break;
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


