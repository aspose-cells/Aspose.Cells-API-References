---
title: "AbstractFormulaChangeMonitor.OnCellFormulaChanged"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractFormulaChangeMonitor yöntemi. Bir hücredeki formül değiştiğinde tetiklenecek olay"
type: docs
url: /tr/net/aspose.cells/abstractformulachangemonitor/oncellformulachanged/
---
## AbstractFormulaChangeMonitor.OnCellFormulaChanged method

Bir hücredeki formül değiştiğinde tetiklenecek olay.

```csharp
public virtual void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | Int32 | Değişen hücrenin sayfa indeksi |
| rowIndex | Int32 | Değişen hücrenin satır indeksi |
| columnIndex | Int32 | Değişen hücrenin sütun indeksi |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo : AbstractFormulaChangeMonitor
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // AbstractFormulaChangeMonitor'dan miras alan demo sınıfımızın bir örneğini oluştur
            var monitor = new AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo();

            // Değişikliği tetiklemek için bir hücreye formül ayarlayın
            worksheet.Cells["A1"].Formula = "=SUM(B1:B10)";

            try
            {
                // OnCellFormulaChanged'i sayfa indeksi 0, satır 0, sütun 0 (A1) ile çağır
                monitor.OnCellFormulaChanged(0, 0, 0);

                Console.WriteLine("OnCellFormulaChanged called successfully for cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OnCellFormulaChanged method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("OnCellFormulaChangedDemo.xlsx");
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            // Formül değişimini işlemek için uygulama
            Console.WriteLine($"Formula changed in sheet {sheetIndex} at row {rowIndex}, column {columnIndex}");
        }

    }
}
```

### Ayrıca Bakınız

* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


