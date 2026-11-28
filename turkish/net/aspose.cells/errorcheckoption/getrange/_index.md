---
title: "ErrorCheckOption.GetRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ErrorCheckOption yöntemi. Bu ayarın verilen indeksle etkilenen aralığını alır"
type: docs
url: /tr/net/aspose.cells/errorcheckoption/getrange/
---
## ErrorCheckOption.GetRange method

Verilen indeksle bu ayarın etkilediği aralığı alır.

```csharp
public CellArea GetRange(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | aralığın indeksi |

### Dönüş Değeri

verilen indeksteki etkilenen aralığı döndür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionMethodGetRangeWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasının ErrorCheckOptions koleksiyonunu kullanarak bir ErrorCheckOption oluştur
            int errorCheckIndex = worksheet.ErrorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = worksheet.ErrorCheckOptions[errorCheckIndex];

            CellArea area = new CellArea();
            area.StartRow = 1;
            area.StartColumn = 1;
            area.EndRow = 3;
            area.EndColumn = 3;
            int addedIndex = errorCheckOption.AddRange(area);

            try
            {
                int rangeCount = errorCheckOption.GetCountOfRange();
                if (rangeCount > 0)
                {
                    CellArea retrievedArea = errorCheckOption.GetRange(0);
                    Console.WriteLine($"Retrieved range: StartRow={retrievedArea.StartRow}, StartColumn={retrievedArea.StartColumn}, " +
                        $"EndRow={retrievedArea.EndRow}, EndColumn={retrievedArea.EndColumn}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRange method: {ex.Message}");
            }

            workbook.Save("ErrorCheckOptionMethodGetRangeWithInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


