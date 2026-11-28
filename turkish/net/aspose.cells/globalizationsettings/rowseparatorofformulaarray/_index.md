---
title: "GlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings özelliği. Formüldeki dizi verisindeki satırlar için ayırıcıyı alır"
type: docs
url: /tr/net/aspose.cells/globalizationsettings/rowseparatorofformulaarray/
---
## GlobalizationSettings.RowSeparatorOfFormulaArray property

Formülde dizi verilerindeki satırlar için ayırıcıyı alır.

```csharp
public virtual char RowSeparatorOfFormulaArray { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Özel küreselleştirme ayarlarıyla yeni bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel küreselleştirme ayarları örneğine erişin
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            // RowSeparatorOfFormulaArray öğesinin mevcut değerini göster
            Console.WriteLine("Current RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Özel satır ayırıcıyı kullanarak bir dizi formülü oluşturun
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=SUM({1,2|3,4})"; // Uses '|' as row separator

            // Doğru ayrıştırmayı göstermek için formülü hesaplayın
            workbook.CalculateFormula();

            // Sonuçları göster
            Console.WriteLine("Array formula using custom separator: " + cell.Formula);
            Console.WriteLine("Calculated result: " + cell.Value);

            // Çalışma kitabını kaydedin
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }

    // Satır ayırıcısını geçersiz kılan özel GlobalizationSettings uygulaması
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override char RowSeparatorOfFormulaArray => '|';
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


