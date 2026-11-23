---
title: "ColorHelper.FromOleColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ColorHelper. Convertit OLE_COLOR"
type: docs
url: /fr/net/aspose.cells.drawing/colorhelper/fromolecolor/
---
## ColorHelper.FromOleColor method

Convertir OLE_COLOR.

```csharp
public static Color FromOleColor(int oleColor)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| oleColor | Int32 | La valeur de OLE_COLOR. |

### Valeur de retour

L'objet Color.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ColorHelperMethodFromOleColorWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int oleColor = 0x00FF0000; // OLE color for blue in BGR format
            
            try
            {
                Color convertedColor = ColorHelper.FromOleColor(oleColor);
                
                // Appliquez la couleur à l'arrière-plan de la cellule
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("Color converted from OLE");
                Style style = cell.GetStyle();
                style.ForegroundColor = convertedColor;
                style.Pattern = BackgroundType.Solid;
                cell.SetStyle(style);
                
                Console.WriteLine($"Converted OLE color {oleColor:X} to RGB: {convertedColor.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            
            workbook.Save("ColorHelperMethodFromOleColorWithInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ColorHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


