---
title: "CalculationData.CellRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationData özelliği. Fonksiyonun bulunduğu hücrenin satır indeksini alır"
type: docs
url: /tr/net/aspose.cells/calculationdata/cellrow/
---
## CalculationData.CellRow property

Fonksiyonun bulunduğu hücrenin satır indeksini alır.

```csharp
public int CellRow { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCellRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı örnek veri ayarlayın
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Hesaplama seçeneklerini ayarlayın
            CalculationOptions opts = new CalculationOptions();
            opts.CustomEngine = new CustomCalculationEngine();

            // Formülleri hesapla
            workbook.CalculateFormula(opts);

            // Hesaplanan hücreye erişin ve CellRow özelliğini gösterin
            Cell calculatedCell = worksheet.Cells["A3"];
            Console.WriteLine("Calculated cell is at row: " + calculatedCell.Row);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Hesaplama verilerinden satır bilgisine erişimi göster
            if (data != null)
            {
                Console.WriteLine("Current calculation is for row: " + data.CellRow);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


