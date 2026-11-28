---
title: "XlsbSaveOptions.LightCellsDataProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XlsbSaveOptions özelliği. Çalışma kitabını hafif modda kaydetmek için veri sağlayıcı"
type: docs
url: /tr/net/aspose.cells/xlsbsaveoptions/lightcellsdataprovider/
---
## XlsbSaveOptions.LightCellsDataProvider property

Çalışma kitabını hafif modda kaydetmek için veri sağlayıcı.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Biraz örnek veri doldurun
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Data {i}");
            }

            // XLSB kaydetme seçeneklerini oluştur
            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            // Çalışma kitabını LightCellsDataProvider ile kaydet
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Kaydedilen veriyi doğrula
                stream.Seek(0, SeekOrigin.Begin);
                Workbook savedWorkbook = new Workbook(stream);
                Console.WriteLine("Workbook saved successfully with LightCellsDataProvider");
            }
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        public bool IsGatherString()
        {
            return true;
        }

        public int NextCell()
        {
            // Burada hücre yineleme mantığını uygula
            return -1; // Return -1 when no more cells
        }

        public int NextRow()
        {
            // Burada satır yineleme mantığını uygula
            return -1; // Return -1 when no more rows
        }

        public void StartCell(Cell cell)
        {
            // Burada hücre işleme mantığını uygula
        }

        public void StartRow(Row row)
        {
            // Burada satır işleme mantığını uygula
        }

        public bool StartSheet(int sheetIndex)
        {
            // Burada sayfa işleme mantığını uygula
            return true; // Return true to process the sheet
        }
    }
}
```

### Ayrıca Bakınız

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


