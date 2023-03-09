---
title: LightCellsDataHandler sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 990
url: /tr/python-net/aspose.cells/lightcellsdatahandler/
is_root: false
---
##  LightCellsDataHandler sınıfı
Büyük elektronik tablo dosyalarını hafif ağırlık modunda okumak için hücre veri işleyicisini temsil eder.



LightCellsDataHandler türü aşağıdaki üyeleri gösterir:

###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [start_sheet(sheet)](/cells/tr/python-net/aspose.cells/lightcellsdatahandler/start_sheet/#Worksheet) | Bir çalışma sayfasını işlemeye başlar.|
| [start_row(row_index)](/cells/tr/python-net/aspose.cells/lightcellsdatahandler/start_row/#int) | Bir satırı işlemek için hazırlanır.|
| [process_row(row)](/cells/tr/python-net/aspose.cells/lightcellsdatahandler/process_row/#Row) | Bir satırı işlemeye başlar.|
| [start_cell(column_index)](/cells/tr/python-net/aspose.cells/lightcellsdatahandler/start_cell/#int) | Bir hücreyi işlemek için hazırlanır.|
| [process_cell(cell)](/cells/tr/python-net/aspose.cells/lightcellsdatahandler/process_cell/#Cell) | Bir hücreyi işlemeye başlar.|



###  Notlar

Bu modda bir çalışma kitabı okurken, çalışma kitabındaki her çalışma sayfasını okurken [LightCellsDataHandler.start_sheet(sheet)](/cells/tr/python-net/aspose.cells/lightcellsdatahandler/start_sheet) kontrol edilecektir.
Bir sayfa için, [LightCellsDataHandler.start_sheet(sheet)](/cells/tr/python-net/aspose.cells/lightcellsdatahandler/start_sheet) doğru verirse, bu sayfanın satırlarının/hücrelerinin tüm verileri ve özellikleri kontrol edilecektir.
ve bu arayüzün uygulanması ile işlenir.Her satır için [LightCellsDataHandler.start_row(row_index)](/cells/tr/python-net/aspose.cells/lightcellsdatahandler/start_row) aranarak işlenmesi gerekip gerekmediği kontrol edilir.
Eğer bir satırın işlenmesi gerekiyorsa öncelikle bu satırın özellikleri okunur ve kullanıcı [LightCellsDataHandler.process_row(row)](/cells/tr/python-net/aspose.cells/lightcellsdatahandler/process_row) ile bu satırın özelliklerine erişebilir.
satır hücrelerinin de işlenmesi gerekiyorsa, o zaman [LightCellsDataHandler.process_row(row)](/cells/tr/python-net/aspose.cells/lightcellsdatahandler/process_row) true döndürmeli ve ardından [LightCellsDataHandler.start_cell(column_index)](/cells/tr/python-net/aspose.cells/lightcellsdatahandler/start_cell) olacaktır
bir hücrenin işlenmesi gerekip gerekmediğini kontrol etmek için bu satırdaki mevcut her hücreye çağrıldı.
daha sonra bu arayüzün uygulanmasıyla hücreyi işlemek için [LightCellsDataHandler.process_cell(cell)](/cells/tr/python-net/aspose.cells/lightcellsdatahandler/process_cell) çağrılacaktır.

###  Ayrıca bakınız
* modül [aspose.cells](..)
