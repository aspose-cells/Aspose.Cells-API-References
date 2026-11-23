---
title: "Worksheet.AddPageBreaks"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Ajoute un saut de page"
type: docs
url: /fr/net/aspose.cells/worksheet/addpagebreaks/
---
## Worksheet.AddPageBreaks method

Ajoute un saut de page.

```csharp
public void AddPageBreaks(string cellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String |  |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAddPageBreaksWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un saut de page horizontal à la ligne 1 (B2)
            worksheet.AddPageBreaks("B2");

            // Ajouter un saut de page horizontal à la ligne 9 (B10)
            worksheet.AddPageBreaks("B10");

            // Vérifier que le premier saut de page a été ajouté à la ligne 1
            Console.WriteLine("First page break row: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


