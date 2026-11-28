---
title: "RowCollection.GetEnumerator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RowCollection yöntemi. Bu koleksiyon içinde satırları yineleyen bir enumerator döndürür."
type: docs
url: /tr/net/aspose.cells/rowcollection/getenumerator/
---
## GetEnumerator() {#getenumerator}

Bu koleksiyon üzerinden satırları yineleyen bir enumerator alır.

```csharp
public IEnumerator GetEnumerator()
```

### Dönüş Değeri

Bu koleksiyondaki mevcut tüm satırları dolaşacak satır enumerator'ı.

### Örnekler

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gösterim için satır yüksekliklerini ayarla
            worksheet.Cells.SetRowHeight(0, 15);
            worksheet.Cells.SetRowHeight(1, 20);
            worksheet.Cells.SetRowHeight(2, 25);

            IEnumerator enumerator = worksheet.Cells.Rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine($"Row index: {row.Index}, Height: {row.Height}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Bu koleksiyon üzerinden satırları yineleyen bir enumerator alır.

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ters | Boolean | satırları ters sırada yineleyip yinelemeyeceği |
| senkron | Boolean | dönen enumerator'ün satır koleksiyonundaki değişiklikleri kontrol edip onunla senkronize kalıp kalmayacağı. |

### Dönüş Değeri

Bu koleksiyondaki mevcut tüm satırları dolaşacak satır enumerator'ı.

### Açıklamalar

Eğer satır koleksiyonu, enumerator ile dolaşma sırasında (yeni Row nesnesi oluşturulmasına veya mevcut Row nesnesinin kaldırılmasına neden olabilecek işlemlerle) değiştirilirse, dolaşmanın son MoveNext() çağrısından hemen sonraki konumdan devam edebilmesi için normal enumerator yerine senkronize enumerator kullanılmalıdır. Bununla birlikte, hiçbir öğenin atlanmaması veya tekrar tekrar dolaşılmaması avantajı sağlarken, senkronize enumerator'ün dezavantajı, normal enumerator ile karşılaştırıldığında performansın biraz düşmesidir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satırlara örnek veri ekle
            for (int i = 0; i < 5; i++)
            {
                Row row = worksheet.Cells.Rows[i];
                row[0].PutValue($"Row {i + 1}");
            }
            
            try
            {
                // RowCollection'ı al
                RowCollection rows = worksheet.Cells.Rows;
                
                // GetEnumerator'ı (reversed: true, sync: false) parametreleriyle çağır
                IEnumerator enumerator = rows.GetEnumerator(true, false);
                
                Console.WriteLine("Iterating rows in reverse order:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
                
                // GetEnumerator'ı (reversed: false, sync: true) parametreleriyle çağır
                enumerator = rows.GetEnumerator(false, true);
                
                Console.WriteLine("\nIterating rows in normal order (synchronized):");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("RowCollectionGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


