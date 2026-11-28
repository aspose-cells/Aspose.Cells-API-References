---
title: "UnionRange.Intersect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange yöntemi. Başka bir aralıkla kesişir"
type: docs
url: /tr/net/aspose.cells/unionrange/intersect/
---
## Intersect(string) {#intersect_2}

Başka bir aralıkla kesişir.

```csharp
public UnionRange Intersect(string range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | String | Aralık. |

### Açıklamalar

İki UnionRange kesişmiyorsa, null döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Biraz örnek veri doldurun
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");

            // A1:B2 kapsayan bir UnionRange oluşturun
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // A1:A2 aralığını temsil eden bir dize parametresiyle Intersect'i çağırın
                UnionRange intersectionResult = unionRange.Intersect("A1:A2");

                // Kesişme hakkında bilgi gösterin
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // Kesişme alanını vurgulayın
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.BackgroundColor = System.Drawing.Color.LightGreen;
                intersectionResult.SetStyle(highlightStyle);

                Console.WriteLine("Intersect method executed successfully with parameter (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("UnionRangeMethodIntersectWithStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Intersect(UnionRange) {#intersect_1}

Başka bir aralıkla kesişir.

```csharp
public UnionRange Intersect(UnionRange unionRange)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| unionRange | UnionRange | Aralık. |

### Açıklamalar

İki UnionRange kesişmiyorsa, null döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithUnionRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["C1"].PutValue("C1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");
            worksheet.Cells["C2"].PutValue("C2");

            // İki UnionRange oluşturun
            UnionRange range1 = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            UnionRange range2 = worksheet.Cells.CreateRange("B1:C2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("B1:C2") });

            try
            {
                // UnionRange parametresiyle Intersect yöntemini çağırın
                UnionRange intersectionResult = range1.Intersect(range2);

                // Kesişme hakkında bilgi gösterin
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // Kesişme alanını vurgulayın
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.BackgroundColor = System.Drawing.Color.Yellow;
                intersectionResult.SetStyle(highlightStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("UnionRangeMethodIntersectWithUnionRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Intersect(Range[]) {#intersect}

Başka bir aralıkla kesişir.

```csharp
public UnionRange Intersect(Range[] ranges)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralıklar | Range[] | Aralık. |

### Açıklamalar

İki UnionRange kesişmiyorsa, null döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodIntersectWithRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelerde örnek veri oluştur
            worksheet.Cells["A1"].PutValue("A1");
            worksheet.Cells["B1"].PutValue("B1");
            worksheet.Cells["A2"].PutValue("A2");
            worksheet.Cells["B2"].PutValue("B2");

            // Kesişmek için aralıklar oluşturun
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B1");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A1:A2");
            Aspose.Cells.Range[] rangesToIntersect = new Aspose.Cells.Range[] { range1, range2 };

            // Çalışma sayfasının UnionRange'ini alın
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // Range[] parametresiyle Intersect yöntemini çağırın
                UnionRange intersectionResult = unionRange.Intersect(rangesToIntersect);

                // Kesişim sonucuyla ilgili bilgileri göster
                Console.WriteLine($"Intersection result range: {intersectionResult.RefersTo}");
                Console.WriteLine($"First row: {intersectionResult.FirstRow}");
                Console.WriteLine($"First column: {intersectionResult.FirstColumn}");
                Console.WriteLine($"Row count: {intersectionResult.RowCount}");
                Console.WriteLine($"Column count: {intersectionResult.ColumnCount}");

                // Kesişme alanını vurgulayın
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.Yellow;
                intersectionResult.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Intersect method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("UnionRangeMethodIntersectWithRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


