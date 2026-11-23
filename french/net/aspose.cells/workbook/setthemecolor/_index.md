---
title: "Workbook.SetThemeColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Définit la couleur du thème"
type: docs
url: /fr/net/aspose.cells/workbook/setthemecolor/
---
## Workbook.SetThemeColor method

Définit la couleur du thème

```csharp
public void SetThemeColor(ThemeColorType type, Color color)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ThemeColorType | Le type de couleur du thème. |
| color | Color | la couleur du thème |

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetThemeColorWithThemeColorTypeColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir la couleur du thème pour Text1 à Vert
            workbook.SetThemeColor(ThemeColorType.Text1, Color.Green);
            
            // Appliquer la couleur du thème au style par défaut
            Style style = workbook.DefaultStyle;
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text1, 0);
            workbook.DefaultStyle = style;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Workbook with theme color saved successfully.");
        }
    }
}
```

### Voir aussi

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


