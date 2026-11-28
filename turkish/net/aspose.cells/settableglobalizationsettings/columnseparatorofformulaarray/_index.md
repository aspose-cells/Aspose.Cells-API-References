---
title: "SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings özelliği. Formüldeki dizi satır verilerindeki öğeler için ayırıcıyı alır"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/
---
## SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray property

Formülde dizi satır verilerindeki öğeler için ayırıcıyı alır.

```csharp
public override char ColumnSeparatorOfFormulaArray { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // SettableGlobalizationSettings örneği oluştur
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // ColumnSeparatorOfFormulaArray öğesinin mevcut değerini göster
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " + settings.ColumnSeparatorOfFormulaArray);

            // ColumnSeparatorOfFormulaArray için yeni bir değer ayarla
            settings.SetColumnSeparatorOfFormulaArray(';');

            // Ayarları çalışma kitabına uygula
            workbook.Settings.GlobalizationSettings = settings;

            // SetArrayFormula kullanarak özel ayırıcı ile bir dizi formülü oluştur
            worksheet.Cells["A1"].SetArrayFormula("SUM({1,2,3;4,5,6})", 1, 1);
            worksheet.Cells["A2"].Formula = "=SUM(A1)";

            // Formülleri hesapla
            workbook.CalculateFormula();

            // Sonucu göster
            Console.WriteLine("Result of array formula calculation: " + worksheet.Cells["A2"].Value);

            // Çalışma kitabını kaydedin
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


