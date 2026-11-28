---
title: "Enum PivotConditionFormatScopeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotConditionFormatScopeType enum. PivotTable koşul biçimlendirme kapsamı türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotconditionformatscopetype/
---
## PivotConditionFormatScopeType enumeration

PivotTable koşul biçimlendirme kapsamı türünü temsil eder.

```csharp
public enum PivotConditionFormatScopeType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Data | `0` | Koşul biçimlendirmenin seçilen veri alanlarına uygulandığını gösterir. |
| Field | `1` | Koşul biçimlendirmenin seçilen PivotTable alan kesişimlerine uygulandığını gösterir. |
| Selection | `2` | Koşul biçimlendirmenin seçilen hücrelere uygulandığını gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotConditionFormatScopeTypeDemo
    {
        public static void PivotConditionFormatScopeTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Çalışma sayfasına bazı veriler ekle
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Bir pivot tablo ekle
            PivotTableCollection pivots = worksheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // PivotFormatCondition ekle
            int formatIndex = pivot.PivotFormatConditions.Add();
            PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
            FormatConditionCollection fcc = pfc.FormatConditions;
            fcc.AddArea(pivot.DataBodyRange);
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;

            // Pivot tablo koşul biçimi için kapsam türünü ayarla
            pfc.ScopeType = PivotConditionFormatScopeType.Data;

            pivot.RefreshData();
            pivot.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotConditionFormatScopeTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


