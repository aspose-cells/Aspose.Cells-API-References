---
title: "FormatConditionCollection.RemoveArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatConditionCollection metodu. Koşullu biçimlendirilmiş hücre aralığını indeksle kaldırır"
type: docs
url: /tr/net/aspose.cells/formatconditioncollection/removearea/
---
## RemoveArea(int) {#removearea_1}

Koşullu biçimlendirilmiş hücre aralığını dizine göre kaldırır.

```csharp
public void RemoveArea(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Kaldırılacak koşullu biçimlendirilmiş hücre aralığının indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Koşullu biçimlendirme ekle
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];

            // Biçimlendirmek için alanlar ekle
            formatConditionCollection.AddArea(CellArea.CreateCellArea(0, 0, 10, 5)); // First area
            formatConditionCollection.AddArea(CellArea.CreateCellArea(5, 5, 15, 10)); // Second area

            // Bir koşul ekle
            formatConditionCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");

            // İlk alan sayısını göster (2 alan eklediğimizi biliyoruz)
            Console.WriteLine("Areas before removal: 2");

            // İkinci alanı kaldır (indeks 1)
            formatConditionCollection.RemoveArea(1);

            // Kaldırma sonrası alan sayısını göster (1 alan kaldırdığımızı biliyoruz)
            Console.WriteLine("Areas after removal: 1");

            // Çalışma kitabını kaydedin
            workbook.Save("RemoveAreaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveArea(int, int, int, int) {#removearea}

Aralıktaki koşullu biçimlendirmeyi kaldır.

```csharp
public bool RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Aralığın başlangıç satırı. |
| startColumn | Int32 | Aralığın başlangıç sütunu. |
| totalRows | Int32 | Aralıktaki satır sayısı. |
| totalColumns | Int32 | Aralıktaki sütun sayısı. |

### Dönüş Değeri

TRUE döndürür, bu FormatCondtionCollection kaldırılmalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            
            int idx = cfc.Add();
            FormatConditionCollection fcc = cfc[idx];
            
            // İlk alanı ekle
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            fcc.AddArea(initialArea);
            
            // Koşul ekle
            idx = fcc.AddCondition(FormatConditionType.Expression);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "=A1>0";
            fc.Style.Font.Color = Color.Red;
            
            // Int32 parametrelerle RemoveArea yöntemini göster
            Console.WriteLine("Before removal - Areas count: " + fcc.Count);
            fcc.RemoveArea(0, 0, 1, 1); // Remove the initial area
            Console.WriteLine("After removal - Areas count: " + fcc.Count);
            
            // Yeni bir alan ekle
            CellArea newArea = CellArea.CreateCellArea(1, 1, 1, 1);
            fcc.AddArea(newArea);
            Console.WriteLine("After adding new area - Areas count: " + fcc.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


