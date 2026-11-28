---
title: "LightCellsDataProvider.IsGatherString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LightCellsDataProvider yöntemi. Hücrenin mevcut dize değerinin global bir havuza toplanıp toplanmayacağını kontrol eder"
type: docs
url: /tr/net/aspose.cells/lightcellsdataprovider/isgatherstring/
---
## LightCellsDataProvider.IsGatherString method

Hücrenin mevcut dize değerinin global bir havuza toplanması gerekip gerekmediğini kontrol eder.

```csharp
public bool IsGatherString()
```

### Dönüş Değeri

sonuç dosyası için dize değeri global bir havuza toplanması gerekiyorsa true.

### Açıklamalar

Dize değerlerini toplama, yalnızca bu uygulama tarafından sağlanan hücrelerde çok sayıda yinelenen dize değeri olduğunda avantaj sağlar. Bu durumda dize toplama, çok daha az bellek kullanır ve daha küçük bir sonuç dosyası oluşturur. LightCellsDataProvider tarafından sağlanan hücrelerde çok sayıda dize değeri bulunup, bunların sadece azı aynıysa, dize toplama daha fazla bellek ve zaman tüketir ve sonuç dosyası için hiçbir avantaj sağlamaz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodIsGatherStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("IsGatherStringDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with IsGatherString implementation");
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
            private readonly object[,] data = new object[3, 2]
            {
                { "Product", "Price" },
                { "Laptop", 1200.50 },
                { "Phone", 899.99 }
            };

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < 3 ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < 2 ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue(data[rowIndex, cellIndex]);
            }

            public bool IsGatherString()
            {
                // Yalnızca başlık satırı için dizeleri topla (rowIndex 0)
                return rowIndex == 0;
            }
        }
    }
}
```

### Ayrıca Bakınız

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


