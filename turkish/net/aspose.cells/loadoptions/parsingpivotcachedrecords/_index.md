---
title: "LoadOptions.ParsingPivotCachedRecords"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/loadoptions/parsingpivotcachedrecords/
---
## LoadOptions.ParsingPivotCachedRecords property

Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer yanlıştır.

```csharp
public bool ParsingPivotCachedRecords { get; set; }
```

### Açıklamalar

Yalnızca Excel Xlsx, Xltx, Xltm, Xlsm ve xlsb dosyaları için geçerlidir

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingPivotCachedRecordsDemo
    {
        public static void Run()
        {
            // CSV yükleme seçeneklerini oluştur
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
            
            // Pivot önbellek kayıtlarının ayrıştırılmasını etkinleştir
            loadOptions.ParsingPivotCachedRecords = true;
            
            // Çalışma kitabını seçeneklerle yükleyin
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "PivotData";
            
            // Pivot tablo oluştur (özelliğin ayarlandığını göstererek)
            int pivotIndex = worksheet.PivotTables.Add("A1:C10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


