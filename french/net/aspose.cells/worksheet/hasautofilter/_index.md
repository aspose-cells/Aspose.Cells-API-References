---
title: "Worksheet.HasAutofilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Indique si cette feuille de calcul possède un filtre automatique"
type: docs
url: /fr/net/aspose.cells/worksheet/hasautofilter/
---
## Worksheet.HasAutofilter property

Indique si cette feuille de calcul possède un filtre automatique.

```csharp
public bool HasAutofilter { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHasAutofilterDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Définissez le filtre automatique
            worksheet.AutoFilter.Range = "A1:B3";
            
            // Vérifiez si la feuille de calcul possède un filtre automatique
            Console.WriteLine("Worksheet has autofilter: " + worksheet.HasAutofilter);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


