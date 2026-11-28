---
title: "Row.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Satır yöntemi. Bu nesnenin başka bir nesneyle aynı satıra referans olup olmadığını kontrol eder"
type: docs
url: /tr/net/aspose.cells/row/equals/
---
## Equals(object) {#equals_1}

Bu nesnenin başka bir nesneyle aynı satıra referans verip vermediğini kontrol eder.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | başka bir nesne |

### Dönüş Değeri

İki nesne aynı satıra referans veriyorsa doğru.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Karşılaştırmak için iki satır oluştur
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];
            
            // Satırları farklı kılmak için bazı özellikleri ayarla
            row1.Height = 20;
            row2.Height = 25;
            
            try
            {
                // Object parametresiyle Equals yöntemini çağır
                bool result1 = row1.Equals((object)row2);
                Console.WriteLine($"Comparing row1 with row2: {result1}");
                
                // row1'i kendisiyle karşılaştır
                bool result2 = row1.Equals((object)row1);
                Console.WriteLine($"Comparing row1 with itself: {result2}");
                
                // null ile karşılaştır
                bool result3 = row1.Equals((object)null);
                Console.WriteLine($"Comparing row1 with null: {result3}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            workbook.Save("RowMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Row) {#equals}

Bu nesnenin başka bir satır nesnesiyle aynı satıra referans verip vermediğini kontrol eder.

```csharp
public bool Equals(Row row)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Row | başka bir satır nesnesi |

### Dönüş Değeri

İki satır nesnesi aynı satıra işaret ediyorsa doğru.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Karşılaştırmak için iki satır oluştur
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];

            // Satırları farklı kılmak için bazı özellikleri ayarla
            row1.Height = 20;
            row2.Height = 25;
            row1.IsHidden = false;
            row2.IsHidden = true;

            try
            {
                // Satırları karşılaştırmak için Equals metodunu çağırın
                bool areEqual = row1.Equals(row2);

                // Sonucu göster
                Console.WriteLine($"Are rows equal? {areEqual}");

                // row1 ile aynı özelliklere sahip başka bir satır oluşturun
                Row row3 = worksheet.Cells.Rows[2];
                row3.Height = row1.Height;
                row3.IsHidden = row1.IsHidden;

                // row1'i row3 ile karşılaştırın (eşit olmalı)
                bool areEqual2 = row1.Equals(row3);
                Console.WriteLine($"Are rows equal after matching properties? {areEqual2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("RowEqualsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


