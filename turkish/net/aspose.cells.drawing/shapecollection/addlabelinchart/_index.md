---
title: "ShapeCollection.AddLabelInChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Grafiğe bir etiket ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addlabelinchart/
---
## ShapeCollection.AddLabelInChart method

Grafiğe bir label ekler.

```csharp
public Label AddLabelInChart(int top, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üst | Int32 | Etiketin sol üst köşeden dikey kaydırmasını grafik alanının 1/4000 biriminde temsil eder. |
| sol | Int32 | Etiketin sol üst köşeden dikey kaydırmasını grafik alanının 1/4000 biriminde temsil eder. |
| yükseklik | Int32 | Etiketin yüksekliğini grafik alanının 1/4000 biriminde temsil eder. |
| genişlik | Int32 | Etiketin genişliğini grafik alanının 1/4000 biriminde temsil eder. |

### Dönüş Değeri

Yeni bir Label nesnesi.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir grafik oluşturmak için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];            
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // AddLabelInChart yöntemini (üst, sol, yükseklik, genişlik) parametreleriyle çağırın
                Label label = chart.Shapes.AddLabelInChart(100, 100, 200, 200);
                
                // Etiket özelliklerini ayarlayın
                label.Text = "Sample Chart Label";
                label.Font.Color = System.Drawing.Color.Red;
                label.Font.Size = 12;

                Console.WriteLine("Label added successfully to chart with parameters (100, 100, 200, 50)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddLabelInChart method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


