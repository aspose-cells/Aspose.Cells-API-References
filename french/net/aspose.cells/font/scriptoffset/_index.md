---
title: "Font.ScriptOffset"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient et définit le décalage de script en pourcentage"
type: docs
url: /fr/net/aspose.cells/font/scriptoffset/
---
## Font.ScriptOffset property

Obtient et définit le décalage de script, en unité de pourcentage

```csharp
public double ScriptOffset { get; set; }
```

### Remarques

Uniquement pour les formes et les graphiques.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyScriptOffsetDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à la cellule A1 et définissez sa valeur
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("ScriptOffset Demo");

            // Obtenir le style et la police de la cellule
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Définir ScriptOffset pour démontrer l'effet indice/exposant
            font.ScriptOffset = 10; // Positive for superscript, negative for subscript
            font.IsSuperscript = true; // Enable superscript

            // Appliquer le style modifié à la cellule
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("FontScriptOffsetDemo.xlsx");

            // Vérifier la valeur de ScriptOffset
            Console.WriteLine("ScriptOffset value: " + font.ScriptOffset);
        }
    }
}
```

### Voir aussi

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


