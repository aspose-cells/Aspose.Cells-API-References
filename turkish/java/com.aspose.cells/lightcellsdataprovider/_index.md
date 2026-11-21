---
title: "LightCellsDataProvider"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hafif modda büyük elektronik tablo dosyalarını kaydetmek için Veri sağlayıcısını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/lightcellsdataprovider/
---
```
public interface LightCellsDataProvider
```

Hafif modda büyük elektronik tablo dosyalarını kaydetmek için Veri sağlayıcısını temsil eder.

**Remarks**

Bu modla bir çalışma kitabı kaydedilirken, [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\\#startSheet-int-) çalışma kitabındaki her çalışma sayfası kaydedilirken kontrol edilecektir. Bir sayfa için, eğer [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\\#startSheet-int-) true dönerse, bu sayfanın satırları/hücreleri için kaydedilecek tüm veri ve özellikler bu arayüzün uygulaması tarafından sağlanacaktır. İlk olarak, kaydedilecek bir sonraki satır indeksini almak için [nextRow()](../../com.aspose.cells/lightcellsdataprovider\\#nextRow--) çağrılacaktır. Eğer geçerli bir satır indeksi döndürülürse (satır indeksleri kaydedilecek satırlar için artan sırada olmalıdır), bu satırı temsil eden bir Row nesnesi [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\\#startRow-Row-) tarafından sağlanacak ve uygulama bu nesnenin özelliklerini ayarlayacaktır. Bir satır için, önce [nextCell()](../../com.aspose.cells/lightcellsdataprovider\\#nextCell--) kontrol edilecektir. Eğer geçerli bir sütun indeksi döndürülürse (sütun indeksleri mevcut satırdaki tüm hücreler için artan sırada olmalıdır), bu hücreyi temsil eden bir Cell nesnesi [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\\#startCell-Cell-) tarafından sağlanacak ve uygulama bu nesnenin veri ve özelliklerini ayarlayacaktır. [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\\#startCell-Cell-) işleminden sonra hücre doğrudan sonuç elektronik tablo dosyasına kaydedilecektir. Ardından bir sonraki hücre kontrol edilecek ve işlenecektir.

Lütfen unutmayın, kullanıcı yalnızca ilgili yöntem tarafından sağlanan mevcut Row/Cell nesnesinin değerlerini ve özelliklerini güncellemelidir. Hücre verileri, sonuç dosyasına akış biçiminde yazıldığı için, diğer nesnelerin çoğu zaten sonuç dosyasına yazılmış olabilir veya onlar için bazı global veriler toplanıp yazılmış olabilir. Bu nedenle, kullanıcı hücre verilerini kaydederken diğer nesneleri güncellerse, bu işlemler kaydedilen verileri etkileyemeyebilir. Daha da kötüsü, bu işlemler tutarsız verilerin sonuç dosyasına kaydedilmesine ve dosyanın bozulmasına neden olabilir. Bu yüzden, şekiller, sütun genişliği ve stiller, koşullu biçimlendirmeler gibi diğer tüm nesnelerle bu uygulamanın hiçbir yönteminde işlem yapmayın. Bunun yerine, bunları yönetin ve Workbook'un "Save" yöntemini çağırmadan önce son duruma ayarlayın.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [isGatherString()](#isGatherString--) | Hücrenin mevcut string değerinin global bir havuza toplanıp toplanmayacağını kontrol eder. |
| [nextCell()](#nextCell--) | Kaydedilecek bir sonraki hücreyi alır. |
| [nextRow()](#nextRow--) | Kaydedilecek bir sonraki satırı alır. |
| [startCell(Cell cell)](#startCell-com.aspose.cells.Cell-) | Bir hücrenin verilerini kaydetmeye başlar. |
| [startRow(Row row)](#startRow-com.aspose.cells.Row-) | Bir satırın verilerini kaydetmeye başlar. |
| [startSheet(int sheetIndex)](#startSheet-int-) | Bir çalışma sayfasını kaydetmeye başlar. |
### isGatherString() {#isGatherString--}
```
public abstract boolean isGatherString()
```


Hücrenin mevcut string değerinin global bir havuza toplanıp toplanmayacağını kontrol eder.

**Remarks**

String değerlerini toplama, yalnızca bu uygulama tarafından sağlanan hücrelerde çok sayıda yinelenen string değeri olduğunda avantaj sağlar. Bu durumda string toplama, çok daha az bellek kullanır ve daha küçük bir sonuç dosyası üretir. Ancak LightCellsDataProvider tarafından sağlanan hücrelerde çok sayıda string değeri bulunup bunların yalnızca az bir kısmı aynıysa, string toplama daha fazla bellek ve zaman tüketir ve sonuç dosyası için hiçbir avantaj sağlamaz.

**Returns:**
boolean - sonuç dosyası için string değerin global bir havuza toplanması gerekiyorsa true.
### nextCell() {#nextCell--}
```
public abstract int nextCell()
```


Kaydedilecek bir sonraki hücreyi alır.

**Remarks**

Bir hücreyi kaydetmeye başlarken çağrılır.

**Returns:**
int - kaydedilecek bir sonraki hücrenin sütun indeksi. -1, mevcut satır verilerinin sonuna gelindiği ve mevcut satırda daha fazla hücre kaydedilmeyeceği anlamına gelir.
### nextRow() {#nextRow--}
```
public abstract int nextRow()
```


Kaydedilecek bir sonraki satırı alır.

**Remarks**

Bir satırı ve hücre verilerini kaydetmeye başlarken (öncesinde [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-)) çağrılır.

**Returns:**
int - kaydedilecek bir sonraki satır indeksi. -1, mevcut sayfa verilerinin sonuna gelindiği ve mevcut sayfada daha fazla satır kaydedilmeyeceği anlamına gelir.
### startCell(Cell cell) {#startCell-com.aspose.cells.Cell-}
```
public abstract void startCell(Cell cell)
```


Bir hücrenin verilerini kaydetmeye başlar.

**Remarks**

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Veri doldurmak için uygulamanın kullanacağı Cell nesnesi. Sütun indeksi, en son [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--) çağrısının döndürdüğü değerdir. Hücre iç hücre modelinde başlatıldıysa mevcut Cell nesnesi kullanılır. Aksi takdirde, veri doldurmak için geçici bir Cell nesnesi kullanılır. |

### startRow(Row row) {#startRow-com.aspose.cells.Row-}
```
public abstract void startRow(Row row)
```


Bir satırın verilerini kaydetmeye başlar.

**Remarks**

Bir satırı ve hücre verilerini kaydetmeye başlarken çağrılır. Mevcut satırın yükseklik, stil vb. gibi özel özellikleri varsa, uygulama bu özellikleri burada verilen Row nesnesine ayarlamalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Veri doldurmak için uygulamanın kullanacağı Row nesnesi. Satır indeksi, en son [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--) çağrısının döndürdüğü değerdir. Satır iç hücre modelinde başlatıldıysa mevcut Row nesnesi kullanılır. Aksi takdirde, veri doldurmak için geçici bir Row nesnesi kullanılır. |

### startSheet(int sheetIndex) {#startSheet-int-}
```
public abstract boolean startSheet(int sheetIndex)
```


Bir çalışma sayfasını kaydetmeye başlar.

**Remarks**

Bir çalışma kitabını kaydederken bir çalışma sayfasını kaydetmeye başlarken çağrılır. Sağlayıcının startRow(Row) veya startCell(Cell) yönteminde daha sonra *`sheetIndex`*'e başvurması gerekiyorsa, yani işlemin hangi çalışma sayfasının işlendiğini bilmesi gerekiyorsa, uygulama *`sheetIndex`* değerini burada tutmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | int | Kaydedilecek mevcut sayfanın indeksi. |

**Returns:**
boolean - bu sağlayıcı verilen sayfa için veri sağlayacaksa true; verilen sayfanın normal veri modeli (Cells) kullanılacaksa false.
