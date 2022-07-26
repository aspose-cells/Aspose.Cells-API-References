---
title: GridDesktop
second_title: Aspose.Cells for .NET API Referansı
description: Aspose GridDesktop class Bir GridDesktop denetimi oluşturmak için bir kök nesneyi temsil eder. Bu denetimi kullanmak için araç kutunuzdan bir forma veya kullanıcı denetimine sürüklemeniz yeterlidir.
type: docs
weight: 840
url: /tr/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

Aspose GridDesktop class Bir GridDesktop denetimi oluşturmak için bir kök nesneyi temsil eder. Bu denetimi kullanmak için, araç kutunuzdan bir forma veya kullanıcı denetimine sürüklemeniz yeterlidir.

```csharp
public class GridDesktop : UserControl
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [GridDesktop](griddesktop)() | Aspose GridDesktop class |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex) { get; set; } | Seçili sayfa dizinini alır veya ayarlar. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont) { get; set; } | Sayfa çubuğunun yazı tipini gösteren etkin sayfayı alır veya ayarlar. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas) { get; set; } | Tüm formülleri çalıştırdığımızda olduğu gibi, tüm formülleri çalıştırmamız gerekip gerekmediğini belirten bir değer alır veya ayarlar, bir hücre değerini güncellerken ve diğerlerini etkiler ve diğerleri de diğerlerini etkiler, giderek daha fazla, tüm hücrelerin yeniden hesaplanması gerekmesine neden olur , tıpkı Kelebek Etkisi gibi, çok sayıda yığın işlemine ihtiyaç duyar, çok düşük performans alır, CELLSNET-41921'deki gibi, bu sorun bu senaryoyu gösterebilen dosyayı içerir tüm formülleri çalıştırsak iyi olur, , tüm formülleri çalıştırırken olduğu gibi bazı optimizasyonlara sahip olabiliriz. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle) { get; set; } | Kontrol için kenarlık stilini gösterir. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible) { get; set; } | Sütun başlığının görünür olup olmadığını belirten bir değer alır veya ayarlar. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont) { get; set; } | Yorum metninin varsayılan görüntüleme yazı tipini alır veya ayarlar. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager) { get; } | ContextMenuManager örneğini alır. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont) { get; set; } | hücresinin varsayılan yazı tipini alır veya ayarlar |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor) { get; set; } | Hücrenin varsayılan yazı tipi rengini alır veya ayarlar. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste) { get; set; } | MS-EXCEL ile kopyalayıp/yapıştırabilmesi için panoya göre kopyala/yapıştır yapılıp yapılmayacağını belirtir. Yalnızca hücre değerini kopyalar/yapıştırır ,Hücrenin biçim, kenarlık stili vb. gibi başka hiçbir ayarını kopyalamaz Varsayılan değer false. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension) { get; set; } | Kopyalama işleminin satır veya sütun sayısını artırıp artırmayacağını belirten bir değer alır veya ayarlar. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption) { get; set; } | Kopyalama işleminin bir hücrenin stilin CellLocked öznitelik değerini kopyalayıp kopyalamayacağını belirten bir değer alır veya ayarlar. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo) { get; set; } | Geri Al işlevinin etkinleştirilip etkinleştirilmediğini gösteren bir değer alır veya ayarlar. Varsayılan değer false. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting) { get; set; } | Bellek seçeneğini alır veya ayarlar. |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible) { get; set; } | Yatay Kaydırma Çubuğu için görünür durumu ayarlar. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible) { get; set; } | Dikey Kaydırma Çubuğu için görünür durumu ayarlar. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names) { get; } | Elektronik tablodaki tüm Ad nesnelerinin koleksiyonunu alır. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows) { get; set; } | Pagination için satır boyutunu ayarlar veya alır.Desteklenen maksimum Sayfa Satırı sayısı 100000'dir, desteklenen maksimum sayfa sayısı 5000'dir. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype) { get; set; } | Yapıştır eylemi yapıldığında hangi yapıştırma türünü belirtir, yalnızca EnableClipboardCopyPaste yanlış olduğunda kullanılabilir . |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1) { get; set; } | Kontrolün R1C1 başvuru stilini kullanıp kullanmadığını gösteren bir değer alır veya ayarlar. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas) { get; set; } | Bir hücrenin değeri değiştiğinde tüm hücrelerin formülünün yeniden hesaplanıp hesaplanmayacağını belirten bir değer alır veya ayarlar. Varsayılan değer true'dur. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible) { get; set; } | Satır başlığının görünür olup olmadığını belirten bir değer alır veya ayarlar. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont) { get; set; } | Sayfa çubuğunun varsayılan görüntüleme yazı tipini alır veya ayarlar. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible) { get; set; } | Sayfa çubuğunun görünür olup olmadığını belirten bir değer alır veya ayarlar. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth) { get; set; } | Sayfa Sekmesinin genişliğini ayarlar/alır. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu) { get; set; } | Denetimin bağlam menüsünü gösterip gösteremeyeceğini belirten bir değer alır veya ayarlar. |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus) { get; set; } | Status hesaplamasının gösterilip gösterilmeyeceğini belirten bir değer alır veya ayarlar. Varsayılan değer true'dur. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager) { get; } | UndoManager örneğini alır. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets) { get; } | Çalışma Sayfalarını Alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear)() | GridDesktop denetimini temizler. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy)() | Odaklanmış hücre içeriğini panoya kopyalar. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut)() | Odaklanmış hücre içeriğini panoya keser. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit)() | Bölünmüş görünümü ayarlar. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter)() | GridDesktop'a FormatPainter. 'yi sonlandırmasını bildirir |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile)(Stream) | Disk IO akışı veya bellek akışı dahil olmak üzere bir excel dosya akışına dışa aktarır. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_2)(string) | Bir excel dosyasına dışa aktarır. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_1)(Stream, FileFormatType) | Disk IO akışı veya bellek akışı dahil olmak üzere bir excel dosya akışına dışa aktarır. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile#exportexcelfile_3)(string, FileFormatType) | Bir excel dosyasına dışa aktarır. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet)() | Geçerli etkin çalışma sayfasını alır. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar)() | yatay kaydırma çubuğuna dönüş |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar)() | dikey kaydırma çubuğuna dönüş |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile)(Stream) | Disk dosya akışı veya bellek akışı dahil olmak üzere bir excel dosya akışından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_3)(string) | Bir excel dosyasından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_1)(Stream, bool) | Disk dosya akışı veya bellek akışı dahil olmak üzere bir excel dosya akışından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_4)(string, bool) | Bir excel dosyasından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_5)(string, int) | Excel dosyasından bir çalışma sayfasını içe aktarır. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_2)(Stream, string, string, bool, bool) | Bir excel dosyasından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile#importexcelfile_6)(string, string, string, bool, bool) | Bir excel dosyasından içe aktarır. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog)(bool) | Hücreleri bulmak veya değiştirmek için FindReplace iletişim kutusunu açar. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste)() | Pano içeriğini odaklanılan hücreye yapıştırır. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol)() | GridDesktop denetimini yenileyin. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas)() | Tüm hücrelerin formülünü çalıştırır. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible)() | Tüm kaydırma çubuklarını görünür olarak ayarlar. |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog)() | Hücre stilini, yazı tipini, renkleri vb. ayarlamak için bir stil iletişim kutusu açar. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter)(bool) | GridDesktop'a FormatPainter'ı başlatmasını bildirir. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit)() | Bölünmüş görünümü ayarla. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion)() | Yayın sürümünü edinin. |

## Alanlar

| İsim | Tanım |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter) | şablondan çalışma kitabını yüklerken verileri filtreleme seçenekleri. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage) | Dosya içe aktarılamadığında mesaj kutusunun gösterilip gösterilmeyeceği, varsayılan değer true |

## Olaylar

| İsim | Tanım |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns) | Sütun silindikten sonra oluşur. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows) | Satır silindikten sonra gerçekleşir. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns) | Yeni sütun eklendikten sonra oluşur. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows) | Yeni satır eklendikten sonra gerçekleşir. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate) | Çalışma kitabında formülü hesaplamadan önce oluşur. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile) | Çalışma kitabı dosyadan yüklenmeden önce oluşur. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick) | Hücre düğmesi tıklandığında gerçekleşir. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged) | Hücre onay kutusu Checked özelliği değiştirildiğinde gerçekleşir. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick) | Izgara hücresi tıklandığında gerçekleşir. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy) | Bir ızgara hücresi ComboBox kopyalanırken gerçekleşir. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged) | Izgara hücresi veri özelliği değiştirildiğinde gerçekleşir. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick) | Izgara hücresi çift tıklandığında gerçekleşir. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged) | Hücre biçimi, Hücreleri Biçimlendir iletişim kutusu aracılığıyla değiştirildiğinde gerçekleşir. |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed) | Bir hücrenin odağı varken bir tuşa basıldığında gerçekleşir. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged) | Hücre açılan kutusu SelectedIndex özelliği değiştiğinde gerçekleşir. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging) | Bir ızgara hücresine karakter yazarken oluşur. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed) | Bir ızgara hücresi doğrulama başarısız olduğunda gerçekleşir. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick) | Sütun başlığı tıklandığında gerçekleşir. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick) | Sütun başlığı çift tıklandığında gerçekleşir. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged) | Yorum verileri değiştiğinde gerçekleşir. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate) | Çalışma kitabında formülü hesapladıktan sonra oluşur. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile) | Çalışma kitabı yüklendiğinde gerçekleşir. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged) | Odaklanılan hücre değiştirildiğinde gerçekleşir. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged) | Satır/sütun gizleme durumu değiştiğinde gerçekleşir. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent) | Satır filtresi öğesi seçildikten sonra gerçekleşir. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick) | Satır başlığı tıklandığında gerçekleşir. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick) | Satır başlığı çift tıklandığında gerçekleşir. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged) | Seçilen hücre aralığı değiştirildiğinde gerçekleşir. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged) | SelectedSheetIndex özelliği değiştirildiğinde gerçekleşir. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick) | Şekil tıklandığında gerçekleşir. |

### Notlar

System.Windows.Forms.UserControl. hakkında daha fazla bilgi için lütfen .NET SDK belgesine bakın.

### Örnekler

```csharp
[C#]
gridDesktop1.Worksheets[0].Cells[0, 0].Value = "2";
gridDesktop1.Worksheets[0].Cells[1, 0].Value = "3";
gridDesktop1.Worksheets[0].Cells[2, 1].Value = "=a1*a2";
gridDesktop1.RunAllFormulas();
gridDesktop1.Invalidate();

[Visual Basic]
gridDesktop1.Worksheets(0).Cells(0, 0).Value = "2"
gridDesktop1.Worksheets(0).Cells(1, 0).Value = "3"
gridDesktop1.Worksheets(0).Cells(2, 1).Value = "=a1*a2"
gridDesktop1.RunAllFormulas()
gridDesktop1.Invalidate()

```

### Ayrıca bakınız

* ad alanı [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop)
* toplantı [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
