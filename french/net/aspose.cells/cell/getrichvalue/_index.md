---
title: "Cell.GetRichValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtient la valeur enrichie de la cellule"
type: docs
url: /fr/net/aspose.cells/cell/getrichvalue/
---
## Cell.GetRichValue method

Obtient la valeur enrichie de la cellule.

```csharp
public CellRichValue GetRichValue()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetRichValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet ws = wb.Worksheets[0];
            
            // Définissez une valeur de texte enrichi dans la cellule A1
            ws.Cells["A1"].PutValue("This is rich text");
            
            // Obtenir la valeur riche de la cellule A1
            CellRichValue richValue = ws.Cells["A1"].GetRichValue();
            
            // Affichez la valeur de texte enrichi
            Console.WriteLine("Rich Text Value: " + ws.Cells["A1"].StringValue);
            
            // Enregistrez le classeur
            wb.Save("RichValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellRichValue](../../cellrichvalue/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


