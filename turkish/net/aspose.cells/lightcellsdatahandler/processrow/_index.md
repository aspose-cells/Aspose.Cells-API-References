---
title: "LightCellsDataHandler.ProcessRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LightCellsDataHandler yöntemi. Bir satırı işlemeye başlar"
type: docs
url: /tr/net/aspose.cells/lightcellsdatahandler/processrow/
---
## LightCellsDataHandler.ProcessRow method

Bir satırı işlemeye başlar.

```csharp
public bool ProcessRow(Row row)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Row | Şu anda işlenen satır nesnesi. |

### Dönüş Değeri

Bu satırın hücrelerinin işlenip işlenmeyeceği. false ise bu satırdaki tüm hücreler yok sayılır.

### Açıklamalar

Satırın yüksekliği, stili vb. özellikleri okunduktan sonra çağrılır. Ancak, bu satırdaki hücreler henüz okunmamıştır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodProcessRowWithRowDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Örnek veri ekleyin.
                worksheet.Cells["A1"].Value = "Test Data";
                worksheet.Cells["A2"].Value = 100;
                worksheet.Cells["B2"].Value = 200;

                // Özel işleyici oluştur
                var handler = new CustomRowHandler();

                // İlk satırı işle
                Row firstRow = worksheet.Cells.Rows[0];
                bool result = handler.ProcessRow(firstRow);

                Console.WriteLine($"ProcessRow returned: {result}");
                Console.WriteLine($"Row height after processing: {firstRow.Height}");

                workbook.Save("ProcessRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ProcessRow demo: {ex.Message}");
            }
        }

        private class CustomRowHandler : LightCellsDataHandler
        {
            public bool ProcessRow(Row row)
            {
                // Satır özelliklerine erişimi göster
                Console.WriteLine($"Processing row index: {row.Index}");
                Console.WriteLine($"Row is hidden: {row.IsHidden}");
                Console.WriteLine($"Row is blank: {row.IsBlank}");

                // Başlık satırı değilse satır yüksekliğini değiştir
                if (row.Index > 0)
                {
                    row.Height = 25.0;
                }

                return true;
            }

            public bool StartSheet(Worksheet sheet) => true;
            public bool StartRow(int rowIndex) => true;
            public bool StartCell(int columnIndex) => true;
            public bool ProcessCell(Cell cell) => true;
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../../row/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


