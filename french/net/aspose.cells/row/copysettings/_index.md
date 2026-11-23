---
title: "Row.CopySettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Row. Copie les paramètres de la ligne tels que le style, la hauteur, la visibilité ...etc."
type: docs
url: /fr/net/aspose.cells/row/copysettings/
---
## Row.CopySettings method

Copie les paramètres de la ligne, tels que le style, la hauteur, la visibilité, ...etc.

```csharp
public void CopySettings(Row source, bool checkStyle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Row | la ligne source dont les paramètres seront copiés vers celle-ci |
| checkStyle | Boolean | indique s'il faut vérifier et rassembler le style. Ne prend effet et n'est nécessaire que lorsque deux objets ligne appartiennent à des classeurs différents et que les styles des deux classeurs sont différents. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodCopySettingsWithRowBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez et stylisez la ligne source
            Row sourceRow = worksheet.Cells.Rows[0];
            Style sourceStyle = workbook.CreateStyle();
            sourceStyle.BackgroundColor = Color.Blue;
            sourceRow.ApplyStyle(sourceStyle, new StyleFlag { All = true });
            sourceRow.Height = 25;
            sourceRow.IsHidden = false;

            // Créez la ligne cible
            Row targetRow = worksheet.Cells.Rows[1];
            
            // Démontrez CopySettings avec copyStyle=true
            targetRow.CopySettings(sourceRow, true);

            // Vérifiez que les paramètres ont été copiés
            Console.WriteLine($"Target row height: {targetRow.Height}");
            Console.WriteLine($"Target row is hidden: {targetRow.IsHidden}");

            workbook.Save("RowCopySettingsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


