---
title: "Workbook.Copy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Başka bir Workbook nesnesini kopyalar"
type: docs
url: /tr/net/aspose.cells/workbook/copy/
---
## Copy(Workbook, CopyOptions) {#copy_1}

Başka bir Workbook nesnesini kopyalar.

```csharp
public void Copy(Workbook source, CopyOptions copyOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Çalışma Kitabı | Kaynak Workbook nesnesi. |
| copyOptions | CopyOptions | Diğer workbook'u kopyalama seçenekleri. |

### Açıklamalar

Bir Excel dosyasını klonlamak çok basittir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookCopyOptionsDemo
    {
        public static void Run()
        {
            // Makrolu kaynak workbook
            Workbook sourceWorkbook = new Workbook("source_with_macros.xlsm");
            
            // Hedef workbook (boş veya mevcut)
            Workbook destWorkbook = new Workbook();
            
            // Makroları korumak için kopyalama seçeneklerini yapılandır
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;
            
            // İçeriği kaynak workbook'tan hedef workbook'a kopyala
            sourceWorkbook.Copy(destWorkbook, options);
            
            // Sonucu kaydet
            destWorkbook.Save("output_with_macros.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../../copyoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Workbook) {#copy}

Kaynak bir Workbook nesnesinden verileri kopyalar.

```csharp
public void Copy(Workbook source)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Çalışma Kitabı | Kaynak Workbook nesnesi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookDemo
    {
        public static void Run()
        {
            // Kaynak ve çıktı dosya yolları
            string sourceFile = "source.xlsx";
            string outputFile = "output.xlsx";

            // Kaynak çalışma kitabını yükle
            Workbook sourceWorkbook = new Workbook(sourceFile);

            // Yeni bir çalışma kitabı oluşturun ve kaynaktan içeriği kopyalayın
            Workbook destinationWorkbook = new Workbook();
            destinationWorkbook.Copy(sourceWorkbook);

            // Kopyalanan çalışma kitabını kaydedin
            destinationWorkbook.Save(outputFile);
            
            Console.WriteLine("Workbook copied successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


