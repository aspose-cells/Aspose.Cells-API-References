---
title: "UnionRange.Union"
second_title: "Aspose.Cells için .NET API Referansı"
description: "UnionRange metodu. Başka bir aralığı birleştir"
type: docs
url: /tr/net/aspose.cells/unionrange/union/
---
## Union(string) {#union_2}

Başka bir aralığı birleştir.

```csharp
public UnionRange Union(string range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | String | Aralık. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk aralığı oluştur ve veri ile doldur
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            range1[0, 0].PutValue("Range1");
            range1[0, 1].PutValue(100);
            range1[1, 0].PutValue("Data");
            range1[1, 1].PutValue(200);

            // İlk aralıktan UnionRange oluştur
            UnionRange unionRange = worksheet.Cells.CreateRange(range1.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range1 });

            try
            {
                // Başka bir aralığı temsil eden string parametresiyle Union metodunu çağır
                UnionRange combinedRange = unionRange.Union("C1:D2");

                // İkinci aralığı veri ile doldur
                worksheet.Cells["C1"].PutValue("Range2");
                worksheet.Cells["D1"].PutValue(300);
                worksheet.Cells["C2"].PutValue("More");
                worksheet.Cells["D2"].PutValue(400);

                Console.WriteLine("Union method executed successfully with parameter (String)");
                Console.WriteLine($"Combined range refers to: {combinedRange.RefersTo}");
                Console.WriteLine($"Total ranges in union: {combinedRange.RangeCount}");

                // Birleştirilmiş aralık hakkında bilgi göster
                Console.WriteLine("\nCombined Range Info:");
                Console.WriteLine($"FirstRow: {combinedRange.FirstRow}, FirstColumn: {combinedRange.FirstColumn}");
                Console.WriteLine($"RowCount: {combinedRange.RowCount}, ColumnCount: {combinedRange.ColumnCount}");
                Console.WriteLine($"CellCount: {combinedRange.CellCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("UnionRangeMethodUnionWithStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Union(UnionRange) {#union_1}

Başka bir aralığı birleştir.

```csharp
public UnionRange Union(UnionRange unionRange)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| unionRange | UnionRange | Aralık. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithUnionRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk aralığı oluştur ve veri ile doldur
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            range1[0, 0].PutValue("Range1");
            range1[0, 1].PutValue(100);
            range1[1, 0].PutValue("Data");
            range1[1, 1].PutValue(200);

            // İkinci aralığı oluştur ve veri ile doldur
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1:D2");
            range2[0, 0].PutValue("Range2");
            range2[0, 1].PutValue(300);
            range2[1, 0].PutValue("More");
            range2[1, 1].PutValue(400);

            // İlk aralıktan UnionRange oluştur
            UnionRange unionRange1 = worksheet.Cells.CreateRange(range1.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range1 });

            // İkinci aralıktan UnionRange oluştur
            UnionRange unionRange2 = worksheet.Cells.CreateRange(range2.RefersTo).UnionRanges(new Aspose.Cells.Range[] { range2 });

            try
            {
                // UnionRange parametresiyle Union metodunu çağır
                UnionRange combinedRange = unionRange1.Union(unionRange2);

                Console.WriteLine("Union method executed successfully with parameter (UnionRange)");
                Console.WriteLine($"Combined range refers to: {combinedRange.RefersTo}");
                Console.WriteLine($"Total ranges in union: {combinedRange.RangeCount}");

                // Birleştirilmiş aralık hakkında bilgi göster
                Console.WriteLine("\nCombined Range Info:");
                Console.WriteLine($"FirstRow: {combinedRange.FirstRow}, FirstColumn: {combinedRange.FirstColumn}");
                Console.WriteLine($"RowCount: {combinedRange.RowCount}, ColumnCount: {combinedRange.ColumnCount}");
                Console.WriteLine($"CellCount: {combinedRange.CellCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("UnionRangeMethodUnionWithUnionRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Union(Range[]) {#union}

Aralıkları birleştir.

```csharp
public UnionRange Union(Range[] ranges)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralıklar | Range[] | Aralıklar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodUnionWithRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Birleştirmeyi göstermek için örnek aralıklar oluştur
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C3:D4");
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("E5:F6");

            // Aralıkları görselleştirmek için değerleri koy
            range1[0, 0].PutValue("Range1");
            range2[0, 0].PutValue("Range2");
            range3[0, 0].PutValue("Range3");

            try
            {
                // İlk birleştirme aralığını oluştur
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range1 });

                // Range[] parametresiyle Union metodunu çağır
                Aspose.Cells.Range[] rangesToUnion = new Aspose.Cells.Range[] { range2, range3 };
                UnionRange resultUnion = unionRange.Union(rangesToUnion);

                Console.WriteLine("Union method executed successfully with parameters (Range[])");
                Console.WriteLine($"Resulting union range count: {resultUnion.RangeCount}");
                Console.WriteLine($"Resulting union refers to: {resultUnion.RefersTo}");

                // Birleşim sonucunu arka plan rengini ayarlayarak vurgulayın
                Style highlightStyle = workbook.CreateStyle();
                highlightStyle.ForegroundColor = System.Drawing.Color.LightYellow;
                highlightStyle.Pattern = BackgroundType.Solid;
                resultUnion.SetStyle(highlightStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Union method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("UnionRangeMethodUnionWithRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


