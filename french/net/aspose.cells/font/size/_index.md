---
title: "Font.Size"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient ou définit la taille de la police"
type: docs
url: /fr/net/aspose.cells/font/size/
---
## Font.Size property

Obtient ou définit la taille de la police.

```csharp
public int Size { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir du texte avec différentes tailles de police
            Cell cell1 = worksheet.Cells["A1"];
            cell1.Value = "Text with size 12";
            Style style1 = workbook.CreateStyle();
            style1.Font.Size = 12;
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A3"];
            cell2.Value = "Text with size 16";
            Style style2 = workbook.CreateStyle();
            style2.Font.Size = 16;
            cell2.SetStyle(style2);

            // Enregistrez le classeur
            workbook.Save("FontSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


