---
title: "VerticalPageBreakCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VerticalPageBreakCollection yöntemi. Koleksiyona dikey bir sayfa sonu ekler"
type: docs
url: /tr/net/aspose.cells/verticalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Koleksiyona bir dikey sayfa kesmesi ekler.

```csharp
public int Add(int startRow, int endRow, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Başlangıç satır indeksi, sıfır tabanlı. |
| endRow | Int32 | Bitiş satır indeksi, sıfır tabanlı. |
| sütun | Int32 | Sütun indeksi, sıfır tabanlı. |

### Dönüş Değeri

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Açıklamalar

Bu yöntem, bir baskı alanı içinde dikey sayfa kesmesi eklemek için kullanılır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;
            
            // (Int32, Int32, Int32) parametreleriyle Add yöntemini gösterin
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            
            // Bağlam için ek örnekler
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3

            Console.WriteLine("Vertical Page Breaks:");
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"{i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
            }

            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Koleksiyona bir dikey sayfa kesmesi ekler.

```csharp
public int Add(int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Hücre sütun indeksi, sıfır tabanlı. |

### Dönüş Değeri

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Açıklamalar

Sayfa kesmesi hücrenin sol üst köşesine eklenir. Lütfen aynı anda bir yatay ve bir dikey sayfa kesmesi ayarlayın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Int32 parametresiyle Add yöntemini gösterin
            verticalPageBreaks.Add(4); // Add vertical page break at column 4

            // Eklenen sayfa kesmesi detaylarını yazdırın
            VerticalPageBreak vpb = verticalPageBreaks[0];
            Console.WriteLine($"Vertical Page Break: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");

            workbook.Save("VerticalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Koleksiyona bir dikey sayfa kesmesi ekler.

```csharp
public int Add(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Hücre satır indeksi, sıfır tabanlı. |
| sütun | Int32 | Hücre sütun indeksi, sıfır tabanlı. |

### Dönüş Değeri

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Açıklamalar

Sayfa kesmesi hücrenin sol üst köşesine eklenir. Lütfen aynı anda bir yatay ve bir dikey sayfa kesmesi ayarlayın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dikey sayfa kesmeleri koleksiyonunu alın
            VerticalPageBreakCollection vPageBreaks = worksheet.VerticalPageBreaks;

            // Farklı sütun konumlarında dikey sayfa kesmeleri ekleyin
            vPageBreaks.Add(0, 5);  // Add page break after column 5
            vPageBreaks.Add(0, 10); // Add page break after column 10
            vPageBreaks.Add(0, 15); // Add page break after column 15

            // Sayfa kesmelerini görselleştirmek için örnek veri ekleyin
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Koleksiyona bir dikey sayfa kesmesi ekler.

```csharp
public int Add(string cellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String | Hücre adı. |

### Dönüş Değeri

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Açıklamalar

Sayfa kesmesi hücrenin sol üst köşesine eklenir. Lütfen aynı anda bir yatay ve bir dikey sayfa kesmesi ayarlayın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.VerticalPageBreaks.Add("G5");
            
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### Ayrıca Bakınız

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


