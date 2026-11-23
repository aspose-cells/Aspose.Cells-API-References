---
title: "CellsFactory.CreateStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsFactory. Crée un nouveau style"
type: docs
url: /fr/net/aspose.cells/cellsfactory/createstyle/
---
## CellsFactory.CreateStyle method

Crée un nouveau style.

```csharp
public Style CreateStyle()
```

### Valeur de retour

Renvoie un objet style.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsFactoryMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer un style en utilisant CellsFactory
            Style style = new CellsFactory().CreateStyle();
            
            // Définir les propriétés de bordure pour le style
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thick, Color.Black);
            
            // Appliquer le style à une cellule
            workbook.Worksheets[0].Cells["A1"].Value = "Hello World";
            workbook.Worksheets[0].Cells["A1"].SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [CellsFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


