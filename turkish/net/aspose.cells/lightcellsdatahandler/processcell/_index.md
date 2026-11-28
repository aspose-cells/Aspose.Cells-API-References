---
title: "LightCellsDataHandler.ProcessCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LightCellsDataHandler yöntemi. Bir hücreyi işlemeye başlar"
type: docs
url: /tr/net/aspose.cells/lightcellsdatahandler/processcell/
---
## LightCellsDataHandler.ProcessCell method

Bir hücreyi işlemeye başlar.

```csharp
public bool ProcessCell(Cell cell)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hücre | Hücre | Şu anda işlenen Hücre nesnesi |

### Dönüş Değeri

bu hücrenin mevcut sayfanın hücre modelinde tutulup tutulmayacağı. Genellikle false olmalıdır, böylece tüm hücreler işlendiğinde bellekte tutulmaz ve bellek tasarrufu sağlanır. Kullanıcının tüm çalışma kitabı işlendikten sonra bazı hücrelere daha sonra erişmesi gibi özel bir amaç için, kullanıcı bu yöntemin true döndürmesini sağlayarak o özel hücreleri Cells modelinde tutabilir ve Cells[row, column] gibi API'lerle daha sonra erişebilir. Ancak, hücre verilerini Cells modelinde tutmak daha fazla bellek gerektirir ve tüm hücreler tutulursa LightCells modunda şablon dosyasını okuma, normal şekilde okuma ile aynı olur.

### Açıklamalar

Bir hücrenin verileri okunduktan sonra çağrılacaktır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodProcessCellWithCellDemo
    {
        public static void Run()
        {
            try
            {
                // Geçici veri dosyası oluştur
                File.WriteAllText("input.txt", "A,B,C\n10,20,30\n40,50,60");

                // Özel light cells işleyicisiyle yükleme seçenekleri oluştur
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Özel işleyiciyle çalışma kitabını yükle
                Workbook workbook = new Workbook("input.txt", loadOptions);

                // İşlenmiş sonuçları kaydet
                workbook.Save("output.xlsx");
                Console.WriteLine("ProcessCell executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ProcessCell: {ex.Message}");
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
                return true; // Process all cells
            }

            public bool ProcessCell(Cell cell)
            {
                // Sayısal değerleri iki katına çıkar ve dizeleri işaretle
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                else if (cell.Type == CellValueType.IsString)
                {
                    cell.PutValue($"TEXT: {cell.StringValue}");
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

* class [Cell](../../cell/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


