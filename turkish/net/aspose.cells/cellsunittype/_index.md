---
title: "Enum CellsUnitType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellsUnitType enum. Ölçüm birimini belirtir"
type: docs
url: /tr/net/aspose.cells/cellsunittype/
---
## CellsUnitType enumeration

Ölçüm birimini belirtir.

```csharp
public enum CellsUnitType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Pixel | `1` | Ölçüm piksellerde. |
| Point | `2` | Ölçüm puanlarda. Bir puan, bir inçin 1/72'sine eşittir. |
| Inch | `4` | Ölçüm inçlerde. |
| Cm | `6` | Ölçüm santimetrelerde. |
| Character | `7` | Karakter biriminde. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Farklı CellsUnitType enum değerlerini kullanmayı gösterin
                Console.WriteLine("Available CellsUnitType values:");

                // Tüm enum değerlerini göster
                Console.WriteLine("Pixel: " + CellsUnitType.Pixel);
                Console.WriteLine("Point: " + CellsUnitType.Point);
                Console.WriteLine("Inch: " + CellsUnitType.Inch);
                Console.WriteLine("Cm: " + CellsUnitType.Cm);
                Console.WriteLine("Character: " + CellsUnitType.Character);

                // Örnek kullanım: Farklı birimler kullanarak sütun genişliğini ayarlayın
                worksheet.Cells.SetColumnWidthPixel(0, 100); // Using Pixel unit
                worksheet.Cells.SetColumnWidthInch(1, 2.0);  // Using Inch unit

                // Tam bir akışı göstermek için çalışma kitabını kaydedin
                workbook.Save("CellsUnitTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with different unit types applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CellsUnitType: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


