---
title: "Cell.R1C1Formula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient ou définit une formule R1C1 de la Cell"
type: docs
url: /fr/net/aspose.cells/cell/r1c1formula/
---
## Cell.R1C1Formula property

Obtient ou définit une formule R1C1 de la [`Cell`](../).

```csharp
public string R1C1Formula { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyR1C1FormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la valeur A1
            worksheet.Cells["A1"].PutValue(10);
            
            // Définir la valeur B1
            worksheet.Cells["B1"].PutValue(20);
            
            // Définir la formule C1 en notation A1
            worksheet.Cells["C1"].Formula = "=A1+B1";
            
            // Obtenir et afficher la formule R1C1
            string r1c1Formula = worksheet.Cells["C1"].R1C1Formula;
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
            
            // Définir la formule D1 en notation R1C1
            worksheet.Cells["D1"].R1C1Formula = "=RC[-3]+RC[-2]";
            
            // Obtenir et afficher la formule A1
            string a1Formula = worksheet.Cells["D1"].Formula;
            Console.WriteLine("A1 Formula: " + a1Formula);
            
            // Enregistrez le classeur
            workbook.Save("R1C1FormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


