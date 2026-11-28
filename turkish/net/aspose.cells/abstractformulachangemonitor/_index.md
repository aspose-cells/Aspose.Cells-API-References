---
title: "AbstractFormulaChangeMonitor sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AbstractFormulaChangeMonitor sınıfı. Kullanıcının belirli işlemler sırasında formül değişikliklerini izleyebilmesi için bir izleyici"
type: docs
url: /tr/net/aspose.cells/abstractformulachangemonitor/
---
## AbstractFormulaChangeMonitor class

Kullanıcının belirli işlemler sırasında formüllerdeki değişiklikleri izleyebilmesi için izleme sağlar.

```csharp
public abstract class AbstractFormulaChangeMonitor
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [OnCellFormulaChanged](../../aspose.cells/abstractformulachangemonitor/oncellformulachanged/)(int, int, int) | Bir hücredeki formül değiştiğinde tetiklenecek olay. |
| virtual [OnFormatConditionFormulaChanged](../../aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/)(FormatCondition) | FormatCondition formülü değiştiğinde tetiklenecek olay. |

### Açıklamalar

Örneğin, hücre aralığını silme/ekleme sırasında, referansların kayması nedeniyle diğer hücrelerin formülleri değişebilir. Lütfen dikkat edin, izleyicideki yöntemler formülü içeren bir nesne için birden fazla kez çağrılabilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassAbstractFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Hücrelerde bazı formüller ayarla
            worksheet.Cells["A1"].Formula = "=B1+C1";
            worksheet.Cells["B1"].Formula = "=D1*2";
            worksheet.Cells["C1"].Value = 5;
            worksheet.Cells["D1"].Value = 10;

            InsertOptions options = new InsertOptions();
            options.FormulaChangeMonitor = new MyFormulaChangeMonitor(wb.Worksheets);
            
            // Formül değişikliklerini tetikleyecek satırlar ekle
            worksheet.Cells.InsertRows(0, 2, options);
        }
    }

    public class MyFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        private readonly WorksheetCollection mWorksheets;
        
        public MyFormulaChangeMonitor(WorksheetCollection worksheets)
        {
            mWorksheets = worksheets;
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"Formula changed in {mWorksheets[sheetIndex].Name}!{CellsHelper.CellIndexToName(rowIndex, columnIndex)}");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


