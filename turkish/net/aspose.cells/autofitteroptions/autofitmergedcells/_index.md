---
title: "AutoFitterOptions.AutoFitMergedCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFitterOptions özelliği. Hücreler bir satırda birleştirildiğinde satır yüksekliğinin otomatik olarak ayarlanıp ayarlanmayacağını gösterir. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/autofitteroptions/autofitmergedcells/
---
## AutoFitterOptions.AutoFitMergedCells property

Hücreler bir satırda birleştirildiğinde satır yüksekliğinin otomatik olarak ayarlanıp ayarlanmayacağını gösterir. Varsayılan değer false'tur.

```csharp
[Obsolete("Use AutoFitterOptions.AutoFitMergedCellsType property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AutoFitMergedCells { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen AutoFitterOptions.AutoFitMergedCellsType özelliğini kullanın. Bu özellik, Aralık 2018'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri oluşturun ve hücreleri birleştirin
            worksheet.Cells["A1"].PutValue("This is a test of AutoFitMergedCells property");
            worksheet.Cells.Merge(0, 0, 3, 3); // Merge cells A1:C3

            // AutoFitterOptions oluşturun ve AutoFitMergedCells özelliğini ayarlayın
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;

            // Birleştirilmiş hücrelerle satırları otomatik olarak ayarlayın
            worksheet.AutoFitRows(options);

            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitMergedCellsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


