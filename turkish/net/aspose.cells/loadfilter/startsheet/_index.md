---
title: "LoadFilter.StartSheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadFilter yöntemi. Belirtilen çalışma sayfasını yüklemeden önce filtre seçeneklerini hazırlar. Kullanıcıların LoadFilter uygulaması, bu çalışma sayfası için verilerin nasıl yükleneceğini belirtmek amacıyla LoadDataFilterOptions'ı burada değiştirebilir"
type: docs
url: /tr/net/aspose.cells/loadfilter/startsheet/
---
## LoadFilter.StartSheet method

Belirtilen çalışma sayfası yüklenmeden önce filtre seçeneklerini hazırlar. Kullanıcının LoadFilter uygulaması burada LoadDataFilterOptions'ı değiştirerek bu çalışma sayfası için verinin nasıl yükleneceğini belirtebilir.

```csharp
public virtual void StartSheet(Worksheet sheet)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfa | Çalışma Sayfası | Yüklenecek çalışma sayfası. Burada verilen çalışma sayfası nesnesi için yalnızca birkaç özellik kullanılabilir çünkü çoğu veri ve özellik yüklenmemiştir. Kullanılabilir özellikler: Name, Index, VisibilityType |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodStartSheetWithWorksheetDemo
    {
        // LoadFilter'ı genişleten özel bir yükleme filtresi sınıfı oluşturun
        class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                Console.WriteLine($"Processing sheet: {sheet.Name}");
                // Burada belirli sayfaları işlemek için özel mantık ekleyebilirsiniz
            }
        }

        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "TestSheet";

            // Özel yükleme filtremizin bir örneğini oluşturun
            CustomLoadFilter loadFilter = new CustomLoadFilter();

            try
            {
                // Worksheet parametresiyle StartSheet yöntemini çağırın
                loadFilter.StartSheet(worksheet);
                
                Console.WriteLine("StartSheet method executed successfully");
                
                // Sayfanın erişilebilir olduğunu göstermek için bazı veriler ekleyin
                worksheet.Cells["A1"].PutValue("StartSheet Demo");
                worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("LoadFilterStartSheetDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../worksheet/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


