---
title: "LightCellsDataHandler.StartCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LightCellsDataHandler yöntemi. Bir hücreyi işlemeye hazırlar"
type: docs
url: /tr/net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

Bir hücreyi işlemeye hazırlar.

```csharp
public bool StartCell(int columnIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | Int32 | işlenecek hücrenin sütun indeksi |

### Dönüş Değeri

bu hücrenin işlenip işlenmeyeceği. Hücreyi yok saymak ve bir sonrakine geçmek için false, mevcut satırın hücre verilerinin sonuna ulaşana kadar.

### Açıklamalar

Mevcut satırda mevcut bir hücreye ulaşıldığında çağrılacaktır. Mevcut satır, son [`ProcessRow`](../processrow/) çağrısının satırıdır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodStartCellWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Geçici bir giriş dosyası oluştur
                File.WriteAllText("input.csv", "Column1,Column2,Column3\n1,2,3\n4,5,6");

                // Özel light cells işleyicisiyle yükleme seçenekleri oluştur
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Özel işleyiciyle çalışma kitabını yükle
                Workbook workbook = new Workbook("input.csv", loadOptions);

                // İşlenmiş çalışma kitabını kaydet
                workbook.Save("output.xlsx");
                Console.WriteLine("StartCell method executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartCell method: {ex.Message}");
            }
        }

        private class CustomLightCellsDataHandler : LightCellsDataHandler
        {
            public bool StartSheet(Worksheet sheet)
            {
                return true; // Process all sheets
            }

            public bool StartRow(int rowIndex)
            {
                return true; // Process all rows
            }

            public bool StartCell(int columnIndex)
            {
                // Sadece sütun indeksi 1'deki (ikinci sütun) hücreleri işle
                return columnIndex == 1;
            }

            public bool ProcessCell(Cell cell)
            {
                // İkinci sütundaki hücrelerin değerini iki katına çıkar
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                return true;
            }

            public bool ProcessRow(Row row)
            {
                return true; // Continue processing
            }
        }
    }
}
```

### Ayrıca Bakınız

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


