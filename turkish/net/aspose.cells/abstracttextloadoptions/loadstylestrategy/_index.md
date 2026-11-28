---
title: "AbstractTextLoadOptions.LoadStyleStrategy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractTextLoadOptions özelliği. Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrıştırılan değerler için uygulanacak stil stratejisini gösterir"
type: docs
url: /tr/net/aspose.cells/abstracttextloadoptions/loadstylestrategy/
---
## AbstractTextLoadOptions.LoadStyleStrategy property

Dize değerini sayıya veya tarih-zamanına dönüştürürken ayrılan değerlere stil uygulama stratejisini belirtir.

```csharp
public TxtLoadStyleStrategy LoadStyleStrategy { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyLoadStyleStrategyDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Demonstrasyon için özel bir stil ayarlayın
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.Name = "Arial";
            customStyle.Font.Size = 12;
            customStyle.Font.Color = System.Drawing.Color.Blue;
            customStyle.Pattern = BackgroundType.Solid;
            customStyle.ForegroundColor = System.Drawing.Color.LightYellow;

            // Stili bir hücreye uygula
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(customStyle);

            // CSV verisi oluşturun
            string csvData = "Data1,Data2\nValue1,Value2";
            byte[] byteArray = Encoding.ASCII.GetBytes(csvData);
            MemoryStream stream = new MemoryStream(byteArray);

            // LoadStyleStrategy ile metin yükleme seçenekleri oluşturun
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn
            };

            // Belirtilen yükleme seçenekleriyle CSV verisini içe aktarın
            cells.ImportCSV(stream, loadOptions, 0, 0);

            // Sonucu göstermek için çalışma kitabını kaydet
            workbook.Save("LoadStyleStrategyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* enum [TxtLoadStyleStrategy](../../txtloadstylestrategy/)
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


