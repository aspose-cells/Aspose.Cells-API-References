---
title: "LoadFilter.LoadFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadFilter yapıcı. Varsayılan filtre seçenekleri LoadDataFilterOptions.All ile bir LoadFilter oluşturur"
type: docs
url: /tr/net/aspose.cells/loadfilter/loadfilter/
---
## LoadFilter() {#constructor}

Varsayılan filtre seçenekleri LoadDataFilterOptions.All ile bir LoadFilter oluşturur.

```csharp
public LoadFilter()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadFilterMethodCtorDemo
    {
        public static void Run()
        {
            // Varsayılan yapıcı ile yeni bir LoadFilter oluştur
            LoadFilter filter = new LoadFilter();
            
            // Yükleme seçeneklerini oluştur ve filtreyi ata
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = filter;
            
            // Filtre ile çalışma kitabını yükle
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);
            
            // Çalışma sayfalarını sayarak kullanımı gösterin
            Console.WriteLine("Number of worksheets loaded: " + workbook.Worksheets.Count);
            
            // Filtrelenmiş hücre verilerini gösterin (varsayılan olarak tüm hücreler yüklüdür)
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine($"Worksheet '{sheet.Name}' has {sheet.Cells.Count} cells");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadFilter(LoadDataFilterOptions) {#constructor_1}

Verilen filtre seçenekleriyle bir LoadFilter oluşturur.

```csharp
public LoadFilter(LoadDataFilterOptions opts)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| opts | LoadDataFilterOptions | varsayılan filtre seçenekleri |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodCtorWithLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yöntem parametreleri için verileri hazırlayın (LoadDataFilterOptions)
            LoadDataFilterOptions filterOptions = LoadDataFilterOptions.CellData | LoadDataFilterOptions.Chart;

            try
            {
                // #ctor yöntemini belirli parametre türleriyle çağırın
                LoadFilter loadFilter = new LoadFilter(filterOptions);

                // Sonucu işleyin veya görüntüleyin
                Console.WriteLine("LoadFilter created successfully with LoadDataFilterOptions: " + filterOptions);

                // Yöntem çağrısının etkisini gösterin
                Console.WriteLine("LoadDataFilterOptions set to: " + loadFilter.LoadDataFilterOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LoadFilter: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("LoadFilterCtorWithLoadDataFilterOptionsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


