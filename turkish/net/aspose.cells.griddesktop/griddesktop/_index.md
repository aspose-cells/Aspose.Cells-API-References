---
title: "GridDesktop sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridDesktop.GridDesktop sınıfı. Aspose GridDesktop sınıfı, bir GridDesktop denetimi oluşturmak için kök nesneyi temsil eder. Bu denetimi kullanmak için sadece araç kutunuzdan bir forma veya kullanıcı denetimine sürükleyin."
type: docs
url: /tr/net/aspose.cells.griddesktop/griddesktop/
---
## GridDesktop class

Aspose GridDesktop sınıfı, bir GridDesktop kontrolü oluşturmak için kök nesneyi temsil eder. Bu kontrolü kullanmak için, araç kutunuzdan bir forma veya kullanıcı denetimine sürüklemeniz yeterlidir.

```csharp
public class GridDesktop : UserControl
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GridDesktop](griddesktop/)() | Aspose GridDesktop sınıfı |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex/) { get; set; } | Seçili sayfa dizinini alır veya ayarlar. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont/) { get; set; } | Aktif sayfanın sheet bar üzerindeki yazı tipini alır veya ayarlar. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas/) { get; set; } | Tüm formüllerin çalıştırılıp çalıştırılmayacağını gösteren bir değeri alır veya ayarlar. Tüm formüller çalıştırıldığında, bir hücre değeri güncellendiğinde diğerlerini etkiler, diğerleri de diğerlerini etkiler, bu durum hücrelerin tamamının yeniden hesaplanmasına neden olur; tıpkı Kelebek Etkisi gibi, çok sayıda yığın işlemi gerekir ve performans çok düşer. CELLSNET-41921'de olduğu gibi, bu sorun bu senaryoyu gösterebilecek dosyayı içerir; bu yüzden tüm formülleri çalıştırmak daha iyidir, çünkü tüm formüller çalıştırıldığında bazı optimizasyonlar elde edebiliriz. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle/) { get; set; } | Denetim için kenarlık stilini gösterir. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible/) { get; set; } | Sütun başlığının görünür olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont/) { get; set; } | Yorum metninin varsayılan görüntüleme yazı tipini alır veya ayarlar. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager/) { get; } | ContextMenuManager örneğini alır. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont/) { get; set; } | Hücrenin varsayılan yazı tipini alır veya ayarlar. |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor/) { get; set; } | Hücrenin varsayılan yazı tipi rengini alır veya ayarlar. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste/) { get; set; } | Panoya dayalı kopyalama/yapıştırmayı gösterir, böylece MS-EXCEL ile kopyala/yapıştır yapılabilir. Yalnızca hücre değerini kopyalar/yapıştırır, hücrenin formatı, kenarlık stili vb. gibi diğer ayarları kopyalamaz. Varsayılan değer false'tur. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension/) { get; set; } | Kopyalama işleminin satır veya sütun sayısını artırıp artırmayacağını gösteren bir değeri alır veya ayarlar. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption/) { get; set; } | Bir hücrenin stilinin CellLocked öznitelik değerinin kopyalama işlemi tarafından kopyalanıp kopyalanmayacağını gösteren bir değeri alır veya ayarlar. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo/) { get; set; } | Geri alma işlevinin etkin olup olmadığını gösteren bir değeri alır veya ayarlar. Varsayılan değer false'tur. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting/) { get; set; } | Bellek seçeneğini alır veya ayarlar, varsayılan değer GridMemorySetting.Normal'dır. |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible/) { get; set; } | Yatay Kaydırma Çubuğu için görünür durumu ayarlar. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible/) { get; set; } | Dikey Kaydırma Çubuğu için görünür durumu ayarlar. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names/) { get; } | Elektronik tablodaki tüm Name nesnelerinin koleksiyonunu alır. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows/) { get; set; } | Sayfalama için satır boyutunu ayarlar veya alır. Desteklenen maksimum PageRows 100000, desteklenen maksimum sayfa sayısı 5000'dir. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype/) { get; set; } | Yapıştırma eylemi gerçekleştirildiğinde hangi yapıştırma türünün kullanılacağını gösterir, yalnızca EnableClipboardCopyPaste false olduğunda kullanılabilir. Varsayılan değer GridPasteType.Default'tir; |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1/) { get; set; } | Denetimin R1C1 referans stilini kullanıp kullanmadığını gösteren bir değeri alır veya ayarlar. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas/) { get; set; } | Bir hücrenin değeri değiştiğinde tüm hücrelerin formülünün yeniden hesaplanıp hesaplanmayacağını gösteren bir değeri alır veya ayarlar. Varsayılan değer true'tir. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible/) { get; set; } | Satır başlığının görünür olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont/) { get; set; } | Sayfa çubuğunun varsayılan görüntüleme yazı tipini alır veya ayarlar. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible/) { get; set; } | Sayfa çubuğunun görünür olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth/) { get; set; } | Sayfa Sekmesi genişliğini ayarlar/alır. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu/) { get; set; } | Denetimin bağlam menüsünü gösterip gösteremeyeceğini belirten bir değeri alır veya ayarlar. |
| [ShowFormulaWarning](../../aspose.cells.griddesktop/griddesktop/showformulawarning/) { get; set; } | Hücre formül değeri ayarlandığında hata veya uyarı mesajının gösterilip gösterilmeyeceğini ayarlar/alır, varsayılan değer true'tir. |
| [ShowNumberStoredAsTextSymbol](../../aspose.cells.griddesktop/griddesktop/shownumberstoredastextsymbol/) { get; set; } | Sayı dizesi içeren ancak metin biçiminde depolanan hücre için üçgen simgesinin gösterilip gösterilmeyeceğini ayarlar/alır. |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus/) { get; set; } | Hesaplama durumunun gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan değer true'tir. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager/) { get; } | UndoManager örneğini alır. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets/) { get; } | Çalışma sayfalarını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear/)() | GridDesktop denetimini temizler. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy/)() | Odaklanmış hücre içeriğini panoya kopyalar. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut/)() | Odaklanmış hücre içeriğini panoya keser. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit/)() | Bölünmüş görünümü ayarlar. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter/)() | GridDesktop'ı FormatPainter'ı sonlandırması için bildirir. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile)(Stream) | Disk IO akışı veya bellek akışı dahil olmak üzere bir Excel dosya akışına dışa aktarır. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_2)(string) | Bir Excel dosyasına dışa aktarır. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_1)(Stream, FileFormatType) | Disk IO akışı veya bellek akışı dahil olmak üzere bir Excel dosya akışına dışa aktarır. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_3)(string, FileFormatType) | Bir Excel dosyasına aktarır. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile)(Stream, GridPdfSaveOptions) | Disk IO akışı veya bellek akışı dahil olmak üzere bir PDF dosya akışına aktarır. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile_1)(string, GridPdfSaveOptions) | Disk IO akışı veya bellek akışı dahil olmak üzere bir PDF dosya akışına aktarır. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet/)() | Geçerli aktif çalışma sayfasını alır. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar/)() | yatay kaydırma çubuğunu döndür |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar/)() | dikey kaydırma çubuğunu döndür |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile)(Stream) | Disk dosya akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_3)(string) | Bir Excel dosyasından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_1)(Stream, bool) | Disk dosya akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_4)(string, bool) | Bir Excel dosyasından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_5)(string, int) | Bir Excel dosyasından çalışma sayfası içe aktarır. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_2)(Stream, string, string, bool, bool) | Bir Excel dosyasından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_6)(string, string, string, bool, bool) | Bir Excel dosyasından içe aktarır. |
| [Invalidate](../../aspose.cells.griddesktop/griddesktop/invalidate/#invalidate)() | Geçersiz kılmayı geçersiz kıl. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog/)(bool) | Hücreleri bulmak veya değiştirmek için FindReplace iletişim kutusunu açar. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste/)() | Pano içeriğini odaklanmış hücreye yapıştırır. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol/)() | GridDesktop kontrolünü yeniler. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas/)() | Tüm hücrelerin formüllerini çalıştırır. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible/)() | Tüm kaydırma çubuklarını görünür yapar. |
| [SetCustomResourceManager](../../aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/)(ResourceManager) | Kullanıcı tanımlı yerelleştirmeyi uygulamak için özel kaynak yöneticisi ayarlar |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog/)() | Hücre stilini, yazı tipini, renkleri vb. ayarlamak için bir stil iletişim kutusunu açar. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter/)(bool) | GridDesktop'ı FormatPainter'ı başlatması için bildirir. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit/)() | Bölünmüş görünümü kaldır. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion/)() | Sürüm numarasını al. |

## Alanlar

| Ad | Açıklama |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter/) | Şablondan çalışma kitabı yüklenirken veri filtreleme seçenekleri. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage/) | Dosya içe aktarılamadığında ileti kutusunun gösterilip gösterilmeyeceği, varsayılan değer true'dur. |

## Olaylar

| Ad | Açıklama |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns/) | Sütun silindikten sonra gerçekleşir. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows/) | Satır silindikten sonra gerçekleşir. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns/) | Yeni sütun eklendikten sonra gerçekleşir. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows/) | Yeni satır eklendikten sonra gerçekleşir. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate/) | Çalışma kitabında formül hesaplanmadan önce gerçekleşir. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile/) | Çalışma kitabı dosyadan yüklenmeden önce gerçekleşir. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick/) | Hücre düğmesi tıklandığında gerçekleşir. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged/) | Hücre onay kutusunun Checked özelliği değiştiğinde gerçekleşir. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick/) | Izgara hücresi tıklandığında oluşur. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy/) | Bir ızgara hücresi ComboBox'ı kopyalandığında oluşur. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged/) | Izgara hücresi veri özelliği değiştirildiğinde oluşur. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick/) | Izgara hücresi çift tıklandığında oluşur. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged/) | Hücre biçimi, Hücreleri Biçimlendir iletişim kutusu aracılığıyla değiştirildiğinde oluşur. |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed/) | Bir hücre odaklandığında bir tuşa basıldığında oluşur. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged/) | Hücre combobox'ının SelectedIndex özelliği değiştiğinde oluşur. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging/) | Izgara hücresine karakter girildiğinde oluşur. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed/) | Izgara hücresi doğrulaması başarısız olduğunda oluşur. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick/) | Sütun başlığı tıklandığında oluşur. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick/) | Sütun başlığı çift tıklandığında oluşur. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged/) | Yorum verisi değiştiğinde oluşur. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile/) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate/) | Çalışma kitabında formül hesaplandıktan sonra oluşur. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile/) | Çalışma kitabı yüklendiğinde oluşur. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged/) | Odaklanan hücre değiştiğinde oluşur. |
| event [PictureClick](../../aspose.cells.griddesktop/griddesktop/pictureclick/) | Şekil tıklandığında oluşur. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged/) | Satır/sütun gizleme durumu değiştiğinde oluşur. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent/) | Satır filtresi öğesi seçildikten sonra oluşur. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick/) | Satır başlığı tıklandığında oluşur. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick/) | Satır başlığı çift tıklandığında oluşur. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged/) | Seçili hücre aralığı değiştiğinde oluşur. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged/) | SelectedSheetIndex özelliği değiştiğinde oluşur. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick/) | Şekil tıklandığında oluşur. |

### Açıklamalar

.NET SDK belgesine, System.Windows.Forms.UserControl hakkında daha fazla bilgi için bakınız.

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

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


