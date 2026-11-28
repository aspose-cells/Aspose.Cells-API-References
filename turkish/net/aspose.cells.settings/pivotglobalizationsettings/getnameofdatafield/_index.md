---
title: "PivotGlobalizationSettings.GetNameOfDataField"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotGlobalizationSettings yöntemi. Veri pivot alanının görüntüleme adını alır. Varsayılan format Alan Toplamı'dir."
type: docs
url: /tr/net/aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/
---
## PivotGlobalizationSettings.GetNameOfDataField method

Veri pivot alanının görüntüleme adını alır. Varsayılan biçim "Sum Of Field".

```csharp
public virtual string GetNameOfDataField(ConsolidationFunction function, string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fonksiyon | ConsolidationFunction | Fonksiyon, pivot alanının değerlerini özetlemek için kullanılır. |
| name | String | Pivot alanının orijinal adı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetNameOfDataFieldWithConsolidationFuStringDemo
    {
        public static void Run()
        {
            try
            {
                // PivotGlobalizationSettings örneği oluştur
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // GetNameOfDataField yöntemi için parametreleri tanımla
                ConsolidationFunction function = ConsolidationFunction.Sum;
                string fieldName = "Sales";

                // GetNameOfDataField yöntemini çağır
                string result = globalizationSettings.GetNameOfDataField(function, fieldName);

                // Sonucu çıktı olarak ver
                Console.WriteLine($"Localized name for data field '{fieldName}' with function '{function}': {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNameOfDataField: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


