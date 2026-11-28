---
title: "OoxmlSaveOptions.ExportCellName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OoxmlSaveOptions özelliği. Hücre adının Excel2007 .xlsx .xlsm .xltx .xltm dosyasına aktarılıp aktarılmayacağını gösterir. Çıktı dosyasına SQL Server DTS tarafından erişilebilecekse bu değer true olmalıdır. Değeri false olarak ayarlamak, büyük dosyalar oluşturulurken performansı büyük ölçüde artıracak ve dosya boyutunu azaltacaktır. Varsayılan değer true'tir."
type: docs
url: /tr/net/aspose.cells/ooxmlsaveoptions/exportcellname/
---
## OoxmlSaveOptions.ExportCellName property

Excel2007 .xlsx (.xlsm, .xltx, .xltm) dosyasına hücre adının dışa aktarılıp aktarılmayacağını gösterir. Çıktı dosyasına SQL Server DTS tarafından erişilebilecekse, bu değer true olmalıdır. Değeri false olarak ayarlamak, büyük dosya oluştururken performansı önemli ölçüde artırır ve dosya boyutunu azaltır. Varsayılan değer true'tir.

```csharp
public bool ExportCellName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyExportCellNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere bazı veriler koyun
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            
            // ExportCellName etkinleştirilmiş XLSX kaydetme seçeneklerini oluştur
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.ExportCellName = true;
            
            // Çalışma kitabını hücre adları dışa aktarılmış şekilde kaydet
            workbook.Save("output_with_cellnames.xlsx", saveOptions);
            
            // ExportCellName devre dışı bırakılmış (varsayılan) başka bir kaydetme seçeneği oluştur
            OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
            
            // Çalışma kitabını hücre adları dışa aktarılmadan kaydet
            workbook.Save("output_without_cellnames.xlsx", saveOptions2);
        }
    }
}
```

### Ayrıca Bakınız

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


