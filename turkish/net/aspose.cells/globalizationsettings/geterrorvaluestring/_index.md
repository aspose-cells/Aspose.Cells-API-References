---
title: "GlobalizationSettings.GetErrorValueString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings yöntemi. Hücre hata değeri için görüntüleme dize değerini alır"
type: docs
url: /tr/net/aspose.cells/globalizationsettings/geterrorvaluestring/
---
## GlobalizationSettings.GetErrorValueString method

Hücrenin hata değerinin görüntüleme dizesi değerini alır

```csharp
public virtual string GetErrorValueString(string err)
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

    public class GlobalizationSettingsMethodGetErrorValueStringWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özel küreselleştirme ayarlarını ayarla
            workbook.Settings.GlobalizationSettings = new CustomErrorGlobalizationSettings();

            // Hata senaryosu oluştur: Sıfıra bölme
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=1/0";  // This will generate #DIV/0! error

            try
            {
                workbook.CalculateFormula();
                string errorValue = cell.DisplayStringValue;
                
                Console.WriteLine($"Error display value: {errorValue}");
                Console.WriteLine("Method executed successfully - see custom error mapping");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }

            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }

    public class CustomErrorGlobalizationSettings : GlobalizationSettings
    {
        public override string GetErrorValueString(string err)
        {
            // Özel hata değeri eşlemeleri
            return err switch
            {
                "#DIV/0!" => "Custom Division Error",
                "#VALUE!" => "Custom Type Mismatch",
                "#NAME?" => "Custom Identifier Error",
                _ => base.GetErrorValueString(err)
            };
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


