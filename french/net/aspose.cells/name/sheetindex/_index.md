---
title: "Name.SheetIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Name. Indique que ce nom appartient à Workbook ou Worksheet. 0  Nom global sinon indice de la feuille basé sur 1"
type: docs
url: /fr/net/aspose.cells/name/sheetindex/
---
## Name.SheetIndex property

Indique que ce nom appartient à un classeur ou à une feuille de calcul. 0 = nom global, sinon indice de la feuille (à partir de 1).

```csharp
public int SheetIndex { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertySheetIndexDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter plusieurs feuilles de calcul
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Créer une plage nommée dans Sheet2
            Worksheet sheet2 = workbook.Worksheets["Sheet2"];
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet2!$A$1:$B$10";
            
            // Afficher l'indice de la feuille de la plage nommée
            Console.WriteLine("Sheet index of named range: " + name.SheetIndex);
            
            // Enregistrez le classeur
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


