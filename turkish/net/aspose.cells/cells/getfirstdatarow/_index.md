---
title: "Cells.GetFirstDataRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen sütunda veri içeren hücrenin ilk satır indeksini alır"
type: docs
url: /tr/net/aspose.cells/cells/getfirstdatarow/
---
## Cells.GetFirstDataRow method

Belirtilen sütunda veri içeren hücrenin ilk satır indeksini alır.

```csharp
public int GetFirstDataRow(int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |

### Dönüş Değeri

ilk satır indeksi.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetFirstDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Yöntemi göstermek için bazı örnek veriler ekle
            worksheet.Cells["A1"].Value = "Header";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["A3"].Value = "Data2";
            worksheet.Cells["B5"].Value = "Data3";
            worksheet.Cells["C7"].Value = "Data4";

            try
            {
                // Çalışma sayfasından Cells koleksiyonunu al
                Cells cells = worksheet.Cells;

                // Sütun A (indeks 0) için GetFirstDataRow çağır
                int firstDataRowA = cells.GetFirstDataRow(0);
                Console.WriteLine($"First data row in column A: {firstDataRowA}");

                // Sütun B (indeks 1) için GetFirstDataRow çağır
                int firstDataRowB = cells.GetFirstDataRow(1);
                Console.WriteLine($"First data row in column B: {firstDataRowB}");

                // Sütun C (indeks 2) için GetFirstDataRow çağır
                int firstDataRowC = cells.GetFirstDataRow(2);
                Console.WriteLine($"First data row in column C: {firstDataRowC}");

                // Çalışma kitabını kaydedin
                workbook.Save("GetFirstDataRowDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


