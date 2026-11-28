---
title: "Sınıf AbstractCalculationMonitor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AbstractCalculationMonitor sınıfı. Kullanıcının formül hesaplamasının ilerlemesini izlemek için bir izleyici."
type: docs
url: /tr/net/aspose.cells/abstractcalculationmonitor/
---
## AbstractCalculationMonitor class

Kullanıcının formül hesaplamasının ilerlemesini izleyebilmesi için izleme sağlar.

```csharp
public abstract class AbstractCalculationMonitor
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CalculatedValue](../../aspose.cells/abstractcalculationmonitor/calculatedvalue/) { get; } | Hücrenin yeni hesaplanan değerini alır. Yalnızca [`AfterCalculate`](./aftercalculate/) içinde kullanılmalıdır. |
| [OriginalValue](../../aspose.cells/abstractcalculationmonitor/originalvalue/) { get; } | Hesaplanan hücrenin eski değerini alır. Yalnızca [`BeforeCalculate`](./beforecalculate/) ve [`AfterCalculate`](./aftercalculate/) içinde kullanılmalıdır. |
| [ValueChanged](../../aspose.cells/abstractcalculationmonitor/valuechanged/) { get; } | Hesaplamadan sonra hücrenin değerinin değişip değişmediğini gösterir. Yalnızca [`AfterCalculate`](./aftercalculate/) içinde kullanılmalıdır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [AfterCalculate](../../aspose.cells/abstractcalculationmonitor/aftercalculate/)(int, int, int) | Bir hücre hesaplandıktan sonra iş mantığını yürütmek için bu yöntemi uygulayın. |
| virtual [BeforeCalculate](../../aspose.cells/abstractcalculationmonitor/beforecalculate/)(int, int, int) | Bir hücre hesaplanmadan önce iş mantığını yürütmek için bu yöntemi uygulayın. |
| virtual [OnCircular](../../aspose.cells/abstractcalculationmonitor/oncircular/)(IEnumerator) | Dairesel referanslarla formüller hesaplanırken bu yöntemi uygulayın. |

### Örnekler

```csharp
using Aspose.Cells;
using System;
using System.Collections;

namespace AsposeCellsExamples
{
    // AbstractCalculationMonitor sınıfının özel uygulaması
    public class CustomCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"Before calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"After calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
            Console.WriteLine($"Original Value: {OriginalValue}, Calculated Value: {CalculatedValue}, Value Changed: {ValueChanged}");
        }

        public override bool OnCircular(IEnumerator circularCellsData)
        {
            Console.WriteLine("Circular reference detected.");
            return false; // Return false to stop calculation when circular reference is detected
        }
    }

    public class CalculationMonitorDemo
    {
        public static void RunDemo()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // CustomCalculationMonitor örneği oluşturun
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();

            // Hesaplama seçeneklerini ayarlayın
            CalculationOptions options = new CalculationOptions
            {
                CalculationMonitor = monitor,
                IgnoreError = false,
                Recursive = true
            };

            // Özel izleyici ile formülleri hesaplayın
            workbook.CalculateFormula(options);

            // Çalışma kitabını kaydedin
            workbook.Save("CalculationMonitorDemo.xlsx");
            workbook.Save("CalculationMonitorDemo.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


