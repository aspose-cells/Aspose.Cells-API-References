---
title: "Worksheet.FreezePanes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur"
type: docs
url: /tr/net/aspose.cells/worksheet/freezepanes/
---
## FreezePanes(int, int, int, int) {#freezepanes}

Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| sütun | Int32 | Sütun indeksi. |
| freezedRows | Int32 | Üst bölmede görünen satır sayısı, satır indeksinden fazla olamaz. |
| freezedColumns | Int32 | Sol bölmede görünen sütun sayısı, sütun indeksinden fazla olamaz. |

### Açıklamalar

Satır indeksi ve sütun indeksi sıfır olamaz. Satır sayısı ve sütun sayısı da sıfır olamaz.

İlk iki parametre dondurulmuş konumu belirler ve son iki parametre sol üst bölmede dondurulan alanı belirler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 3. satır, 3. sütunda, 3 dondurulmuş satır ve 3 dondurulmuş sütun ile bölmeleri dondurun
            worksheet.FreezePanes(3, 3, 3, 3);
            
            // Çalışma kitabını kaydedin
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## FreezePanes(string, int, int) {#freezepanes_1}

Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String | Hücre adı. |
| freezedRows | Int32 | Üst bölmede görünen satır sayısı, satır indeksinden fazla olamaz. |
| freezedColumns | Int32 | Sol bölmede görünen sütun sayısı, sütun indeksinden fazla olamaz. |

### Açıklamalar

Satır indeksi ve sütun indeksi sıfır olamaz. Satır sayısı ve sütun sayısı da sıfır olamaz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // "C3" konumunda, 3 dondurulmuş satır ve 3 dondurulmuş sütun ile bölmeleri dondurun
            worksheet.FreezePanes("C3", 3, 3);

            // Çalışma kitabını kaydedin
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


