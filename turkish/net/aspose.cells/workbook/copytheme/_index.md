---
title: "Workbook.CopyTheme"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Temayı başka bir çalışma kitabından kopyalar"
type: docs
url: /tr/net/aspose.cells/workbook/copytheme/
---
## Workbook.CopyTheme method

Başka bir çalışma kitabından temayı kopyalar.

```csharp
public void CopyTheme(Workbook source)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Çalışma Kitabı | Kaynak çalışma kitabı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyThemeWithWorkbookDemo
    {
        public static void Run()
        {
            // Kaynak çalışma kitabını oluştur (tema, bir şablon dosyası açıldığında otomatik olarak ayarlanır)
            Workbook sourceWorkbook = new Workbook(FileFormatType.Xlsx);

            // Hedef çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            
            // Temayı kaynak çalışma kitabından hedef çalışma kitabına kopyala
            destWorkbook.CopyTheme(sourceWorkbook);

            // Hedef çalışma kitabını kaydet
            destWorkbook.Save("output_with_theme.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


