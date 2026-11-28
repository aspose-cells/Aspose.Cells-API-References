---
title: "FormatConditionCollection.AddArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatConditionCollection yöntemi. Koşullu biçimlendirilmiş bir hücre aralığı ekler"
type: docs
url: /tr/net/aspose.cells/formatconditioncollection/addarea/
---
## FormatConditionCollection.AddArea method

Koşullu biçimlendirilmiş bir hücre aralığı ekler.

```csharp
public int AddArea(CellArea cellArea)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | CellArea | Koşullu biçimlendirilmiş hücre aralığı. |

### Dönüş Değeri

Koşullu biçimlendirilmiş hücre aralığının indeksi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue(row * col);
                }
            }

            // Koşullu biçimlendirme ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection formatCollection = worksheet.ConditionalFormattings[index];
            
            // Biçim koşulu oluştur
            formatCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Hücre alanları oluştur ve bunları biçim koleksiyonuna ekle
            CellArea area1 = CellArea.CreateCellArea(0, 0, 4, 4);
            CellArea area2 = CellArea.CreateCellArea(5, 5, 9, 9);
            
            formatCollection.AddArea(area1);
            formatCollection.AddArea(area2);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


