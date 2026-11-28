---
title: "SettableGlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings özelliği. Formülde dizi verisinin satırları için ayırıcıyı alır"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/
---
## SettableGlobalizationSettings.RowSeparatorOfFormulaArray property

Formülde dizi verilerindeki satırlar için ayırıcıyı alır.

```csharp
public override char RowSeparatorOfFormulaArray { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // SettableGlobalizationSettings örneği oluştur
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Formül dizileri için varsayılan satır ayırıcıyı göster
            Console.WriteLine("Default RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Formül dizileri için yeni bir satır ayırıcı ayarla
            settings.SetRowSeparatorOfFormulaArray(';');

            // Ayarları çalışma kitabına uygula
            workbook.Settings.GlobalizationSettings = settings;

            // Çalışma sayfasında bir dizi formülü oluştur
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            worksheet.Cells["A2"].SetArrayFormula("=SUM(A1:C2)", 1, 1);

            // Formülleri hesapla
            workbook.CalculateFormula();

            // Çalışma kitabını kaydedin
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


