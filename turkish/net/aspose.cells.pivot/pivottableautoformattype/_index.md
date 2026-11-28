---
title: "Enum PivotTableAutoFormatType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotTableAutoFormatType enum. PivotTable otomatik biçim türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivottableautoformattype/
---
## PivotTableAutoFormatType enumeration

PivotTable otomatik biçim türünü temsil eder.

```csharp
public enum PivotTableAutoFormatType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Hiçbiri biçim türünü temsil eder. |
| Classic | `1` | Klasik otomatik biçim türünü temsil eder. |
| Report1 | `2` | Report1 biçim türünü temsil eder. |
| Report2 | `3` | Report2 biçim türünü temsil eder. |
| Report3 | `4` | Report3 biçim türünü temsil eder. |
| Report4 | `5` | Report4 biçim türünü temsil eder. |
| Report5 | `6` | Report5 biçim türünü temsil eder. |
| Report6 | `7` | Report6 biçim türünü temsil eder. |
| Report7 | `8` | Report7 biçim türünü temsil eder. |
| Report8 | `9` | Report8 biçim türünü temsil eder. |
| Report9 | `10` | Report9 biçim türünü temsil eder. |
| Report10 | `11` | Report10 biçim türünü temsil eder. |
| Table1 | `12` | Table1 biçim türünü temsil eder. |
| Table2 | `13` | Table2 biçim türünü temsil eder. |
| Table3 | `14` | Table3 biçim türünü temsil eder. |
| Table4 | `15` | Table4 biçim türünü temsil eder. |
| Table5 | `16` | Table5 biçim türünü temsil eder. |
| Table6 | `17` | Table6 biçim türünü temsil eder. |
| Table7 | `18` | Table7 biçim türünü temsil eder. |
| Table8 | `19` | Table8 biçim türünü temsil eder. |
| Table9 | `20` | Table9 biçim türünü temsil eder. |
| Table10 | `21` | Table10 biçim türünü temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableAutoFormatTypeDemo
    {
        public static void PivotTableAutoFormatTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PivotTable için bazı örnek veriler ekleyin
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Çalışma sayfasına bir PivotTable ekle
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // PivotTable'a alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // PivotTable için otomatik biçim türünü ayarlayın
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report1;

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableAutoFormatTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


