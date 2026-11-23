---
title: "Font.IsBold"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient ou définit une valeur indiquant si la police est en gras"
type: docs
url: /fr/net/aspose.cells/font/isbold/
---
## Font.IsBold property

Obtient ou définit une valeur indiquant si la police est en gras.

```csharp
public bool IsBold { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsBoldDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à la cellule A1 et définissez sa valeur
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Bold Text Demo");
            
            // Obtenez le style de la cellule et définissez la police en gras
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("FontIsBoldDemo.xlsx");
            
            // Vérifiez la propriété en gras
            Workbook loadedWorkbook = new Workbook("FontIsBoldDemo.xlsx");
            Style loadedStyle = loadedWorkbook.Worksheets[0].Cells["A1"].GetStyle();
            Console.WriteLine("IsBold property: " + loadedStyle.Font.IsBold);
        }
    }
}
```

### Voir aussi

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


