---
title: "DefaultStyleSettings.HorizontalAlignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DefaultStyleSettings. Obtient/Définit la valeur par défaut pour l'alignement horizontal"
type: docs
url: /fr/net/aspose.cells/defaultstylesettings/horizontalalignment/
---
## DefaultStyleSettings.HorizontalAlignment property

Obtient/Définit la valeur par défaut pour l'alignement horizontal

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Définir l'alignement horizontal pour démontrer la propriété
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;

            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Centered Text";
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


