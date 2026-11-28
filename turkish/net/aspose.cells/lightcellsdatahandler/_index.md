---
title: "Arayüz LightCellsDataHandler"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LightCellsDataHandler arayüzü. Büyük elektronik tablo dosyalarını hafif modda okumak için hücre veri işleyicisini temsil eder."
type: docs
url: /tr/net/aspose.cells/lightcellsdatahandler/
---
## LightCellsDataHandler interface

Hafif modda büyük elektronik tablo dosyalarını okumak için hücre veri işleyicisini temsil eder.

```csharp
public interface LightCellsDataHandler
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ProcessCell](../../aspose.cells/lightcellsdatahandler/processcell/)(Cell) | Bir hücreyi işlemeye başlar. |
| [ProcessRow](../../aspose.cells/lightcellsdatahandler/processrow/)(Row) | Bir satırı işlemeye başlar. |
| [StartCell](../../aspose.cells/lightcellsdatahandler/startcell/)(int) | Bir hücreyi işlemeye hazırlar. |
| [StartRow](../../aspose.cells/lightcellsdatahandler/startrow/)(int) | Bir satırı işlemeye hazırlar. |
| [StartSheet](../../aspose.cells/lightcellsdatahandler/startsheet/)(Worksheet) | Bir çalışma sayfasını işlemeye başlar. |

### Açıklamalar

Bu modda bir çalışma kitabı okunurken, her çalışma sayfası okunurken [`StartSheet`](./startsheet/) kontrol edilir. Bir sayfa için, eğer [`StartSheet`](./startsheet/) true dönerse, bu sayfanın satır/hücre verileri ve özellikleri bu arayüzün uygulaması tarafından kontrol edilir ve işlenir. Her satır için, işlenmesi gerekip gerekmediğini kontrol etmek üzere [`StartRow`](./startrow/) çağrılır. Bir satırın işlenmesi gerekiyorsa, önce bu satırın özellikleri okunur ve kullanıcı bu özelliklere [`ProcessRow`](./processrow/) ile erişebilir. Satırın hücrelerinin de işlenmesi gerekiyorsa, [`ProcessRow`](./processrow/) true döndürmeli ve ardından bu satırdaki mevcut her hücre için işlenip işlenmeyeceğini kontrol etmek üzere [`StartCell`](./startcell/) çağrılır. Bir hücrenin işlenmesi gerekiyorsa, hücreyi bu arayüzün uygulamasıyla işlemek için [`ProcessCell`](./processcell/) çağrılır.  Lütfen dikkat, kullanıcı yalnızca ilgili yöntem tarafından sağlanan mevcut Row/Cell nesnesinin değerleri ve özellikleri üzerinde işlem yapmalıdır. Hücre verileri şablon dosyasından akış biçiminde okunduğu için, diğer nesneler hücre verileri yüklendikten sonra sıfırlanabilir/güncellenebilir. Bu nedenle, bu uygulamada diğer nesneler üzerinde işlem yapmak, çalışma kitabındaki mevcut nesneleri etkileyemeyebilir. Daha da kötüsü, bu işlemler çalışma kitabında tutarsız veri oluşturabilir ve daha sonra beklenmeyen sorunlar veya istisnalar ortaya çıkabilir. Bu yüzden şekiller, sütun genişlikleri, stiller, koşullu biçimlendirmeler gibi diğer tüm nesneler için, lütfen bu uygulamanın hiçbir yönteminde işlem yapmayın. Bunun yerine, çalışma kitabı oluşturulduktan sonra bu nesneleri yönetin.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerDemo : LightCellsDataHandler
    {
        public static void LightCellsDataHandlerExample()
        {
            // LightCellsDataHandler ile bir çalışma kitabı oluşturun ve yükleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // LightCellsDataHandlerDemo örneği oluşturun
            LightCellsDataHandlerDemo handler = new LightCellsDataHandlerDemo();

            // Çalışma kitabı için LightCellsDataHandler'ı ayarlayın
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = handler;

            // Belirtilen yükleme seçenekleriyle çalışma kitabını yükle
            workbook = new Workbook("LargeFile_original.xlsx", loadOptions);

            // İşlemi göstermek için çalışma kitabını kaydedin
            workbook.Save("ProcessedLargeFile.xlsx");
        }

        // StartSheet metodunu uygulayın
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine("Starting to process sheet: " + sheet.Name);
            return true; // Continue processing
        }

        // StartRow metodunu uygulayın
        public bool StartRow(int rowIndex)
        {
            Console.WriteLine("Starting to process row: " + rowIndex);
            return true; // Continue processing
        }

        // ProcessRow metodunu uygulayın
        public bool ProcessRow(Row row)
        {
            Console.WriteLine("Processing row: " + row.Index);
            return true; // Continue processing
        }

        // StartCell metodunu uygulayın
        public bool StartCell(int columnIndex)
        {
            Console.WriteLine("Starting to process cell in column: " + columnIndex);
            return true; // Continue processing
        }

        // ProcessCell metodunu uygulayın
        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine("Processing cell: " + cell.Name + " with value: " + cell.StringValue);
            return true; // Continue processing
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


