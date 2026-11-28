---
title: "HorizontalPageBreakCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HorizontalPageBreakCollection yöntemi. Koleksiyona bir yatay sayfa sonu ekler"
type: docs
url: /tr/net/aspose.cells/horizontalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Koleksiyona bir yatay sayfa sonu ekler.

```csharp
public int Add(int row, int startColumn, int endColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi, sıfır tabanlı. |
| startColumn | Int32 | Başlangıç sütun indeksi, sıfır tabanlı. |
| endColumn | Int32 | Bitiş sütun indeksi, sıfır tabanlı. |

### Dönüş Değeri

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Açıklamalar

Bu yöntem, bir yazdırma alanı içinde yatay sayfa sonu eklemek için kullanılır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add yöntemini (Int32, Int32, Int32) parametreleriyle göster
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Koleksiyona bir yatay sayfa sonu ekler.

```csharp
public int Add(int row)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Hücre satır indeksi, sıfır tabanlı. |

### Dönüş Değeri

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Açıklamalar

Sayfa kesmesi hücrenin sol üst köşesine eklenir. Lütfen aynı anda bir yatay ve bir dikey sayfa kesmesi ayarlayın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Int32 parametresi kullanarak yatay sayfa sonları ekle
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Koleksiyona bir yatay sayfa sonu ekler.

```csharp
public int Add(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Hücre satır indeksi, sıfır tabanlı. |
| sütun | Int32 | Hücre sütun indeksi, sıfır tabanlı. |

### Dönüş Değeri

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Açıklamalar

Sayfa kesmesi hücrenin sol üst köşesine eklenir. Lütfen aynı anda bir yatay ve bir dikey sayfa kesmesi ayarlayın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Birden fazla satır oluşturmak için örnek veri ekle
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Belirli satırlarda yatay sayfa sonları ekle
            worksheet.HorizontalPageBreaks.Add(9, 0);  // Page break after row 9
            worksheet.HorizontalPageBreaks.Add(19, 0); // Page break after row 19
            worksheet.HorizontalPageBreaks.Add(29, 0); // Page break after row 29

            // Çalışma kitabını kaydedin
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Koleksiyona bir yatay sayfa sonu ekler.

```csharp
public int Add(string cellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String | Hücre adı. |

### Dönüş Değeri

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Açıklamalar

Sayfa kesmesi hücrenin sol üst köşesine eklenir. Lütfen aynı anda bir yatay ve bir dikey sayfa kesmesi ayarlayın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satır 4'te yatay sayfa sonu ekle (D5, sıfır tabanlı indekste satır 4'tür)
            worksheet.HorizontalPageBreaks.Add("D5");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


