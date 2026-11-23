---
title: "Font.Underline"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient ou définit le type de soulignement de la police"
type: docs
url: /fr/net/aspose.cells/font/underline/
---
## Font.Underline property

Obtient ou définit le type de soulignement de la police.

```csharp
public FontUnderlineType Underline { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyUnderlineDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Accédez à la cellule et définissez le style de soulignement
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Underlined Text");
            
            // Obtenez le style et modifiez les propriétés de la police
            Style style = cell.GetStyle();
            style.Font.Underline = FontUnderlineType.Single;
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FontUnderlineType](../../fontunderlinetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


