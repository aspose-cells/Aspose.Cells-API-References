---
title: "Cell.HasCustomFunction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Vérifie s'il y a une fonction personnalisée non prise en charge dans la formule de cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/hascustomfunction/
---
## Cell.HasCustomFunction property

Vérifie s'il existe une fonction personnalisée (fonction non prise en charge) dans la formule de cette cellule.

```csharp
public bool HasCustomFunction { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook wb = new Workbook();
            
            // Ajouter un nom de fonction personnalisée
            NameCollection nc = wb.Worksheets.Names;
            nc[nc.Add("MyCustomFunc")].RefersTo = "=MYTESTFUNC()";
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Tester avec une fonction intégrée
            Cell cell1 = cells[0, 0];
            cell1.Formula = "=SUM(A1:B1)";
            Console.WriteLine("HasCustomFunction (SUM): " + cell1.HasCustomFunction);
            
            // Tester avec une fonction personnalisée
            Cell cell2 = cells[1, 0];
            cell2.Formula = "=MYTESTFUNC()";
            Console.WriteLine("HasCustomFunction (MYTESTFUNC): " + cell2.HasCustomFunction);
            
            // Tester avec une plage nommée contenant une fonction personnalisée
            Cell cell3 = cells[2, 0];
            cell3.Formula = "=MyCustomFunc";
            Console.WriteLine("HasCustomFunction (Named Range): " + cell3.HasCustomFunction);
            
            // Tester avec une fonction personnalisée imbriquée
            Cell cell4 = cells[3, 0];
            cell4.Formula = "=SUM(MYTESTFUNC(), A1)";
            Console.WriteLine("HasCustomFunction (Nested): " + cell4.HasCustomFunction);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


