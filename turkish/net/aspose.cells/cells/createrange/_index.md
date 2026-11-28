---
title: "Cells.CreateRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Hücre aralığından bir Range nesnesi oluşturur"
type: docs
url: /tr/net/aspose.cells/cells/createrange/
---
## CreateRange(string, string) {#createrange_3}

Bir hücre aralığından bir [`Range`](../../range/) nesnesi oluşturur.

```csharp
public Range CreateRange(string upperLeftCell, string lowerRightCell)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| upperLeftCell | String | Üst sol hücre adı. |
| lowerRightCell | String | Alt sağ hücre adı. |

### Dönüş Değeri

Bir [`Range`](../../range/) nesnesi

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // A1'den A2'ye bir aralık oluştur
            Aspose.Cells.Range range = cells.CreateRange("A1", "A2");
            range.Name = "MyRange";
            
            // Aralıktaki değerleri ayarla
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            
            // Formülde aralığı kullan
            cells["B1"].Formula = "=SUM(MyRange)";
            
            // Formülü hesapla
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of MyRange (A1:A2) is: " + cells["B1"].IntValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, int, int) {#createrange_1}

Bir hücre aralığından bir [`Range`](../../range/) nesnesi oluşturur.

```csharp
public Range CreateRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Bu aralığın ilk satırı |
| firstColumn | Int32 | Bu aralığın ilk sütunu |
| totalRows | Int32 | Satır sayısı |
| totalColumns | Int32 | Sütun sayısı |

### Dönüş Değeri

Bir [`Range`](../../range/) nesnesi

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Kaynak aralığı oluştur (başlangıç satırı 2, sütun 2, 3 satır ve 4 sütun ile)
            Aspose.Cells.Range rangeSrc = cells.CreateRange(2, 2, 3, 4);

            // Kaynak aralığı örnek veriyle doldurun
            for (int i = 0; i < rangeSrc.RowCount; i++)
            {
                for (int j = 0; j < rangeSrc.ColumnCount; j++)
                {
                    rangeSrc[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Hedef aralığı oluştur (başlangıç satırı 8, sütun 0 ve aynı boyutlarda)
            Aspose.Cells.Range rangeDest = cells.CreateRange(8, 0, 3, 4);

            // Değerleri kaynaktan hedefe kopyalayın
            rangeDest.CopyValue(rangeSrc);

            // Çalışma kitabını kaydedin
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(string) {#createrange_2}

Bir [`Range`](../../range/) nesnesini aralığın adresinden oluşturur.

```csharp
public Range CreateRange(string address)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| address | String | Aralığın adresi. |

### Dönüş Değeri

Bir [`Range`](../../range/) nesnesi

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dize adresi kullanarak bir aralık oluşturun
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Aralıktaki verileri doldurun
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Yeni bir çalışma sayfasında başka bir aralık oluşturun
            workbook.Worksheets.Add();
            Worksheet worksheet2 = workbook.Worksheets[1];
            Aspose.Cells.Range range2 = worksheet2.Cells.CreateRange("A1:C3");

            // Aralıklar arasında verileri kopyalayın
            range2.Copy(range);

            // Çalışma kitabını kaydedin
            workbook.Save("CreateRangeWithStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, bool) {#createrange}

Hücre satırlarından veya hücre sütunlarından bir [`Range`](../../range/) nesnesi oluşturur.

```csharp
public Range CreateRange(int firstIndex, int number, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | Int32 | İlk satır indeksi veya ilk sütun indeksi, sıfır tabanlı. |
| sayı | Int32 | Satır veya sütunların toplam sayısı, bir tabanlı. |
| isVertical | Boolean | Doğru - Aralık hücre sütunlarından oluşturulur. Yanlış - Aralık hücre satırlarından oluşturulur. |

### Dönüş Değeri

Bir [`Range`](../../range/) nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // A1 (0,0) hücresinden başlayarak 5 satır ve 3 sütunlu bir aralık oluşturun
            Aspose.Cells.Range range = cells.CreateRange(0, 0, true);

            // Aralığa bazı verileri doldurun
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Row {i}, Col {j}");
                }
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


