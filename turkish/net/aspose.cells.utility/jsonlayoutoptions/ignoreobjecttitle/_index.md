---
title: "JsonLayoutOptions.IgnoreObjectTitle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonLayoutOptions özelliği. Nesne, bir nesnenin özelliği ise başlığın göz ardı edilip edilmediğini gösterir"
type: docs
url: /tr/net/aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/
---
## JsonLayoutOptions.IgnoreObjectTitle property

Nesne, bir nesnenin özelliği ise başlığın göz ardı edilip edilmediğini gösterir.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreObjectTitle { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen JsonLayoutOptions.IgnoreTitle özelliğini kullanın. Bu özellik Şubat 2023'ten itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class JsonLayoutOptionsPropertyIgnoreObjectTitleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Nesne başlıklarıyla örnek JSON verileri
            string json = @"{
                ""Employees"": {
                    ""Employee"": [
                        { ""Name"": ""John"", ""Age"": 30 },
                        { ""Name"": ""Jane"", ""Age"": 25 }
                    ]
                }
            }";

            // JsonLayoutOptions oluştur
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Mevcut IgnoreObjectTitle değerini göster
            Console.WriteLine("Current IgnoreObjectTitle value: " + options.IgnoreObjectTitle);

            // Nesne başlıklarını göz ardı etmek için ayarla
            options.IgnoreObjectTitle = true;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // IgnoreObjectTitle = true ile JSON içe aktar
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Göz ardı edilen başlıklarla kaydet
            workbook.Save("IgnoreObjectTitle_True.xlsx");

            // Çalışma sayfasını sıfırla
            worksheet.Cells.Clear();

            // Nesne başlıklarını dahil etmek için ayarla
            options.IgnoreObjectTitle = false;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // IgnoreObjectTitle = false ile JSON içe aktar
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Dahil edilen başlıklarla kaydet
            workbook.Save("IgnoreObjectTitle_False.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


