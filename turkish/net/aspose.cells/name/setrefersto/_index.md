---
title: "Name.SetRefersTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Name yöntemi. Bu Name'in referansını ayarlayın"
type: docs
url: /tr/net/aspose.cells/name/setrefersto/
---
## Name.SetRefersTo method

Bu Name'in referansını ayarla.

```csharp
public void SetRefersTo(string refersTo, bool isR1C1, bool isLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| refersTo | String | Referans. |
| isR1C1 | Boolean | Referansın R1C1 formatında olup olmadığı. |
| isLocal | Boolean | Referansın yerel ayara göre biçimlendirilip biçimlendirilmediği. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodSetRefersToWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Adlandırılmış bir aralık oluştur
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];

            try
            {
                // SetRefersTo'yi parametrelerle (String, Boolean, Boolean) çağırın
                namedRange.SetRefersTo("=Sheet1!$A$1:$A$3", false, false);

                // Sonucu göster
                Console.WriteLine($"Named range 'MyNamedRange' now refers to: {namedRange.RefersTo}");

                // Formülde adlandırılmış aralığı kullanarak doğrula
                worksheet.Cells["B1"].Formula = "=SUM(MyNamedRange)";
                workbook.CalculateFormula();

                Console.WriteLine($"Result of SUM(MyNamedRange): {worksheet.Cells["B1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRefersTo method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("NameMethodSetRefersToWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


