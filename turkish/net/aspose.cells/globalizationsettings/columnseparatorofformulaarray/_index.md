---
title: "GlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings özelliği. Formüldeki dizi satır verilerindeki öğeler için ayırıcıyı alır"
type: docs
url: /tr/net/aspose.cells/globalizationsettings/columnseparatorofformulaarray/
---
## GlobalizationSettings.ColumnSeparatorOfFormulaArray property

Formülde dizi satır verilerindeki öğeler için ayırıcıyı alır.

```csharp
public virtual char ColumnSeparatorOfFormulaArray { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Geçersiz kılınmış sütun ayırıcıyla özel küreselleştirme ayarları oluştur
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Mevcut sütun ayırıcı değerini göster
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " +
                globalizationSettings.ColumnSeparatorOfFormulaArray);

            // Özel ayırıcı kullanarak dizi formülü oluştur
            Cell cell = worksheet.Cells["A1"];
            cell.SetArrayFormula("=SUM({1;2;3;4})", 1, 1); // Uses custom ';' column separator

            // Formül depolamayı doğrula (gerçek formül dizesinde noktalı virgüller gösterir)
            Console.WriteLine("Stored array formula: " + cell.Formula);

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ColumnSeparatorOfFormulaArray => ';';
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


