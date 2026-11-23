---
title: "Font.SchemeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient et définit le type de schéma de la police"
type: docs
url: /fr/net/aspose.cells/font/schemetype/
---
## Font.SchemeType property

Obtient et définit le type de schéma de la police.

```csharp
public FontSchemeType SchemeType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertySchemeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            Font font = cell.GetStyle().Font;
            font.SchemeType = FontSchemeType.Minor;
            font.Name = "Calibri";
            font.Size = 12;

            workbook.Save("FontSchemeTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FontSchemeType](../../fontschemetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


