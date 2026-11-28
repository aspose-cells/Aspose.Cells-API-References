---
title: "LightCellsDataProvider.StartCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LightCellsDataProvider yöntemi. Bir hücrenin verilerini kaydetmeye başlar"
type: docs
url: /tr/net/aspose.cells/lightcellsdataprovider/startcell/
---
## LightCellsDataProvider.StartCell method

Bir hücrenin verilerini kaydetmeye başlar.

```csharp
public void StartCell(Cell cell)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cell | Cell | Veri doldurmak için uygulanacak hücre nesnesi. Sütun indeksi, en son [`NextCell`](../nextcell/) çağrısının döndürdüğü değerdir. Hücre iç hücre modeli içinde başlatıldıysa, mevcut hücre nesnesi kullanılacaktır. Aksi takdirde, veri doldurmak için geçici bir Cell nesnesi kullanılacaktır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartCellWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Parametre olarak kullanılacak bir hücre oluştur
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");
            
            // Özel veri sağlayıcı oluştur
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("StartCellWithCellDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with StartCell implementation");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private int rowIndex = -1;
            private int cellIndex = -1;
            private readonly int totalRows = 5;
            private readonly int totalCells = 3;

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < totalRows ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < totalCells ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue($"Row {cell.Row + 1}, Col {cell.Column + 1}");
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

* class [Cell](../../cell/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


