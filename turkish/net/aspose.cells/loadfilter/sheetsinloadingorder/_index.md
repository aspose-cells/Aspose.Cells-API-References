---
title: "LoadFilter.SheetsInLoadingOrder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadFilter özelliği. Yüklenmesi gereken sayfa indekslerini ve sırasını belirtir. Varsayılan değer null olup, şablon dosyasındaki tüm sayfaları varsayılan sırada yükleyeceği anlamına gelir. Null değilse ve bazı sayfa indeksleri döndürülen dizide bulunmuyorsa, sayfa yüklenmez"
type: docs
url: /tr/net/aspose.cells/loadfilter/sheetsinloadingorder/
---
## LoadFilter.SheetsInLoadingOrder property

Yüklenmesi gereken sayfaları (indekslerini) ve sıralamayı belirtir. Varsayılan değer null'dır ve bu, şablon dosyasındaki tüm sayfaların varsayılan sırayla yüklenmesini ifade eder. Null değilse ve bazı sayfa indeksleri döndürülen dizide yoksa, o sayfa yüklenmez.

```csharp
public virtual int[] SheetsInLoadingOrder { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertySheetsInLoadingOrderDemo
    {
        public static void Run()
        {
            // Birden çok sayfa içeren yeni bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Özel bir yükleme filtresi oluştur
            LoadFilter loadFilter = new LoadFilter(LoadDataFilterOptions.All);
            
            // Varsayılan SheetsInLoadingOrder'ı göster (null tüm sayfaları yüklemek anlamına gelir)
            Console.WriteLine("Initial SheetsInLoadingOrder is null: " + (loadFilter.SheetsInLoadingOrder == null));
            
            // Özel sayfa sırası ile yüklemeyi göstermek için bir şablon dosyası oluştur
            workbook.Save("Template.xlsx");
            
            // Özel filtrimizle yükleme seçenekleri oluştur
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = loadFilter;
            
            // Çalışma kitabını varsayılan ayarlarla yükle (tüm sayfalar)
            Workbook loadedWorkbook1 = new Workbook("Template.xlsx", loadOptions);
            Console.WriteLine("Sheets loaded with default filter: " + loadedWorkbook1.Worksheets.Count);
            
            // Belirli bir sayfa yükleme sırası ile yeni bir filtre oluştur
            LoadFilter orderedFilter = new LoadFilter(LoadDataFilterOptions.All)
            {
                // Not: SheetsInLoadingOrder yalnızca okunabilir, bu yüzden yeni bir filtre oluşturmamız gerekiyor
                // isteğe bağlı sıralamayı yapıcıda ya da başka yollarla
                // Bu, özelliğin yalnızca okunabilir olmasının sınırlamasını gösterir
            };
            
            // SheetsInLoadingOrder yalnızca okunabilir olduğundan, LoadFilter'ı alt sınıfa almamız gerekecek
            // özel sayfa yükleme sırasını göstermek için
            CustomLoadFilter customFilter = new CustomLoadFilter(new int[] { 2, 0 }); // Load Sheet3 first, then Sheet1
            
            LoadOptions customLoadOptions = new LoadOptions();
            customLoadOptions.LoadFilter = customFilter;
            
            // Çalışma kitabını özel sayfa sırası ile yükle
            Workbook loadedWorkbook2 = new Workbook("Template.xlsx", customLoadOptions);
            Console.WriteLine("Sheets loaded with custom filter: " + loadedWorkbook2.Worksheets.Count);
            Console.WriteLine("First sheet in custom order: " + loadedWorkbook2.Worksheets[0].Name);
        }
    }

    // SheetsInLoadingOrder işlevselliğini göstermek için özel LoadFilter uygulaması
    public class CustomLoadFilter : LoadFilter
    {
        private readonly int[] _sheetsOrder;
        
        public CustomLoadFilter(int[] sheetsOrder) : base(LoadDataFilterOptions.All)
        {
            _sheetsOrder = sheetsOrder;
        }
        
        public override int[] SheetsInLoadingOrder => _sheetsOrder;
    }
}
```

### Ayrıca Bakınız

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


