---
title: "LightCellsDataProvider.StartRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LightCellsDataProvider yöntemi. Bir satırın verilerini kaydetmeye başlar"
type: docs
url: /tr/net/aspose.cells/lightcellsdataprovider/startrow/
---
## LightCellsDataProvider.StartRow method

Bir satırın verilerini kaydetmeye başlar.

```csharp
public void StartRow(Row row)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| row | Row | Veri doldurmak için uygulanacak satır nesnesi. Satır indeksi, en son [`NextRow`](../nextrow/) çağrısının döndürdüğü değerdir. Satır iç hücre modeli içinde başlatıldıysa, mevcut satır nesnesi kullanılacaktır. Aksi takdirde, veri doldurmak için geçici bir Row nesnesi kullanılacaktır. |

### Açıklamalar

Bir satır ve hücre verileri kaydedilirken başlangıçta çağrılacaktır. Eğer mevcut satırın yükseklik, stil gibi bazı özel özellikleri varsa, uygulama bu özellikleri burada verilen Row nesnesine ayarlamalıdır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartRowWithRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özel bir veri sağlayıcı oluşturun
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                // Çalışma kitabını özel veri sağlayıcımızla işleyin
                workbook.Save("StartRowDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook processed successfully with StartRow implementation.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartRow method: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private int currentRow = -1;
            private readonly int totalRows = 5;

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                currentRow++;
                return currentRow < totalRows ? currentRow : -1;
            }

            public void StartRow(Row row)
            {
                // StartRow yöntemini Row parametresiyle gösterin
                row.Height = 25;
                row.IsHidden = (currentRow % 2 == 0);
                Console.WriteLine($"Processing row {row.Index}, Height: {row.Height}, Hidden: {row.IsHidden}");
            }

            public int NextCell()
            {
                return 0; // Process only first cell in each row
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue($"Row {cell.Row + 1} Data");
            }

            public bool IsGatherString()
            {
                return false;
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../../row/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


