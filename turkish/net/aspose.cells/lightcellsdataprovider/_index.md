---
title: "Arayüz LightCellsDataProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LightCellsDataProvider arayüzü. Büyük elektronik tablo dosyalarını hafif modda kaydetmek için veri sağlayıcıyı temsil eder."
type: docs
url: /tr/net/aspose.cells/lightcellsdataprovider/
---
## LightCellsDataProvider interface

Hafif modda büyük elektronik tablo dosyalarını kaydetmek için Veri sağlayıcısını temsil eder.

```csharp
public interface LightCellsDataProvider
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [IsGatherString](../../aspose.cells/lightcellsdataprovider/isgatherstring/)() | Hücrenin mevcut dize değerinin global bir havuza toplanması gerekip gerekmediğini kontrol eder. |
| [NextCell](../../aspose.cells/lightcellsdataprovider/nextcell/)() | Kaydedilecek bir sonraki hücreyi al. |
| [NextRow](../../aspose.cells/lightcellsdataprovider/nextrow/)() | Kaydedilecek bir sonraki satırı al. |
| [StartCell](../../aspose.cells/lightcellsdataprovider/startcell/)(Cell) | Bir hücrenin verilerini kaydetmeye başlar. |
| [StartRow](../../aspose.cells/lightcellsdataprovider/startrow/)(Row) | Bir satırın verilerini kaydetmeye başlar. |
| [StartSheet](../../aspose.cells/lightcellsdataprovider/startsheet/)(int) | Bir çalışma sayfasını kaydetmeye başlar. |

### Açıklamalar

Bu modla bir çalışma kitabı kaydedilirken, [`StartSheet`](./startsheet/) her çalışma sayfası kaydedildiğinde kontrol edilecektir. Tek bir sayfa için, [`StartSheet`](./startsheet/) true dönerse, bu sayfanın satırları/hücreleri için kaydedilecek tüm veri ve özellikler bu arayüzün uygulanması tarafından sağlanacaktır. İlk olarak, kaydedilecek bir sonraki satır indeksini almak için [`NextRow`](./nextrow/) çağrılacaktır. Geçerli bir satır indeksi döndürülürse (satır indeksi kaydedilecek satırlar için artan sırada olmalıdır), bu satırı temsil eden bir Row nesnesi, özelliklerini ayarlamak için [`StartRow`](./startrow/) tarafından sağlanacaktır. Tek bir satır için, önce [`NextCell`](./nextcell/) kontrol edilecektir. Geçerli bir sütun indeksi döndürülürse (sütun indeksi mevcut satırdaki tüm hücreler için artan sırada olmalıdır), bu hücreyi temsil eden bir Cell nesnesi, verisini ve özelliklerini ayarlamak için [`StartCell`](./startcell/) tarafından sağlanacaktır. [`StartCell`](./startcell/) sonrası hücre doğrudan sonuç elektronik tablo dosyasına kaydedilecektir. Ardından bir sonraki hücre kontrol edilip işlenecektir. Lütfen, kullanıcının yalnızca ilgili metodun sağladığı mevcut Row/Cell nesnesinin değerlerini ve özelliklerini güncellemesi gerektiğini unutmayın. Hücre verileri akış biçiminde sonuç dosyasına yazıldığı için, diğer nesnelerin çoğu zaten sonuç dosyasına yazılmış ya da onlar için bazı global veriler toplanıp yazılmış olabilir. Bu nedenle, kullanıcı hücre verileri kaydedilirken diğer nesneleri güncellerse, bu işlemler kaydedilen verileri etkileyemeyebilir. Daha da kötüsü, bu işlemler tutarsız verilerin sonuç dosyasına kaydedilmesine ve dosyanın bozulmasına yol açabilir. Bu yüzden, şekiller, sütun genişlikleri ve stiller, koşullu biçimlendirmeler gibi diğer tüm nesneler için, bu uygulamanın hiçbir metodunda onlarla işlem yapmayınız. Bunun yerine, bunları yönetip, Workbook'un "Save" metodunu çağırmadan önce son duruma getirin.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderDemo
    {
        public static void LightCellsDataProviderExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özel bir LightCellsDataProvider oluşturun
            CustomLightCellsDataProvider dataProvider = new CustomLightCellsDataProvider();

            // Çalışma kitabını kaydetmek için LightCellsDataProvider'ı ayarlayın
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx)
            {
                LightCellsDataProvider = dataProvider
            };

            // Çalışma kitabını özel LightCellsDataProvider ile kaydedin
            workbook.Save("LightCellsDataProviderExample.xlsx", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;

        public bool StartSheet(int sheetIndex)
        {
            // İlk sayfanın işlenmesine başlayın
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            // Bir sonraki satıra geçin
            currentRow++;
            currentCell = -1;

            // Mevcut satır indeksini döndürün veya daha fazla satır yoksa -1 döndürün
            return currentRow < 10 ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // Gerekirse satırı başlatın
        }

        public int NextCell()
        {
            // Bir sonraki hücreye geçin
            currentCell++;

            // Mevcut hücre indeksini döndürün veya daha fazla hücre yoksa -1 döndürün
            return currentCell < 10 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            // Hücrenin değerini ayarlayın
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            // Dizgelerin küresel bir havuza toplanıp toplanmayacağını döndürün
            return false;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


