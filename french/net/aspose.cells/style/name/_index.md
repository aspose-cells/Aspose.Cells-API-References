---
title: "Style.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient ou définit le nom du style"
type: docs
url: /fr/net/aspose.cells/style/name/
---
## Style.Name property

Obtient ou définit le nom du style.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer et appliquer le premier style nommé
            Style style1 = workbook.CreateStyle();
            style1.Number = 7;
            style1.Name = "Sales";
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Sales Data");
            
            // Créer et appliquer le deuxième style nommé
            Style style2 = workbook.CreateStyle();
            style2.Font.Size = 14;
            style2.Font.IsBold = true;
            style2.Font.IsItalic = true;
            style2.Font.Color = System.Drawing.Color.Yellow;
            style2.ForegroundColor = System.Drawing.Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            style2.Name = "Header";
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Header Text");
            
            // Enregistrez le classeur
            workbook.Save("StylePropertyNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


