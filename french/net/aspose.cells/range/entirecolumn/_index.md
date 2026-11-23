---
title: "Range.EntireColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient un objet Range qui représente la colonne entière ou les colonnes contenant la plage spécifiée"
type: docs
url: /fr/net/aspose.cells/range/entirecolumn/
---
## Range.EntireColumn property

Obtient un objet Range qui représente la colonne entière (ou les colonnes) contenant la plage spécifiée.

```csharp
public Range EntireColumn { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez une plage commençant à la cellule C1 (ligne 0, colonne 2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, 1, 1);
            
            // Obtenez la colonne entière contenant la plage (colonne C)
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            
            // Appliquez le formatage à la colonne entière
            Style style = entireColumn[0, 0].GetStyle();
            style.Custom = "##0%";
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            entireColumn.ApplyStyle(style, styleFlag);
            
            // Enregistrez le classeur
            workbook.Save("EntireColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


