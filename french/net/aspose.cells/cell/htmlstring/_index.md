---
title: "Cell.HtmlString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient et définit la chaîne html qui contient des données et certains formats dans cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/htmlstring/
---
## Cell.HtmlString property

Obtient et définit la chaîne HTML qui contient des données et certains formats dans cette cellule.

```csharp
public string HtmlString { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHtmlStringDemo
    {
        public static void Run()
        {
            // Créer une instance de classe Workbook
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la collection de cellules
            Cells cells = worksheet.Cells;
            
            // Définir la chaîne HTML avec formatage dans la cellule A1
            cells["A1"].HtmlString = "This is <b>bold</b> and <i>italic</i> text<br>with a line break";
            
            // Enregistrez le classeur
            workbook.Save("HtmlStringDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


