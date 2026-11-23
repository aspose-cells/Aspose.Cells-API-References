---
title: "PageSetup.IsAutoFirstPageNumber"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Indique si le premier numéro de page est attribué automatiquement"
type: docs
url: /fr/net/aspose.cells/pagesetup/isautofirstpagenumber/
---
## PageSetup.IsAutoFirstPageNumber property

Indique si le numéro de première page est attribué automatiquement.

```csharp
public bool IsAutoFirstPageNumber { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsAutoFirstPageNumberDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir les propriétés de mise en page
            worksheet.PageSetup.IsAutoFirstPageNumber = true;
            Console.WriteLine("Auto First Page Number (Worksheet 1): " + worksheet.PageSetup.IsAutoFirstPageNumber);

            // Ajouter une deuxième feuille de calcul
            worksheet = workbook.Worksheets.Add("Sheet2");
            worksheet.PageSetup.IsAutoFirstPageNumber = false;
            worksheet.PageSetup.FirstPageNumber = 3;
            Console.WriteLine("Auto First Page Number (Worksheet 2): " + worksheet.PageSetup.IsAutoFirstPageNumber);
            Console.WriteLine("First Page Number (Worksheet 2): " + worksheet.PageSetup.FirstPageNumber);

            // Enregistrez le classeur
            workbook.Save("PageSetup_IsAutoFirstPageNumber_Example.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


