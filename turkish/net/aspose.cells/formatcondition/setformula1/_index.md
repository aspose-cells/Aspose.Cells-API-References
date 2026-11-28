---
title: "FormatCondition.SetFormula1"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition yöntemi. Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar"
type: docs
url: /tr/net/aspose.cells/formatcondition/setformula1/
---
## FormatCondition.SetFormula1 method

Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Bu biçim koşuluyla ilişkili değer veya ifade. Girdi değeri '=' ile başlıyorsa, formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak kabul edilir. '=' ile başlayan metin değeri için kullanıcı, formülü şu formatta girebilir: "=\"=...\"". |
| isR1C1 | Boolean | Formülün R1C1 formülü olup olmadığı. |
| isLocal | Boolean | Formülün yerel biçimlendirilip biçimlendirilmediği. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodSetFormula1WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Koşullu biçimlendirme aralığı ekle
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // İlk biçim koşulunu al
            FormatCondition fc = fcc[0];

            try
            {
                // SetFormula1'i (String, Boolean, Boolean) parametreleriyle çağır
                fc.SetFormula1("SUM(A1:A4)", false, false);

                // Sonucu göster
                Console.WriteLine("SetFormula1 executed successfully with formula: " + fc.Formula1);
                Console.WriteLine("Conditional formatting applied to range A1:A4 with formula: " + fc.Formula1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1 method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("FormatConditionSetFormula1Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


