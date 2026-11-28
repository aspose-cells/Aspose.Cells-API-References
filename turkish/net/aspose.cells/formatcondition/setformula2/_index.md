---
title: "FormatCondition.SetFormula2"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition yöntemi. Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar"
type: docs
url: /tr/net/aspose.cells/formatcondition/setformula2/
---
## FormatCondition.SetFormula2 method

Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodSetFormula2WithStringBooleanBooleanDemo
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

            // Bir biçim koşulu ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // İlk biçim koşulunu al
            FormatCondition fc = fcs[0];

            try
            {
                // SetFormula2'yi (String, Boolean, Boolean) parametreleriyle çağır
                fc.SetFormula2("25", false, false);

                // Sonucu göster
                Console.WriteLine("SetFormula2 executed successfully. New Formula2: " + fc.Formula2);
                Console.WriteLine("Cells A1:A4 will be formatted if their values are between 10 and 25");

                // Etkiyi görünür kılmak için bazı stiller uygula
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightGreen;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula2 method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("FormatConditionSetFormula2Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


