---
title: "Enum CellValueType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellValueType enum. Bir hücre değer tipini belirtir"
type: docs
url: /tr/net/aspose.cells/cellvaluetype/
---
## CellValueType enumeration

Bir hücre değeri türünü belirtir.

```csharp
public enum CellValueType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| IsUnknown | `0` | Hücre değer tipi bilinmiyor. |
| IsNull | `1` | Boş hücre. İlgili değer null olmalıdır. |
| IsNumeric | `2` | Hücre değeri sayısaldır. İlgili değer int veya double olmalıdır. |
| IsDateTime | `4` | Hücre değeri tarih/zaman tipindedir. İlgili değer DateTime olmalıdır. |
| IsString | `8` | Hücre değeri string'tir. İlgili değer string olmalıdır. |
| IsBool | `16` | Hücre değeri boolean'dır. İlgili değer bool olmalıdır. |
| IsError | `32` | Hücre hata değeri içerir. İlgili değer hata string'i olmalıdır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueTypeDemo
    {
        public static void CellValueTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue(123); // Numeric value
            worksheet.Cells["A2"].PutValue("Hello World"); // String value
            worksheet.Cells["A3"].PutValue(DateTime.Now); // DateTime value
            worksheet.Cells["A4"].PutValue(true); // Boolean value
            worksheet.Cells["A5"].PutValue(null); // Null value

            // Hücrelerin değer tiplerini kontrol edin ve görüntüleyin
            DisplayCellValueType(worksheet.Cells["A1"]);
            DisplayCellValueType(worksheet.Cells["A2"]);
            DisplayCellValueType(worksheet.Cells["A3"]);
            DisplayCellValueType(worksheet.Cells["A4"]);
            DisplayCellValueType(worksheet.Cells["A5"]);

            // Çalışma kitabını kaydedin
            workbook.Save("CellValueTypeExample.xlsx");
            workbook.Save("CellValueTypeExample.pdf");
        }

        private static void DisplayCellValueType(Cell cell)
        {
            Console.WriteLine($"Cell {cell.Name} has value: {cell.Value} and type: {cell.Type}");

            switch (cell.Type)
            {
                case CellValueType.IsNumeric:
                    Console.WriteLine("The cell contains a numeric value.");
                    break;
                case CellValueType.IsString:
                    Console.WriteLine("The cell contains a string value.");
                    break;
                case CellValueType.IsDateTime:
                    Console.WriteLine("The cell contains a DateTime value.");
                    break;
                case CellValueType.IsBool:
                    Console.WriteLine("The cell contains a boolean value.");
                    break;
                case CellValueType.IsNull:
                    Console.WriteLine("The cell is blank.");
                    break;
                case CellValueType.IsError:
                    Console.WriteLine("The cell contains an error value.");
                    break;
                default:
                    Console.WriteLine("The cell value type is unknown.");
                    break;
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


