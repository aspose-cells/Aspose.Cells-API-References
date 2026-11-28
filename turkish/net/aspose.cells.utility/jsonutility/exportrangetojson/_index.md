---
title: "JsonUtility.ExportRangeToJson"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonUtility yöntemi. Aralığı json dosyasına dışa aktarma"
type: docs
url: /tr/net/aspose.cells.utility/jsonutility/exportrangetojson/
---
## ExportRangeToJson(Range, ExportRangeToJsonOptions) {#exportrangetojson_1}

Aralığı json dosyasına dışa aktarma.

```csharp
[Obsolete("Use ExportRangeToJson(Range range, JsonSaveOptions options) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ExportRangeToJson(Range range, ExportRangeToJsonOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | Aralık | Aralık. |
| seçenekler | ExportRangeToJsonOptions | Dışa aktarma seçenekleri. |

### Dönüş Değeri

Json dize değeri.

### Açıklamalar

NOTE: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ExportRangeToJson(Range range, JsonSaveOptions options) yöntemini kullanın. Bu özellik Kasım 2022'den itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonUtilityMethodExportRangeToJsonWithRangeExportRangeToJsonOptionsDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Veriyi kapsayan bir aralık oluşturun
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Dışa aktarma seçeneklerini oluşturun
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.ExportAsString = true;

            // Aralığı JSON'a dışa aktar
            string json = JsonUtility.ExportRangeToJson(range, options);
            
            Console.WriteLine(json);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../../aspose.cells/range/)
* class [ExportRangeToJsonOptions](../../exportrangetojsonoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## ExportRangeToJson(Range, JsonSaveOptions) {#exportrangetojson}

Aralığı json dosyasına dışa aktarma.

```csharp
public static string ExportRangeToJson(Range range, JsonSaveOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | Aralık | Aralık. |
| seçenekler | JsonSaveOptions | Dışa aktarma seçenekleri. |

### Dönüş Değeri

Json dize değeri.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonUtilityMethodExportRangeToJsonWithRangeJsonSaveOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["C2"].PutValue("New York");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["C3"].PutValue("London");

            // Aralık oluştur (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 3);
            
            // JSON dışa aktarma seçeneklerini yapılandırın
            JsonSaveOptions options = new JsonSaveOptions();
            options.ExportEmptyCells = true;
            options.HasHeaderRow = true;
            options.ExportNestedStructure = false;

            // Aralığı JSON'a dışa aktar
            string jsonOutput = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options);
            
            // JSON sonucunu çıktılayın
            Console.WriteLine(jsonOutput);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../../aspose.cells/range/)
* class [JsonSaveOptions](../../../aspose.cells/jsonsaveoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


