---
title: "Workbook.Theme"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Tema adını alır"
type: docs
url: /tr/net/aspose.cells/workbook/theme/
---
## Workbook.Theme property

Tema adını alır.

```csharp
public string Theme { get; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyThemeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Varsayılan temayı almayı gösterin
            Console.WriteLine("Default theme: " + workbook.Theme);
            
            // Tema rengini değiştirin ve doğrulayın
            workbook.SetThemeColor(ThemeColorType.Accent1, Color.Blue);
            Color accent1 = workbook.GetThemeColor(ThemeColorType.Accent1);
            Console.WriteLine("Modified Accent1 color: " + accent1);
            
            // Tema kalıcılığını göstermek için çalışma kitabını kaydedin
            workbook.Save("ThemeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


