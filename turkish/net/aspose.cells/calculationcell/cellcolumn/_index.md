---
title: "CalculationCell.CellColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationCell özelliği. Hücrenin sütun indeksini alır"
type: docs
url: /tr/net/aspose.cells/calculationcell/cellcolumn/
---
## CalculationCell.CellColumn property

Hücrenin sütun indeksini alır.

```csharp
public int CellColumn { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationCellPropertyCellColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Biraz veri ve basit bir formül ekle
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Yansıma yoluyla bir CalculationCell örneği elde edin (konstrüktörü public değildir)
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell), 
                    nonPublic: true);

                // CellColumn özelliği değerini oku ve göster
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);

                // İlgili özelliklerin ek gösterimi (isteğe bağlı)
                Console.WriteLine("CellRow value: " + calcCell.CellRow);
                Console.WriteLine("Workbook is null: " + (calcCell.Workbook == null));
                Console.WriteLine("Worksheet is null: " + (calcCell.Worksheet == null));

                // Çalışma kitabını kaydet (dosya eklediğimiz verileri içerecek)
                workbook.Save("CellColumnDemo.xlsx");
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

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


