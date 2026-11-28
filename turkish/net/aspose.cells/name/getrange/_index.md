---
title: "Name.GetRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Name yöntemi. Bu isim bir aralığa işaret ediyorsa aralığı alır"
type: docs
url: /tr/net/aspose.cells/name/getrange/
---
## GetRange() {#getrange}

Bu ad bir aralığa referans veriyorsa aralığı alır.

```csharp
public Range GetRange()
```

### Dönüş Değeri

Aralık.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // Adlandırılmış bir aralık oluştur
            int index = workbook.Worksheets.Names.Add("MyRange");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!A1:B3";
            Name namedRange = workbook.Worksheets.Names[index];
            
            // GetRange yöntemini göster
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Named Range Address: " + range.Address);
            Console.WriteLine("Worksheet Name: " + range.Worksheet.Name);
            
            // Aralığı değiştir
            foreach (Cell cell in range)
            {
                if (cell.Row == 0)
                {
                    cell.PutValue(cell.StringValue.ToUpper());
                }
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(bool) {#getrange_1}

Bu ad bir aralığa referans veriyorsa aralığı alır

```csharp
public Range GetRange(bool recalculate)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yeniden hesapla | Boolean | Bu ad bu çağrıdan önce hesaplandıysa yeniden hesaplayıp hesaplamama. |

### Dönüş Değeri

Aralık.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Örnek verileri doldur
            for (int i = 0; i < 4; i++)
            {
                cells[i, 1].PutValue(i); // Column B values: 0,1,2,3
            }

            // Formülle bir adlandırılmış aralık oluştur
            int nameIndex = wb.Worksheets.Names.Add("testname");
            Name name = wb.Worksheets.Names[nameIndex];
            name.RefersTo = "IFERROR(Sheet1!$B$2:$B$4,-1)";

            // Formüllerde adlandırılmış aralığı kullan
            cells["C1"].Formula = "=testname";
            cells["D1"].Formula = "SUM(testname)";

            // Formülleri hesapla
            wb.CalculateFormula();

            // GetRange(true) kullanarak aralığı al
            Aspose.Cells.Range namedRange = name.GetRange(true);
            Console.WriteLine($"Named range: FirstRow={namedRange.FirstRow}, FirstColumn={namedRange.FirstColumn}, " +
                $"RowCount={namedRange.RowCount}, ColumnCount={namedRange.ColumnCount}");

            // Adlandırılmış aralığı kullanarak bir grafik oluştur
            int chartIndex = sheet.Charts.Add(ChartType.Column, 10, 1, 20, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("testname", true);
            Console.WriteLine($"Chart data points count: {chart.NSeries[0].CountOfDataValues}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(int, int, int) {#getrange_2}

Bu ad bir aralığa referans veriyorsa aralığı alır. Eğer bu adın referansı mutlak değilse, aralık farklı hücreler için değişebilir.

```csharp
public Range GetRange(int sheetIndex, int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | Int32 | İlgili sayfa indeksi. |
| satır | Int32 | İlgili satır indeksi. |
| sütun | Int32 | İlgili sütun indeksi |

### Dönüş Değeri

Aralık.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Dairy");
            
            // Doğru yöntem imzasını kullanarak bir adlandırılmış aralık oluştur
            int index = workbook.Worksheets.Names.Add("SubCat");
            workbook.Worksheets.Names["SubCat"].RefersTo = "=" + worksheet.Name + "!A2:A4";
            
            // Satır, sütun ve satır sayısı parametreleriyle GetRange kullanarak aralığı al
            Aspose.Cells.Range range = workbook.Worksheets.Names["SubCat"].GetRange(0, 0, 3);
            
            // Aralık referansını göster
            Console.WriteLine("Range refers to: " + range.RefersTo);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


