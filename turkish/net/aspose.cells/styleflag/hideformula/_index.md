---
title: "StyleFlag.HideFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Formülü gizleme ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/hideformula/
---
## StyleFlag.HideFormula property

Formülü gizle ayarı uygulanacak.

```csharp
public bool HideFormula { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyHideFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell a1 = worksheet.Cells["A1"];
            // A1 hücresine bir formül ekleyin
            a1.Formula = "=1+2";
            a1.Value = 3; // Display value

            // HideFormula true olarak ayarlanmış bir stil bayrağı oluşturun
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HideFormula = true;

            // Bir stil oluşturun ve IsFormulaHidden özelliğini true olarak ayarlayın
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;

            // Stil bayrağıyla stili A1 hücresine uygulayın
            a1.SetStyle(style, styleFlag);

            // HideFormula etkisini görmek için çalışma sayfasını koruyun
            worksheet.Protection.AllowEditingObject = true;
            worksheet.Protection.AllowEditingContent = false;
            worksheet.Protection.Password = "password";

            // Çalışma kitabını kaydedin
            workbook.Save("PropertyHideFormulaDemo.xlsx");

            // Formülün gizli olduğunu doğrulayın
            Console.WriteLine("Formula in A1: " + a1.Formula);
            Console.WriteLine("Is formula hidden? " + a1.GetStyle().IsFormulaHidden);
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


