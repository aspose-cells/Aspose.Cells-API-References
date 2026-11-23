---
title: "ColorScale.MaxColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ColorScale. Obtient ou définit la couleur du dégradé pour la valeur maximale dans la plage"
type: docs
url: /fr/net/aspose.cells/colorscale/maxcolor/
---
## ColorScale.MaxColor property

Obtenir ou définir la couleur du dégradé pour la valeur maximale dans la plage.

```csharp
public Color MaxColor { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMaxColorDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Ajouter une mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Créer un objet CellArea au lieu d'utiliser une chaîne
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Ajouter une condition d'échelle de couleurs
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];
            ColorScale colorScale = fc.ColorScale;

            // Configurer l'échelle de couleurs
            colorScale.Is3ColorScale = false; // Use 2-color scale for simplicity
            colorScale.MinColor = Color.Green;
            colorScale.MaxColor = Color.Red; // Demonstrating MaxColor property

            // Définir les objets de valeur
            colorScale.MinCfvo.Type = FormatConditionValueType.Min;
            colorScale.MaxCfvo.Type = FormatConditionValueType.Max;

            // Enregistrez le classeur
            workbook.Save("ColorScaleMaxColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


