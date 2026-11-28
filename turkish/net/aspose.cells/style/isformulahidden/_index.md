---
title: "Style.IsFormulaHidden"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Çalışma sayfası korunduğunda formülün gizlenip gizlenmeyeceğini temsil eder"
type: docs
url: /tr/net/aspose.cells/style/isformulahidden/
---
## Style.IsFormulaHidden property

Çalışma sayfası korunduğunda formülün gizlenip gizlenmeyeceğini temsil eder.

```csharp
public bool IsFormulaHidden { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFormulaHiddenDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // IsFormulaHidden özelliği true olarak ayarlanmış bir stil oluştur
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;
            
            // Stili bir hücreye uygula
            cells["A1"].SetStyle(style);
            cells["A1"].Formula = "=1+1";

            // IsFormulaHidden özelliği false olarak ayarlanmış başka bir stil oluştur
            Style style2 = workbook.CreateStyle();
            style2.IsFormulaHidden = false;
            
            // İkinci stili başka bir hücreye uygula
            cells["B1"].SetStyle(style2);
            cells["B1"].Formula = "=2+2";

            // Etkiyi görmek için çalışma sayfasını koru
            worksheet.Protect(ProtectionType.All, "password", null);

            // Çalışma kitabını kaydedin
            workbook.Save("IsFormulaHiddenDemo.xlsx");

            Console.WriteLine("Workbook saved with IsFormulaHidden examples.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


