---
title: "InsertOptions.UpdateReference"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété InsertOptions. Indique si les références dans d’autres feuilles de calcul seront mises à jour"
type: docs
url: /fr/net/aspose.cells/insertoptions/updatereference/
---
## InsertOptions.UpdateReference property

Indique si les références dans d'autres feuilles de calcul seront mises à jour.

```csharp
public bool UpdateReference { get; set; }
```

### Remarques

À partir de la version 26.7, nous définissons la valeur par défaut de cette propriété à true.

### Exemples

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook wb = new Workbook();
            
            // Ajoutez une deuxième feuille de calcul et définissez des formules qui font référence à Sheet1
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].Formula = "=Sheet1!A10";
            sheet2.Cells["B1"].Formula = "=Sheet1!A5";
            
            // Définir des formules dans Sheet1
            Worksheet sheet1 = wb.Worksheets[0];
            sheet1.Cells["A1"].Formula = "=A10";
            sheet1.Cells["B1"].Formula = "=A5";

            // Créer des options d’insertion avec UpdateReference activé
            InsertOptions iopts = new InsertOptions();
            iopts.UpdateReference = true;
            
            // Suivre les modifications de formules
            HashSet<string> changedCells = new HashSet<string>();
            iopts.UpdateReference = true;
            
            // Insérer des lignes qui mettront à jour les références dans les formules
            sheet1.Cells.InsertRows(5, 3, iopts);
            
            // Afficher le nombre de cellules modifiées
            Console.WriteLine("Formulas were automatically updated due to UpdateReference=true");
            
            // Afficher les formules mises à jour
            Console.WriteLine("Sheet1 A1 formula: " + sheet1.Cells["A1"].Formula);
            Console.WriteLine("Sheet2 A1 formula: " + sheet2.Cells["A1"].Formula);
        }
    }
}
```

### Voir aussi

* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


