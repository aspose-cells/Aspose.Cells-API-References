---
title: "Workbook.GetThemeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Obtient la couleur du thème"
type: docs
url: /fr/net/aspose.cells/workbook/getthemecolor/
---
## Workbook.GetThemeColor method

Obtient la couleur du thème.

```csharp
public Color GetThemeColor(ThemeColorType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ThemeColorType | Le type de couleur du thème. |

### Valeur de retour

La couleur du thème.

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetThemeColorWithThemeColorTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenir la couleur du thème pour Accent6
            Color color = workbook.GetThemeColor(ThemeColorType.Accent6);
            Console.WriteLine("Theme Color (Accent6): " + color.ToString());
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


