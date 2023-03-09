---
title: LightCellsDataProvider sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1000
url: /tr/python-net/aspose.cells/lightcellsdataprovider/
is_root: false
---
##  LightCellsDataProvider sınıfı
Büyük elektronik tablo dosyalarını hafif ağırlık modunda kaydetmek için Veri sağlayıcıyı temsil eder.



LightCellsDataProvider türü aşağıdaki üyeleri gösterir:

###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [start_sheet(sheet_index)](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/start_sheet/#int) | Bir çalışma sayfasını kaydetmeye başlar.|
| [next_row()](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/next_row/#) | Kaydedilecek bir sonraki satırı alır.|
| [start_row(row)](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/start_row/#Row) | Bir satırın verilerini kaydetmeye başlar.|
| [next_cell()](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/next_cell/#) | Kaydedilecek bir sonraki hücreyi alır.|
| [start_cell(cell)](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/start_cell/#Cell) | Bir hücrenin verilerini kaydetmeye başlar.|
| [is_gather_string()](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/#) |Hücrenin geçerli dize değerinin genel bir havuzda toplanması gerekip gerekmediğini kontrol eder.|



###  Notlar

Bir çalışma kitabını bu modda kaydederken, çalışma kitabındaki her çalışma sayfasını kaydederken [LightCellsDataProvider.start_sheet(sheet_index)](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/start_sheet) kontrol edilecektir.
Bir sayfa için, [LightCellsDataProvider.start_sheet(sheet_index)](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/start_sheet) doğru verirse, bu sayfanın satırlarının/hücrelerinin tüm verileri ve özellikleri kaydedilecektir.
bu arayüzün uygulanması ile sağlanacaktır.İlk etapta [LightCellsDataProvider.next_row()](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/next_row) çağrılarak bir sonraki satır indeksinin kaydedilmesi sağlanacaktır.
Geçerli bir satır dizini döndürülürse (satırların kaydedilmesi için satır dizini artan sırada olmalıdır),
daha sonra bu satırı temsil eden bir Row nesnesi, uygulama için özelliklerini [LightCellsDataProvider.start_row(row)](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/start_row) ile ayarlamak üzere sağlanacaktır.
Bir satır için öncelikle [LightCellsDataProvider.next_cell()](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/next_cell) kontrol edilecektir.Geçerli bir sütun dizini döndürülürse (bir satırın tüm hücrelerinin kaydedilebilmesi için sütun dizini artan sırada olmalıdır),
daha sonra, bu hücreyi temsil eden bir Cell nesnesi, [LightCellsDataProvider.start_cell(cell)](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/start_cell) tarafından veri ve özelliklerini ayarlamak için uygulama için sağlanacaktır.
Bu hücrenin verileri ayarlandıktan sonra, bu hücre doğrudan oluşturulan elektronik tablo dosyasına kaydedilecek ve bir sonraki hücre kontrol edilerek işlenecektir.

###  Ayrıca bakınız
* modül [aspose.cells](..)
