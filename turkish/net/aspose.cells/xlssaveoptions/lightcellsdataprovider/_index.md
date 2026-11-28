---
title: "XlsSaveOptions.LightCellsDataProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XlsSaveOptions özelliği. Çalışma kitabını hafif modda kaydetmek için veri sağlayıcı"
type: docs
url: /tr/net/aspose.cells/xlssaveoptions/lightcellsdataprovider/
---
## XlsSaveOptions.LightCellsDataProvider property

Çalışma kitabını hafif modda kaydetmek için veri sağlayıcı.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // XLS kaydetme seçenekleri oluştur
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            
            // LightCellsDataProvider'ı ayarla
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();
            
            // Çalışma kitabını LightCells modunda kaydet
            workbook.Save("output.xls", saveOptions);
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
            return 0; // Only process first cell for demonstration
        }

        public int NextRow()
        {
            return 0; // Only process first row for demonstration
        }

        public void StartCell(Cell cell)
        {
            // LightCells işleyişini göstermek için uzun bir dize değeri ayarla
            cell.PutValue(new string('X', 257));
        }

        public void StartRow(Row row)
        {
            // Bu demo için özel satır işleme gerek yok
        }

        public bool StartSheet(int sheetIndex)
        {
            // Bu demo için özel sayfa işleme gerek yok
            return false;
        }
    }
}
```

### Ayrıca Bakınız

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


