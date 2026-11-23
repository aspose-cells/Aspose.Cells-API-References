---
title: "Énumération TargetModeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.TargetModeType. Représente le type de mode cible"
type: docs
url: /fr/net/aspose.cells/targetmodetype/
---
## TargetModeType enumeration

Représente le type de mode cible.

```csharp
public enum TargetModeType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| External | `0` | Lien externe |
| FilePath | `1` | Chemins locaux et complets vers des fichiers ou dossiers. |
| Email | `2` | Courriel. |
| CellReference | `3` | Lien sur une cellule ou une plage nommée. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTargetModeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un hyperlien externe
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Obtenir l'hyperlien et vérifier son TargetModeType
            Hyperlink link = worksheet.Hyperlinks[0];
            Console.WriteLine("Hyperlink TargetModeType: " + link.LinkType);
            
            // Supprimer l'hyperlien
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


