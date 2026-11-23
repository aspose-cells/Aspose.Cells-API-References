---
title: "ExternalLink.PathType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalLink. Obtient le type de chemin de ce lien externe"
type: docs
url: /fr/net/aspose.cells/externallink/pathtype/
---
## ExternalLink.PathType property

Obtenez le type de chemin de ce lien externe

```csharp
public string PathType { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyPathTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Créer un lien externe vers un autre classeur
            sheet.Cells["A1"].Formula = "='C:\\Temp\\ExternalWorkbook.xlsx'!Sheet1!A1";
            
            // Obtenir le lien externe
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Afficher le type de chemin du lien externe
            Console.WriteLine("Path Type: " + externalLink.PathType);
            
            // Enregistrez le classeur
            workbook.Save("ExternalLinkDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


