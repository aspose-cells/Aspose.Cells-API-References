---
title: "UnionRange.PutValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange yöntemi. Değeri aralığa koyar; uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrelerin sayı biçimi sıfırlanır"
type: docs
url: /tr/net/aspose.cells/unionrange/putvalue/
---
## UnionRange.PutValue method

Bir değeri aralığa koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringValue | String | Giriş değeri |
| isConverted | Boolean | Doğru: uygun ise başka veri tipine dönüştürüldü. |
| setStyle | Boolean | Doğru: başka veri tipine dönüştürürken sayı formatını hücrenin stiline ayarla |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1'den B2'ye kadar hücreleri kapsayan bir birleşim aralığı oluşturun
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            
            try
            {
                // PutValue yöntemini şu parametrelerle çağırın: (String, Boolean, Boolean)
                unionRange.PutValue("Sample Value", true, true);
                
                Console.WriteLine("PutValue method executed successfully with parameters (String, Boolean, Boolean)");
                
                // Etkiyi göstermek için aralık bilgilerini görüntüleyin
                Console.WriteLine($"Range address: {unionRange.RefersTo}");
                Console.WriteLine($"Value set in range: {unionRange.Value}");
                
                // Etkiyi görünür kılmak için biçimlendirme uygulayın
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.HorizontalAlignment = TextAlignmentType.Center;
                unionRange.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PutValue method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("UnionRangeMethodPutValueWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


