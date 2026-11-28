---
title: "Cell.GetFormatConditions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Bu hücreye uygulanan biçim koşullarını alır"
type: docs
url: /tr/net/aspose.cells/cell/getformatconditions/
---
## Cell.GetFormatConditions method

Bu hücreye uygulanan biçim koşullarını al.

```csharp
public FormatConditionCollection[] GetFormatConditions()
```

### Dönüş Değeri

[`FormatConditionCollection`](../../formatconditioncollection/) nesnesini döndürür

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormatConditionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücre koleksiyonunu al
            Cells cells = worksheet.Cells;
            
            // Örnek veri ekleyin.
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            
            // A1 hücresine biçim koşulu ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            
            // A1 hücresi için biçim koşullarını al
            FormatConditionCollection[] conditions = cells["A1"].GetFormatConditions();
            
            // Biçim koşullarının sayısını çıktı olarak ver
            Console.WriteLine("Number of format conditions: " + conditions.Length);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


