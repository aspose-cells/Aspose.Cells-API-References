---
title: "ChartCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartCollection yöntemi. Koleksiyona bir grafik ekler"
type: docs
url: /tr/net/aspose.cells.charts/chartcollection/add/
---
## Add(ChartType, int, int, int, int) {#add}

Koleksiyona bir grafik ekler.

```csharp
public int Add(ChartType type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ChartType | Grafik türü |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| bottomRow | Int32 | Alt sağ satır indeksi |
| rightColumn | Int32 | Alt sağ sütun indeksi |

### Dönüş Değeri

[`Chart`](../../chart/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 1; i <= 10; i++)
            {
                sheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                sheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Belirtilen parametreleri kullanarak bir grafik ekle
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 2, 25, 11);
            Chart chart = sheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("=Sheet1!$A$1:$B$11", true);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, int, int, int, int) {#add_2}

Koleksiyona bir grafik ekler.

```csharp
[Obsolete("Use ChartCollection.Add(ChartType, string, bool ,int , int, int, int ) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ChartType type, string dataRange, int topRow, int leftColumn, int rightRow, 
    int bottomColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ChartType | Grafik türü |
| dataRange | String | Grafiğin veri aralığını belirtir |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| rightRow | Int32 | Alt sağ satır indeksi |
| bottomColumn | Int32 | Alt sağ sütun indeksi |

### Dönüş Değeri

[`Chart`](../../chart/) object index.

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen `Add` özelliğini kullanın. Bu özellik Mayıs 2022'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithChartTypeStringInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // Add yöntemini (ChartType, String, Int32, Int32, Int32, Int32) parametreleriyle çağır
                int chartIndex = worksheet.Charts.Add(
                    ChartType.Column,          // Chart type
                    "A1:B4",                  // Data range
                    0,                        // Top row position
                    3,                        // Left column position
                    15,                       // Bottom row position
                    8                         // Right column position
                );

                Console.WriteLine("Chart added successfully at index: " + chartIndex);
                
                // Yeni oluşturulan grafiğe eriş
                Chart chart = worksheet.Charts[chartIndex];
                chart.Title.Text = "Sample Column Chart";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("ChartCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(byte[], string, bool, int, int, int, int) {#add_3}

Önceden ayarlanmış şablonla bir grafik ekler.

```csharp
public int Add(byte[] data, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| veri | Byte[] | Grafik şablon dosyasının (.crtx) verileri. |
| dataRange | String | Grafiğin veri aralığını belirtir |
| isVertical | Boolean | Seriyi hücre değerleri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| rightRow | Int32 | Alt sağ satır indeksi |
| bottomColumn | Int32 | Alt sağ sütun indeksi |

### Dönüş Değeri

[`Chart`](../../chart/) object index.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithByteArrayStringBooleanInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Grafik verisini temsil eden bir bayt dizisi oluştur (basitleştirilmiş örnek)
            byte[] chartData = new byte[] { 0x01, 0x02, 0x03 };

            try
            {
                // Add metodunu belirli parametrelerle çağırın
                int chartIndex = worksheet.Charts.Add(
                    chartData,          // Byte[] data
                    "A1:B4",            // String dataRange
                    true,               // Boolean isVertical
                    0,                  // Int32 topRow
                    0,                  // Int32 leftColumn
                    15,                 // Int32 rightRow
                    8                   // Int32 bottomColumn
                );

                Console.WriteLine($"Chart added successfully at index: {chartIndex}");

                // Eklenen grafiğe eriş
                Chart chart = worksheet.Charts[chartIndex];
                chart.Type = ChartType.Column;

                // Sonucu kaydet
                workbook.Save("ChartCollectionMethodAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, bool, int, int, int, int) {#add_1}

Koleksiyona bir grafik ekler.

```csharp
public int Add(ChartType type, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ChartType | Grafik türü |
| dataRange | String | Grafiğin veri aralığını belirtir |
| isVertical | Boolean | Seriyi hücre değerleri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| rightRow | Int32 | Alt sağ satır indeksi |
| bottomColumn | Int32 | Alt sağ sütun indeksi |

### Dönüş Değeri

[`Chart`](../../chart/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeStringBooleanInt32IntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);

            // Belirtilen parametrelerle grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, "A1:C3", true, 4, 4, 14, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


