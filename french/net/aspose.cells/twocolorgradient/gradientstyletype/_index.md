---
title: "TwoColorGradient.GradientStyleType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TwoColorGradient. Obtient et définit le style d’ombrage du dégradé"
type: docs
url: /fr/net/aspose.cells/twocolorgradient/gradientstyletype/
---
## TwoColorGradient.GradientStyleType property

Obtient et définit le style d'ombrage du dégradé.

```csharp
public GradientStyleType GradientStyleType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class TwoColorGradientPropertyGradientStyleTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            TwoColorGradient gradient = new TwoColorGradient(Color.CornflowerBlue, Color.LightCoral, GradientStyleType.FromCenter, 1);
            Console.WriteLine("Initial GradientStyleType: " + gradient.GradientStyleType);

            Style cellStyle = worksheet.Cells["B2"].GetStyle();
            cellStyle.Pattern = BackgroundType.Solid;
            cellStyle.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["B2"].SetStyle(cellStyle);
            worksheet.Cells["B2"].PutValue("Initial Gradient (From Center)");

            gradient.GradientStyleType = GradientStyleType.DiagonalUp;
            Console.WriteLine("Modified GradientStyleType: " + gradient.GradientStyleType);

            Style modifiedStyle = worksheet.Cells["F6"].GetStyle();
            modifiedStyle.Pattern = BackgroundType.Solid;
            modifiedStyle.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["F6"].SetStyle(modifiedStyle);
            worksheet.Cells["F6"].PutValue("Modified Gradient (Diagonal Up)");

            worksheet.Cells.SetColumnWidth(1, 30);
            worksheet.Cells.SetColumnWidth(5, 30);
            worksheet.AutoFitRow(1);
            worksheet.AutoFitRow(5);

            workbook.Save("TwoColorGradientStyleTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


