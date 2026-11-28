---
title: "Row.GetEnumerator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Row yöntemi. Hücre sayacısını alır"
type: docs
url: /tr/net/aspose.cells/row/getenumerator/
---
## GetEnumerator() {#getenumerator}

Hücre enumeratörünü alır.

```csharp
public IEnumerator GetEnumerator()
```

### Dönüş Değeri

Bu satırdaki mevcut tüm hücreleri dolaşacak hücre sayacısı.

### Örnekler

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Biraz örnek veri doldurun
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            // İlk satır (başlık satırı) için sayacı al
            IEnumerator en = cells.Rows[0].GetEnumerator();
            while (en.MoveNext())
            {
                Cell cell = (Cell)en.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Bu satırdaki hücreleri yineleyen bir enumeratör alır.

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ters | Boolean | hücreleri ters sırada yineleyip yinelemeyeceği |
| senkron | Boolean | döndürülen sayacının bu satırdaki hücrelerin değişimini kontrol edip onunla senkronize kalıp kalmayacağı. |

### Dönüş Değeri

Bu satırdaki mevcut tüm hücreleri dolaşacak hücre sayacısı.

### Açıklamalar

Eğer satır, sayacı kullanarak dolaşma sırasında (yeni Hücre oluşturulmasına veya mevcut Hücre'nin kaldırılmasına neden olabilecek işlemlerle) değiştirilecekse, normal sayıcı yerine senkronize sayıcı kullanılmalıdır, böylece dolaşma son MoveNext() tarafından dolaşılmış olan konumun hemen sonrasından devam edebilir. Bununla birlikte, hiçbir öğenin atlanmaması veya tekrar dolaşılmaması avantajına ek olarak, senkronize sayıcının dezavantajı, normal sayıcıya kıyasla performansın biraz düşmesidir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk satırdaki hücrelere bazı veriler ekle
            Row row = worksheet.Cells.Rows[0];
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            try
            {
                // reversed=false ve sync=true ile GetEnumerator'ı çağır
                IEnumerator enumerator = row.GetEnumerator(false, true);
                
                Console.WriteLine("Cells in row 1:");
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }

                // reversed=true ve sync=false ile GetEnumerator'ı çağırarak ters yinelemeyi göster
                Console.WriteLine("\nCells in row 1 (reversed order):");
                enumerator = row.GetEnumerator(true, false);
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("RowMethodGetEnumeratorWithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


