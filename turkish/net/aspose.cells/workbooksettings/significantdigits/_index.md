---
title: "WorkbookSettings.SignificantDigits"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Önemli basamak sayısını alır ve ayarlar. Varsayılan değer SignificantDigits'dir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/significantdigits/
---
## WorkbookSettings.SignificantDigits property

Önemli basamak sayısını alır ve ayarlar. Varsayılan değer [`SignificantDigits`](../../cellshelper/significantdigits/)'dir.

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int SignificantDigits { get; set; }
```

### Açıklamalar

Şu anda sadece 15 veya 17 olabilir. NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [`SignificantDigitsType`](../significantdigitstype/) kullanın. Bu özellik, Haziran 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Önemli basamakları göstermek için örnek sayısal veri ekle
            sheet.Cells["A1"].PutValue(123.4567890123456789);
            sheet.Cells["A2"].PutValue(0.000000000123456789);

            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;

            // Önemli basamakları 15'e ayarla (double için maksimum hassasiyet)
            settings.SignificantDigits = 15;

            // Önemli basamakların etkisini göstermek için çalışma kitabını kaydet
            workbook.Save("SignificantDigitsDemo.xlsx");

            Console.WriteLine("Workbook saved with SignificantDigits set to 15.");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


