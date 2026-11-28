---
title: "CalculationCell.Workbook"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationCell özelliği. Workbook nesnesini alır"
type: docs
url: /tr/net/aspose.cells/calculationcell/workbook/
---
## CalculationCell.Workbook property

Workbook nesnesini alır.

```csharp
public Workbook Workbook { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Yapıcı erişime açık olmadığından, yansıma kullanarak CalculationCell örneği oluştur.
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // Workbook özelliği değerini göster
                Console.WriteLine("Workbook Name: " + calcCell.Workbook.FileName);
                Console.WriteLine("Workbook Has Macro: " + calcCell.Workbook.HasMacro);
                Console.WriteLine("Workbook Worksheet Count: " + calcCell.Workbook.Worksheets.Count);

                // Bağlam için ilgili özellikleri göster
                Console.WriteLine("Worksheet Name: " + calcCell.Worksheet.Name);
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);

                // Çalışma kitabını kaydedin
                workbook.Save("WorkbookDemo.xlsx");
                Console.WriteLine("Workbook property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../../workbook/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


