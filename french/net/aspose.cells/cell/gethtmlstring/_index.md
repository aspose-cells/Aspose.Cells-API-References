---
title: "Cell.GetHtmlString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtient la chaîne HTML qui contient les données et certains formats dans cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/gethtmlstring/
---
## Cell.GetHtmlString method

Obtient la chaîne html qui contient des données et certains formats dans cette cellule.

```csharp
public string GetHtmlString(bool html5)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| html5 | Boolean | Indique si la valeur est compatible avec html5 |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHtmlStringWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir une valeur d'exemple pour la cellule avec mise en forme
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            style.Font.Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            // Démontrer GetHtmlString avec un paramètre booléen
            string htmlWithoutDiv = cell.GetHtmlString(false);
            string htmlWithDiv = cell.GetHtmlString(true);
            
            Console.WriteLine("HTML without div wrapper:");
            Console.WriteLine(htmlWithoutDiv);
            Console.WriteLine("\nHTML with div wrapper:");
            Console.WriteLine(htmlWithDiv);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


