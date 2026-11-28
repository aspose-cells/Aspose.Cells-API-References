---
title: "Cells.Merge"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen hücre aralığını tek bir hücreye birleştirir"
type: docs
url: /tr/net/aspose.cells/cells/merge/
---
## Merge(int, int, int, int) {#merge}

Belirtilen hücre aralığını tek bir hücrede birleştirir.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Bu aralığın ilk satırı (sıfır tabanlı) |
| firstColumn | Int32 | Bu aralığın ilk sütunu (sıfır tabanlı) |
| totalRows | Int32 | Satır sayısı (bir tabanlı) |
| totalColumns | Int32 | Sütun sayısı (bir tabanlı) |

### Açıklamalar

Birleştirilmiş hücreye, aralıktaki sol üst hücrenin adresi üzerinden başvurun.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Birleştirmeyi göstermek için hücrelere değerler koyun
            cells[0, 0].PutValue("Merged Area");
            cells[5, 5].PutValue("Not Merged");

            // Satır 0, sütun 0'dan başlayarak 3 satır ve 2 sütun kapsayan hücreleri birleştirin
            cells.Merge(0, 0, 3, 2);

            // Çalışma kitabını kaydedin
            workbook.Save("MergeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool) {#merge_1}

Belirtilen hücre aralığını tek bir hücrede birleştirir.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool mergeConflict)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Bu aralığın ilk satırı (sıfır tabanlı) |
| firstColumn | Int32 | Bu aralığın ilk sütunu (sıfır tabanlı) |
| totalRows | Int32 | Satır sayısı (bir tabanlı) |
| totalColumns | Int32 | Sütun sayısı (bir tabanlı) |
| mergeConflict | Boolean | Birleştirme çakışması birleştirilmiş aralıklar. |

### Açıklamalar

Birleştirilmiş hücreye, aralıktaki sol üst hücrenin adresi üzerinden başvurun. mergeConflict true ise ve birleştirilmiş aralık diğer birleştirilmiş hücrelerle çakışırsa, diğer birleştirilmiş hücreler otomatik olarak kaldırılacaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satır 3, sütun 4 (D3) ile satır 7, sütun 5 (E7) arasındaki hücreleri - 5 satır ve 2 sütun - birleştirin
            worksheet.Cells.Merge(3, 4, 5, 2, true);
            
            // Çalışma kitabını kaydedin
            workbook.Save("MergeDemoOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool, bool) {#merge_2}

Belirtilen hücre aralığını tek bir hücrede birleştirir.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool checkConflict, bool mergeConflict)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Bu aralığın ilk satırı (sıfır tabanlı) |
| firstColumn | Int32 | Bu aralığın ilk sütunu (sıfır tabanlı) |
| totalRows | Int32 | Satır sayısı (bir tabanlı) |
| totalColumns | Int32 | Sütun sayısı (bir tabanlı) |
| checkConflict | Boolean | Birleştirilmiş hücrelerin diğer birleştirilmiş hücrelerle kesişip kesişmediğini kontrol edip etmediğini gösterir |
| mergeConflict | Boolean | Birleştirme çakışması birleştirilmiş aralıklar. |

### Açıklamalar

Birleştirilmiş hücreye, aralıktaki sol üst hücrenin adresi üzerinden başvurun. mergeConflict true ise ve birleştirilmiş aralık diğer birleştirilmiş hücrelerle çakışırsa, diğer birleştirilmiş hücreler otomatik olarak kaldırılacaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanBooDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Birleştirilecek hücrelere bazı veriler koyun
            cells[0, 1].PutValue("Merged Cell");
            cells[1, 1].PutValue("This will be merged");

            // Seçenek olmadan hücreleri birleştirin (basit birleştirme)
            cells.Merge(0, 1, 2, 2);
            Console.WriteLine("Cells merged without options");

            // Sonraki birleştirmeyi göstermek için önce birleştirmeyi kaldırın
            cells.UnMerge(0, 1, 2, 2);

            // ignoreStyle=false ve mergeConflict=true ile hücreleri birleştirin
            cells.Merge(0, 1, 2, 2, false, true);
            Console.WriteLine("Cells merged with ignoreStyle=false and mergeConflict=true");

            // Çalışma kitabını kaydedin
            workbook.Save("MergeCellsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


