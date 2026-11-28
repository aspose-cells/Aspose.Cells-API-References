---
title: "SettableGlobalizationSettings.GetErrorValueString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Hücrelerin hata değerinin görüntüleme dizesini alır"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/geterrorvaluestring/
---
## SettableGlobalizationSettings.GetErrorValueString method

Hücrenin hata değerinin görüntüleme dizesi değerini alır

```csharp
public override string GetErrorValueString(string err)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hata | String | hata değerleri gibi #VALUE!,#NAME? |

### Dönüş Değeri

Varsayılan olarak hata değerini kendisi döndürür

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetErrorValueStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel küreselleşme ayarları oluşturun
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Hata değeri içeren bir hücre oluştur
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("#N/A");
            Style style = workbook.CreateStyle();
            cell.SetStyle(style);
            style.Number = 10; // Set format to Error value

            try
            {
                // GetErrorValueString'i hata değeri dizesiyle çağır
                string errorString = settings.GetErrorValueString("#N/A");
                
                // Sonucu göster
                Console.WriteLine("Error value string: " + errorString);

                // Dönen dizeyi başka bir hücrenin değerine ayarlayarak etkiyi göster
                worksheet.Cells["A2"].PutValue("Error representation: " + errorString);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


