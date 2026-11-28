---
title: "HtmlSaveOptions.ExportArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Mevcut aktif Çalışma Sayfasının dışa aktarılan CellArea'ını alır veya ayarlar. Bu niteliği ayarlarsanız, mevcut aktif Çalışma Sayfasının yazdırma alanı atlanır. Dosya HTML olarak kaydedildiğinde yalnızca belirtilen alan dışa aktarılır."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportarea/
---
## HtmlSaveOptions.ExportArea property

Mevcut aktif Çalışma Sayfasının dışa aktarılacak CellArea'ını alır veya ayarlar. Bu özniteliği ayarlarsanız, mevcut aktif Çalışma Sayfasının yazdırma alanı atlanır. Dosya HTML'ye kaydedilirken yalnızca belirtilen alan dışa aktarılır.

```csharp
public CellArea ExportArea { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekleyin
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Dışa aktarma alanı ile HTML kaydetme seçeneklerini ayarlayın
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportArea = CellArea.CreateCellArea("B2", "D5");

            // Çalışma kitabını belirtilen dışa aktarma alanı ile kaydet
            workbook.Save("output.html", options);
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


