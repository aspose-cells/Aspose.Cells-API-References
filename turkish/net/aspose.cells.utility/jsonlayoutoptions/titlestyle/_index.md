---
title: "JsonLayoutOptions.TitleStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonLayoutOptions özelliği. Başlığın stilini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.utility/jsonlayoutoptions/titlestyle/
---
## JsonLayoutOptions.TitleStyle property

Başlığın stilini alır ve ayarlar.

```csharp
public Style TitleStyle { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyTitleStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek JSON verisi
            string jsonInput = @"
            {
                ""Name"": ""John"",
                ""Age"": 30,
                ""JoinDate"": ""2023-05-15""
            }";

            // Başlıklar için özel stil oluştur
            CellsFactory factory = new CellsFactory();
            Style titleStyle = factory.CreateStyle();
            titleStyle.HorizontalAlignment = TextAlignmentType.Center;
            titleStyle.Font.Color = System.Drawing.Color.BlueViolet;
            titleStyle.Font.IsBold = true;

            // JSON içe aktarma seçeneklerini yapılandır
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.TitleStyle = titleStyle;
            options.ConvertNumericOrDate = true;
            options.DateFormat = "yyyy-MM-dd";

            // JSON verilerini özel başlık stiliyle içe aktar
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);

            // Daha iyi görünürlük için sütunları otomatik sığdır
            worksheet.AutoFitColumns();

            // Çalışma kitabını kaydedin
            workbook.Save("JsonWithStyledTitles.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../../aspose.cells/style/)
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


