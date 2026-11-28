---
title: "LightCellsDataProvider.StartSheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LightCellsDataProvider yöntemi. Bir çalışma sayfasını kaydetmeye başlar"
type: docs
url: /tr/net/aspose.cells/lightcellsdataprovider/startsheet/
---
## LightCellsDataProvider.StartSheet method

Bir çalışma sayfasını kaydetmeye başlar.

```csharp
public bool StartSheet(int sheetIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | Int32 | Kaydedilecek mevcut sayfanın indeksi. |

### Dönüş Değeri

Verilen sayfa için veri sağlayacaksa true; verilen sayfa normal veri modeli (Cells) kullanmalıysa false.

### Açıklamalar

Bir çalışma kitabı kaydedilirken bir çalışma sayfası kaydedilmesinin başında çağrılacaktır. Sağlayıcının başvurması gerekiyorsa

```csharp
sheetIndex
```

daha sonra startRow(Row) veya startCell(Cell) yönteminde, yani işlem hangi çalışma sayfasının işlendiğini bilmesi gerekiyorsa, uygulama bunu tutmalıdır

```csharp
sheetIndex
```

buradaki değer.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartSheetWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                Workbook workbook = new Workbook();
                workbook.Worksheets.Clear(); // Start with clean worksheet
                
                // Özel veri sağlayıcı oluştur ve hafif hücreler modunda kaydet
                var saveOptions = new OoxmlSaveOptions
                {
                    LightCellsDataProvider = new CustomLightCellsDataProvider()
                };

                Console.WriteLine("Starting workbook save with LightCellsDataProvider...");
                workbook.Save("StartSheetDemoOutput.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully. Check StartSheetDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private bool sheetProcessed = false;

            // Bir çalışma sayfasını işlemeye başlandığında çağrılır
            public bool StartSheet(int sheetIndex)
            {
                Console.WriteLine($"Processing sheet index: {sheetIndex}");
                // Yalnızca ilk sayfayı işle (indeks 0)
                if (sheetIndex == 0)
                {
                    sheetProcessed = true;
                    return true;
                }
                return false;
            }

            public int NextRow()
            {
                if (sheetProcessed)
                {
                    sheetProcessed = false;
                    return 0; // Process first row (index 0)
                }
                return -1; // Stop processing after first row
            }

            public void StartRow(Row row)
            {
                row.Height = 20;
            }

            public int NextCell()
            {
                return 0; // Process first cell (index 0)
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue("Data from LightCellsDataProvider");
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

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


