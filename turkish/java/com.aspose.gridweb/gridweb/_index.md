---
title: "GridWeb"
second_title: "Aspose.Cells for Java API Referansı"
description: "GridWeb denetiminin temel sınıfı."
type: docs
url: /tr/java/com.aspose.gridweb/gridweb/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebControl](../../com.aspose.gridweb/webcontrol), [com.aspose.gridweb.ExtWebControl](../../com.aspose.gridweb/extwebcontrol), [com.aspose.gridweb.MainWeb](../../com.aspose.gridweb/mainweb)
```
public class GridWeb extends MainWeb
```

GridWeb denetiminin temel sınıfı.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridWeb()](#GridWeb--) |  |
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [AfterColumnFilter](#AfterColumnFilter) | Sütun filtrelendikten sonra gerçekleşir. |
| [AjaxCallFinished](#AjaxCallFinished) | Kontrolün ajax güncellemesi tamamlandığında tetiklenir. |
| [BeforeColumnFilter](#BeforeColumnFilter) | Filtrelenecek sütundan önce gerçekleşir. |
| [CellClickOnAjax](#CellClickOnAjax) | Hücre tıklandığında gerçekleşir ve bu olay için ajaxcallback yapılması gerekir. |
| [CellClientUpdate](#CellClientUpdate) | İstemci hücre güncellemesi gerçekleştiğinde gerçekleşir. |
| [CellCommand](#CellCommand) | Hücrenin komut hiperlinki tıklandığında gerçekleşir. |
| [CellDoubleClick](#CellDoubleClick) | Hücre çift tıklandığında gerçekleşir. |
| [CellModifiedOnAjax](#CellModifiedOnAjax) | Hücre ajax çağrısında değiştirildiğinde gerçekleşir. |
| [ColumnDeleted](#ColumnDeleted) | Kullanıcı istemci tarafı menüsünden bir sütunu sildiğinde gerçekleşir. |
| [ColumnDeleting](#ColumnDeleting) | Kullanıcı istemci tarafı menüsünden bir sütunu silmeye çalıştığında gerçekleşir. |
| [ColumnDoubleClick](#ColumnDoubleClick) | Sütun başlığı çift tıklandığında gerçekleşir. |
| [ColumnInserted](#ColumnInserted) | Kullanıcı istemci tarafı menüsünden bir sütun eklediğinde gerçekleşir. |
| [CustomCommand](#CustomCommand) | Kullanıcı özel bir komut düğmesine tıkladığında gerçekleşir. |
| [LoadCustomData](#LoadCustomData) | Denetimin SessionMode'u Custom olarak ayarlandığında ve sayfa verilerini yüklemesi gerektiğinde tetiklenir. |
| [PageIndexChanged](#PageIndexChanged) | Denetimin sayfa dizini değiştiğinde oluşur. |
| [RowDeleted](#RowDeleted) | Kullanıcı istemci tarafı menüsünden bir satırı sildiğinde oluşur. |
| [RowDeleting](#RowDeleting) | Kullanıcı istemci tarafı menüsünden bir satırı silmeye çalıştığında oluşur. |
| [RowDoubleClick](#RowDoubleClick) | Satır başlığı çift tıklandığında oluşur. |
| [RowInserted](#RowInserted) | Kullanıcı istemci tarafı menüsünden bir satır eklediğinde oluşur. |
| [SaveCommand](#SaveCommand) | \"save\" düğmesi tıklandığında oluşur. |
| [SheetAdded](#SheetAdded) | Kullanıcı araç çubuğu menüsünden bir çalışma sayfası eklediğinde oluşur. |
| [SheetTabClick](#SheetTabClick) | Sayfa sekmesi tıklandığında oluşur. |
| [SubmitCommand](#SubmitCommand) | \"submit\" düğmesi tıklandığında oluşur. |
| [UndoCommand](#UndoCommand) | \"undo\" düğmesi tıklandığında oluşur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [calculateFormula()](#calculateFormula--) | Formüllerin sonucunu hesaplar. |
| [createChildControls()](#createChildControls--) | WebControl'dan CreateChildControls uygular, yalnızca dahili kullanım içindir. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getACWClientPath()](#getACWClientPath--) | Denetimin script/görüntü dosyalarının web yolunu alır. |
| [getACWLanguageFileUrl()](#getACWLanguageFileUrl--) | Denetimin dil dosyasının web URL'sini alır. |
| [getActiveCell()](#getActiveCell--) | Mevcut sayfanın etkin hücresini alır. |
| [getActiveCellBgColor()](#getActiveCellBgColor--) | Etkin hücrenin arka plan rengini belirtir. |
| [getActiveCellColor()](#getActiveCellColor--) | Etkin hücrenin rengini belirtir. |
| [getActiveHeaderBgColor()](#getActiveHeaderBgColor--) | Etkin satır/sütun başlığının arka plan rengini belirtir. |
| [getActiveHeaderColor()](#getActiveHeaderColor--) | Etkin satır/sütun başlığının rengini belirtir. |
| [getActiveSheet()](#getActiveSheet--) | Etkin sayfayı alır |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Etkin sayfa dizinini alır. |
| [getActiveTabStyle()](#getActiveTabStyle--) | Etkin sekmenin stilini belirtir. |
| [getAutoRefreshChart()](#getAutoRefreshChart--) | Hücre değerini güncellerken Grafik görüntüsünün güncellenip güncellenmediğini alır. Varsayılan değer true'tur. |
| [getBackColor()](#getBackColor--) | WebControl içinde BackColor'i alır |
| [getBorderColor()](#getBorderColor--) | WebControl içinde BorderColor'i alır |
| [getBorderStyle()](#getBorderStyle--) | WebControl içinde BorderStyle'i alır |
| [getBorderWidth()](#getBorderWidth--) | WebControl içinde BorderWidth'i alır |
| [getBottomTableStyle()](#getBottomTableStyle--) | Denetimin alt çubuğunun stilini alır. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | WebControl içindeki CssClass'i alır |
| [getCurrentPageIndex()](#getCurrentPageIndex--) | Sayfalama modunda geçerli sayfa dizinini alır. |
| [getCustomCalculationEngine()](#getCustomCalculationEngine--) | Kullanıcının, Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel hesaplama motorunu temsil eder. |
| [getCustomCommandButtons()](#getCustomCommandButtons--) | Özel komut düğmesi koleksiyonunu alır |
| [getCustomStyleFileName()](#getCustomStyleFileName--) | Özel stil dosya adını alır. |
| [getDPI()](#getDPI--) | Makinenin DPI değerini alır/ayarlar. |
| [getDefaultFontName()](#getDefaultFontName--) | Denetimin varsayılan yazı tipi adını alır. |
| [getDefaultFontSize()](#getDefaultFontSize--) | Denetimin varsayılan yazı tipi boyutunu alır. |
| [getDefaultGridLineColor()](#getDefaultGridLineColor--) | Varsayılan ızgara çizgisinin rengini alır. |
| [getDisplayCellTip()](#getDisplayCellTip--) | İpuçlarının gösterilip gösterilmeyeceğini alır. Varsayılan değer doğrudur. |
| [getEditMode()](#getEditMode--) | Denetimin düzenleme modunu alır. |
| [getEnableAJAX()](#getEnableAJAX--) | AJAX çağrısının kullanılıp kullanılmayacağını alır. Varsayılan değer doğrudur. |
| [getEnableAsync()](#getEnableAsync--) | Hücre verilerinin asenkron şekilde yüklenip yüklenmeyeceğini alır, 10.000'den fazla hücre içeren bir sayfa için uygulanması önerilir. |
| [getEnableClientColumnOperations()](#getEnableClientColumnOperations--) | İstemci tarafı sütun işlemlerinin etkinleştirilip etkinleştirilmeyeceğini alır. |
| [getEnableClientFreeze()](#getEnableClientFreeze--) | İstemci tarafı dondurma işlemlerinin etkinleştirilip etkinleştirilmeyeceğini alır. |
| [getEnableClientMergeOperations()](#getEnableClientMergeOperations--) | İstemci tarafı birleştirme işlemlerinin etkinleştirilip etkinleştirilmeyeceğini alır. |
| [getEnableClientResizeColumnRow()](#getEnableClientResizeColumnRow--) | İstemci tarafı sütun ve satır yeniden boyutlandırmanın etkinleştirilip etkinleştirilmeyeceğini alır. |
| [getEnableClientRowOperations()](#getEnableClientRowOperations--) | İstemci tarafı satır işlemlerinin etkinleştirilip etkinleştirilmeyeceğini alır. |
| [getEnableDoubleClickEvent()](#getEnableDoubleClickEvent--) | Müşteri tarafı çift tıklama olayının etkinleştirilip etkinleştirilmeyeceğini alır. |
| [getEnableMetalLightEffect()](#getEnableMetalLightEffect--) | Metal ışık etkisinin uygulanıp uygulanmayacağını alır. |
| [getEnablePaging()](#getEnablePaging--) | Denetimin sayfalama modunun etkinleştirilip etkinleştirilmeyeceğini alır. |
| [getEnableStyleDialogbox()](#getEnableStyleDialogbox--) | İstemci tarafı stil iletişim kutusunun etkinleştirilip etkinleştirilmeyeceğini alır. |
| [getEnabled()](#getEnabled--) | WebControl içindeki Enabled'ı alır |
| [getFilteredPaging()](#getFilteredPaging--) | Veri filtrelendikten sonra sayfalamanın etkinleştirilip etkinleştirilmeyeceğini alır, EnablePaging true olduğunda etkili olur. |
| [getFont()](#getFont--) | WebControl içindeki Font'u alır |
| [getForceValidation()](#getForceValidation--) | Müşteri tarafı doğrulamanın zorunlu olup olmadığını alır. |
| [getForeColor()](#getForeColor--) | WebControl içindeki ForeColor'ı alır |
| [getFrameTableStyle()](#getFrameTableStyle--) | Denetimin çerçeve stilini alır. |
| [getGoonDefaultSaveOperation()](#getGoonDefaultSaveOperation--) | GridWeb'in varsayılan kaydetme işlemini yapıp yapmayacağını alır, varsayılan değer doğrudur. |
| [getHeaderBarHeight()](#getHeaderBarHeight--) | Denetimin üst başlık çubuğunun yüksekliğini (System.Web.UI.WebControl.Unit) alır. |
| [getHeaderBarStyle()](#getHeaderBarStyle--) | Başlık çubuğunun stilini alır. |
| [getHeaderBarTableStyle()](#getHeaderBarTableStyle--) | Denetimin başlık çubuğu stilini alır. |
| [getHeaderBarWidth()](#getHeaderBarWidth--) | Denetimin genişliğini (System.Web.UI.WebControl.Unit) veya sol başlık çubuğunu alır. |
| [getHeight()](#getHeight--) | Denetimin yüksekliğini (System.Web.UI.WebControl.Unit) alır. |
| [getIgnoreStyleWithNoData()](#getIgnoreStyleWithNoData--) | GridWeb'ün hücre değeri içermeyen ancak stillendirilmiş satırları veya sütunları göstermeyi göz ardı edip etmediğini alır. |
| [getLoadOptions()](#getLoadOptions--) | GridWeb için yükleme seçeneklerini temsil eder. |
| [getMaxColumn()](#getMaxColumn--) | Web sayfasının maksimum görüntüleme sütun indeksini (sıfır tabanlı) alır. |
| [getMaxRow()](#getMaxRow--) | Web sayfasının maksimum görüntüleme satır indeksini (sıfır tabanlı) alır. |
| [getMessage()](#getMessage--) | Izgara için mesajı alır. |
| [getMinColumn()](#getMinColumn--) | Web sayfasının minimum görüntüleme sütun indeksini (sıfır tabanlı) alır. |
| [getMinRow()](#getMinRow--) | Web sayfasının minimum görüntüleme satır indeksini (sıfır tabanlı) alır. |
| [getModifiedCells()](#getModifiedCells--) | İstemci tarafından değiştirilen hücrelerin koleksiyonunu alır. |
| [getNeedRenderGroupRows()](#getNeedRenderGroupRows--) | Grup satırlarının gösterilip gösterilmeyeceğini alır. |
| [getNoHScroll()](#getNoHScroll--) | Yatay kaydırma çubuğunun gizli olup olmadığını belirten bir değeri alır. |
| [getNoScroll()](#getNoScroll--) | Kaydırma çubuğunun gösterilip gösterilmeyeceğini alır. |
| [getNoVScroll()](#getNoVScroll--) | Dikey kaydırma çubuğunun gizli olup olmadığını belirten bir değeri alır. |
| [getOnAjaxCallFinishedClientFunction()](#getOnAjaxCallFinishedClientFunction--) | Ajax çağrısı tamamlandığında çağrılacak istemci tarafı fonksiyon adını alır. |
| [getOnCellErrorClientFunction()](#getOnCellErrorClientFunction--) | Bir hücrenin doğrulaması başarısız olduğunda çağrılacak istemci tarafı fonksiyon adını alır. |
| [getOnCellSelectedAjaxCallBackClientFunction()](#getOnCellSelectedAjaxCallBackClientFunction--) | Bir hücre seçildiğinde çağrılacak istemci tarafı fonksiyonu alır. |
| [getOnCellSelectedClientFunction()](#getOnCellSelectedClientFunction--) | Bir hücre seçildiğinde çağrılacak istemci tarafı fonksiyonu alır. |
| [getOnCellUnselectedClientFunction()](#getOnCellUnselectedClientFunction--) | Bir hücre seçimi kaldırıldığında çağrılacak istemci tarafı fonksiyonu alır. |
| [getOnCellUpdatedClientFunction()](#getOnCellUpdatedClientFunction--) | Bir hücrenin değeri güncellendiğinde çağrılacak istemci tarafı fonksiyon adını alır. |
| [getOnContextMenuShowClientFunction()](#getOnContextMenuShowClientFunction--) | Bağlam menüsü gösterildiğinde çağrılacak istemci tarafı fonksiyonunu alır. |
| [getOnDoubleClickCellClientFunction()](#getOnDoubleClickCellClientFunction--) | Bir hücre çift tıklandığında çağrılacak istemci tarafı fonksiyonunu alır. |
| [getOnDoubleClickRowClientFunction()](#getOnDoubleClickRowClientFunction--) | Bir satır çift tıklandığında çağrılacak istemci tarafı fonksiyonunu alır. |
| [getOnGridInitClientFunction()](#getOnGridInitClientFunction--) | Izgara başlatıldığında çağrılacak istemci tarafı fonksiyon adını alır. |
| [getOnPageChangeClientFunction()](#getOnPageChangeClientFunction--) | Sayfa indeksi değiştikten sonra çağrılacak istemci tarafı fonksiyonunu alır. Yalnızca EnablePaging true olduğunda etkili olur. |
| [getOnPageSubmitClientFunction()](#getOnPageSubmitClientFunction--) | Sayfa istemci tarafında gönderilmeden önce çağrılacak istemci fonksiyonunu alır. |
| [getOnShapeSelectedClientFunction()](#getOnShapeSelectedClientFunction--) | Bir şekil seçildiğinde çağrılacak istemci tarafı işlevi alır. |
| [getOnSubmitClientFunction()](#getOnSubmitClientFunction--) | Denetim istemci tarafında gönderilmeden önce çağrılacak istemci işlevini alır. |
| [getOnlyAuto()](#getOnlyAuto--) | Yüksekliği özelleştirilmemiş satırların yalnızca sığdırılıp sığdırılmayacağını alır, varsayılan değer false'tur. |
| [getPageSize()](#getPageSize--) | Sayfalama modundaki sayfa boyutunu alır. |
| [getPictureCachePath()](#getPictureCachePath--) | Çalışma kitabı için görüntü depolama yolunu alır, tüm şekiller ve görüntüler bu dizinde saklanır, varsayılan yol geçerli uygulamanın temel dizini altındaki acwcache'tir, kullanıcıların oturum süresi dışındaki dosyaları temizlemek için bir zamanlama hizmeti uygulamaları gerekir. |
| [getPresetStyle()](#getPresetStyle--) | Ön ayarlı stili alır. |
| [getRefreshValidation()](#getRefreshValidation--) | Hücre değeri değiştikten sonra doğrulama değerinin yenilenip yenilenmeyeceğini alır. |
| [getRenderHiddenRow()](#getRenderHiddenRow--) | Gizli satırın GridControl içinde işlenip işlenmeyeceğini alır, varsayılan değer false'tur. |
| [getRowHeightForCSV()](#getRowHeightForCSV--) | CSV dosyası için satır yüksekliği değerini puan cinsinden alır, varsayılan değer 14.5'tir. |
| [getScrollBarArrowColor()](#getScrollBarArrowColor--) | Kaydırma çubuğunun ok düğmesinin rengini belirtir. |
| [getScrollBarBaseColor()](#getScrollBarBaseColor--) | Denetimin kaydırma çubuğunun rengini belirtir. |
| [getSelectCellBgColor()](#getSelectCellBgColor--) | Çoklu seçim aralığındaki seçili hücrelerin arka plan rengini belirtir. |
| [getSelectCellColor()](#getSelectCellColor--) | Çoklu seçim aralığındaki seçili hücrelerin rengini belirtir. |
| [getSelectCells()](#getSelectCells--) | Seçili hücre koleksiyonunu alır. |
| [getSessionStorePath()](#getSessionStorePath--) | Oturum modu File veya ViewState olduğunda oturum önbellek depolama yolunu alır, örnek: gridweb.SessionStorePath="c:/mytempdir/session"; ardından oturum verileri c:/mytempdir/session içinde saklanır. |
| [getSettings()](#getSettings--) | Çalışma kitabı ayarlarını temsil eder. |
| [getShowAddButton()](#getShowAddButton--) | Çalışma sayfası ekleme düğmesinin gösterilip gösterilmeyeceğini alır. |
| [getShowBottomBar()](#getShowBottomBar--) | Denetimin alt kısmında komut çubuğunun (komut çubuğu ve sekme çubuğu dahil) gösterilip gösterilmeyeceğini belirtir. |
| [getShowCellEditBox()](#getShowCellEditBox--) | Gridweb'in MS-EXCEL gibi düzenleme kutusu araç çubuğunu gösterip göstermediği. Etkinleştirilirse, geçerli hücre için bir düzenleme kutusu Gridweb'de görüntülenir. |
| [getShowCommandBarAtTop()](#getShowCommandBarAtTop--) | Denetimin üst kısmında komut çubuğunun (komut çubuğu ve sekme çubuğu dahil) gösterilip gösterilmeyeceğini belirtir. |
| [getShowContextMenu()](#getShowContextMenu--) | Bağlam menüsünün gösterilip gösterilmeyeceğini alır. Varsayılan değer true'tur. |
| [getShowDefaultGridLine()](#getShowDefaultGridLine--) | Hücrelerin varsayılan ızgara çizgilerinin gösterilip gösterilmeyeceğini alır. |
| [getShowHeaderBar()](#getShowHeaderBar--) | Başlık çubuğunun gösterilip gösterilmeyeceğini alır. |
| [getShowLoading()](#getShowLoading--) | Sunucuya postback yapılırken bir yükleme iletişim kutusunun gösterilip gösterilmeyeceğini belirtir. |
| [getShowLoadingPosition()](#getShowLoadingPosition--) | Sunucuya postback yapılırken yükleme iletişim kutusunun gösterileceği sol, üst konumunu (px cinsinden) belirtir, vb. 100,200 ifadesi, yükleme iletişim kutusunun sol, üst konumunun 100px,200px olduğu anlamına gelir. |
| [getShowSaveButton()](#getShowSaveButton--) | Kaydet düğmesinin gösterilip gösterilmeyeceğini alır. |
| [getShowSubmitButton()](#getShowSubmitButton--) | Gönder düğmesinin gösterilip gösterilmeyeceğini alır. |
| [getShowTabBar()](#getShowTabBar--) | Sekme çubuğunun gösterilip gösterilmeyeceğini alır. |
| [getShowTabNavigation()](#getShowTabNavigation--) | Sekme gezinme düğmesinin gösterilip gösterilmeyeceğini alır, varsayılan değer true'dur. |
| [getShowUndoButton()](#getShowUndoButton--) | Geri al düğmesinin gösterilip gösterilmeyeceğini alır. |
| [getSpanWrap()](#getSpanWrap--) | İçeriğin hücre aralığında sarılıp sarılmayacağını belirtir, varsayılan değer true'dur. |
| [getTabIndex()](#getTabIndex--) | WebControl içindeki TabIndex'i alır |
| [getTabStyle()](#getTabStyle--) | Sekme çubuğunun stilini alır. |
| [getToolTip()](#getToolTip--) | WebControl içindeki ToolTip'i alır |
| [getUseClientPageHeight()](#getUseClientPageHeight--) | GridWeb'ün istemci sayfa yüksekliğini kontrol yüksekliği olarak kullanıp kullanmayacağını alır, Height=\"100%\" ayarlandığında uygundur, varsayılan değer false'tur. |
| [getVersion()](#getVersion--) | Sürüm numarasını al. |
| [getViewPanelScrollLeft()](#getViewPanelScrollLeft--) | Izgaranın görünüm panelindeki kaydırma çubuğunun konumunu alır. |
| [getViewPanelScrollTop()](#getViewPanelScrollTop--) | Izgaranın görünüm panelindeki kaydırma çubuğunun konumunu alır. |
| [getViewTableStyle()](#getViewTableStyle--) | Veri görünüm panelinin stilini alır. |
| [getWidth()](#getWidth--) | Denetimin genişliğini (System.Web.UI.WebControl.Unit) alır. |
| [getWorkSheets()](#getWorkSheets--) | Çalışma sayfalarının koleksiyonunu alır. |
| [getXhtmlMode()](#getXhtmlMode--) | XHTML stilinin kullanılıp kullanılmayacağını alır, varsayılan değer true'dur. |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream stream)](#importExcelFile-java.io.InputStream-) | Disk dosyası akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışından içe aktarır. |
| [importExcelFile(InputStream stream, String passwordtoOpen)](#importExcelFile-java.io.InputStream-java.lang.String-) | Disk dosyası akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışından içe aktarır. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Bir Excel dosyasından içe aktarır. |
| [importExcelFile(String fileName, String passwordtoOpen)](#importExcelFile-java.lang.String-java.lang.String-) | Bir Excel dosyasından içe aktarır. |
| [isCalculateFormula()](#isCalculateFormula--) | Hücre değeri değiştikten sonra veya dosya içe aktarıldıktan sonra formülün hesaplanıp hesaplanmayacağını alır. |
| [loadCSVFile(InputStream stream)](#loadCSVFile-java.io.InputStream-) | CSV dosyası akışından verileri yükler. |
| [loadCSVFile(String fileName)](#loadCSVFile-java.lang.String-) | CSV dosyasından verileri yükler. |
| [loadHTMLFile(InputStream stream)](#loadHTMLFile-java.io.InputStream-) | HTML dosyası akışından verileri yükler. |
| [loadHTMLFile(String fileName)](#loadHTMLFile-java.lang.String-) | HTML dosyasından verileri yükler. |
| [loadSpreadSheetMLFile(InputStream stream)](#loadSpreadSheetMLFile-java.io.InputStream-) | SpreadSheetML dosyası akışından verileri yükler. |
| [loadSpreadSheetMLFile(String fileName)](#loadSpreadSheetMLFile-java.lang.String-) | SpreadSheetML dosyasından verileri yükler. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshChartShape()](#refreshChartShape--) | Etkin çalışma sayfası için tüm grafik görüntülerini yeniler. |
| [saveCSVFile(OutputStream stream)](#saveCSVFile-java.io.OutputStream-) | Verileri CSV dosyası akışına kaydeder. |
| [saveCSVFile(String targetFile)](#saveCSVFile-java.lang.String-) | Verileri CSV dosyasına kaydeder. |
| [saveCustomStyleFile(String fileName)](#saveCustomStyleFile-java.lang.String-) | Denetimin mevcut stil verilerini bir XML dosyasına kaydeder. |
| [saveHTMLFile(OutputStream stream)](#saveHTMLFile-java.io.OutputStream-) | Verileri bir HTML dosya akışına kaydeder. |
| [saveHTMLFile(String targetFile)](#saveHTMLFile-java.lang.String-) | Verileri bir HTML dosyasına kaydeder. |
| [saveSpreadSheetMLFile(OutputStream stream)](#saveSpreadSheetMLFile-java.io.OutputStream-) | Verileri bir SpreadSheetML dosya akışına kaydeder. |
| [saveSpreadSheetMLFile(String targetFile)](#saveSpreadSheetMLFile-java.lang.String-) | Verileri bir SpreadSheetML dosyasına kaydeder. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Çalışma sayfalarını bir Excel dosyasına kaydeder. |
| [saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)](#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-) | Çalışma sayfalarını bir Excel dosyasına kaydeder. |
| [saveToExcelFile(OutputStream stream, int format)](#saveToExcelFile-java.io.OutputStream-int-) | Çalışma sayfalarını bir Excel dosyasına kaydeder. |
| [saveToExcelFile(String targetFile)](#saveToExcelFile-java.lang.String-) | Çalışma sayfalarını Excel 2003 formatında bir Excel dosyasına kaydeder. |
| [saveToExcelFile(String targetFile, GridSaveOptions saveOptions)](#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-) | Çalışma sayfalarını bir Excel dosyasına kaydeder. |
| [saveToExcelFile(String targetFile, int format)](#saveToExcelFile-java.lang.String-int-) | Çalışma sayfalarını bir Excel dosyasına kaydeder. |
| [setACWClientPath(String value)](#setACWClientPath-java.lang.String-) | Denetimin script/görüntü dosyalarının web yolunu ayarlar. |
| [setACWLanguageFileUrl(String value)](#setACWLanguageFileUrl-java.lang.String-) | Denetimin dil dosyasının web URL'sini ayarlar. |
| [setActiveCell(GridCell value)](#setActiveCell-com.aspose.gridweb.GridCell-) | Geçerli sayfanın etkin hücresini ayarlar. |
| [setActiveCellBgColor(Color value)](#setActiveCellBgColor-com.aspose.gridweb.Color-) | Etkin hücrenin arka plan rengini belirtir. |
| [setActiveCellColor(Color value)](#setActiveCellColor-com.aspose.gridweb.Color-) | Etkin hücrenin rengini belirtir. |
| [setActiveHeaderBgColor(Color value)](#setActiveHeaderBgColor-com.aspose.gridweb.Color-) | Etkin satır/sütun başlığının arka plan rengini belirtir. |
| [setActiveHeaderColor(Color value)](#setActiveHeaderColor-com.aspose.gridweb.Color-) | Etkin satır/sütun başlığının rengini belirtir. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Etkin sayfa dizinini ayarlar. |
| [setActiveTabStyle(GridTableItemStyle value)](#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Etkin sekmenin stilini belirtir. |
| [setAutoRefreshChart(boolean value)](#setAutoRefreshChart-boolean-) | Hücre değeri güncellenirken Grafik görüntüsünün güncellenip güncellenmeyeceğini ayarlar. Varsayılan değer true'tur. |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | WebControl içindeki BackColor'ı ayarlar |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | WebControl içindeki BorderColor'ı ayarlar |
| [setBorderStyle(int value)](#setBorderStyle-int-) | WebControl içindeki BorderStyle'ı ayarlar |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | WebControl içindeki BorderWidth'ı ayarlar |
| [setBottomTableStyle(GridTableStyle value)](#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-) | Denetimin alt çubuğunun stilini ayarlar. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Hücre değeri değiştikten sonra veya dosya içe aktarıldıktan sonra formülün hesaplanıp hesaplanmayacağını ayarlar. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | WebControl içindeki CssClass'i ayarlar |
| [setCurrentPageIndex(int value)](#setCurrentPageIndex-int-) | Sayfalama modunda geçerli sayfa dizinini ayarlar. |
| [setCustomCalculationEngine(GridAbstractCalculationEngine value)](#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-) | Kullanıcının, Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel hesaplama motorunu temsil eder. |
| [setCustomStyle(InputStream stream)](#setCustomStyle-java.io.InputStream-) | Disk dosya akışı veya bellek akışı dahil olmak üzere akıştan özel stil dosyasını ayarlar. |
| [setCustomStyleFileName(String value)](#setCustomStyleFileName-java.lang.String-) | Özel stil dosyasının adını ayarlar. |
| [setDPI(double value)](#setDPI-double-) | Makinenin DPI değerini alır/ayarlar. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Denetimin varsayılan yazı tipi adını ayarlar. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | Denetimin varsayılan yazı tipi boyutunu ayarlar. |
| [setDefaultGridLineColor(Color value)](#setDefaultGridLineColor-com.aspose.gridweb.Color-) | Varsayılan ızgara çizgisi rengini ayarlar. |
| [setDisplayCellTip(boolean value)](#setDisplayCellTip-boolean-) | İpuçlarının gösterilip gösterilmeyeceğini ayarlar. Varsayılan değer true'tur. |
| [setEditMode(boolean value)](#setEditMode-boolean-) | Denetimin düzenleme modunu ayarlar. |
| [setEnableAJAX(boolean value)](#setEnableAJAX-boolean-) | AJAX çağrısının kullanılıp kullanılmayacağını ayarlar. Varsayılan değer true'tur. |
| [setEnableAsync(boolean value)](#setEnableAsync-boolean-) | Hücre verilerinin eşzamansız şekilde yüklenip yüklenmeyeceğini ayarlar, 10.000'den fazla hücre içeren bir sayfa için uygulanması önerilir. |
| [setEnableClientColumnOperations(boolean value)](#setEnableClientColumnOperations-boolean-) | İstemci tarafı sütun işlemlerinin etkinleştirilip etkinleştirilmeyeceğini ayarlar. |
| [setEnableClientFreeze(boolean value)](#setEnableClientFreeze-boolean-) | İstemci tarafı dondurma işlemlerinin etkinleştirilip etkinleştirilmeyeceğini ayarlar. |
| [setEnableClientMergeOperations(boolean value)](#setEnableClientMergeOperations-boolean-) | İstemci tarafı birleştirme işlemlerinin etkinleştirilip etkinleştirilmeyeceğini ayarlar. |
| [setEnableClientResizeColumnRow(boolean value)](#setEnableClientResizeColumnRow-boolean-) | İstemci tarafı sütun ve satır yeniden boyutlandırmayı etkinleştirip etkinleştirmeyeceğini ayarlar. |
| [setEnableClientRowOperations(boolean value)](#setEnableClientRowOperations-boolean-) | İstemci tarafı satır işlemlerini etkinleştirip etkinleştirmeyeceğini ayarlar. |
| [setEnableDoubleClickEvent(boolean value)](#setEnableDoubleClickEvent-boolean-) | Müşteri tarafı çift tıklama olayını etkinleştirip etkinleştirmeyeceğini ayarlar. |
| [setEnableMetalLightEffect(boolean value)](#setEnableMetalLightEffect-boolean-) | Metal ışık etkisini uygulayıp uygulamayacağını ayarlar. |
| [setEnablePaging(boolean value)](#setEnablePaging-boolean-) | Denetimin sayfalama modunu etkinleştirip etkinleştirmeyeceğini ayarlar. |
| [setEnableStyleDialogbox(boolean value)](#setEnableStyleDialogbox-boolean-) | İstemci tarafı stil iletişim kutusunu etkinleştirip etkinleştirmeyeceğini ayarlar. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | WebControl içindeki Enabled'ı ayarlar |
| [setFilteredPaging(boolean value)](#setFilteredPaging-boolean-) | Veri filtrelendikten sonra sayfalama özelliğini etkinleştirip etkinleştirmeyeceğini ayarlar; EnablePaging true olduğunda etkili olur. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Yazı tipi klasörünü ayarlar |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Yazı tipleri klasörlerini ayarlar |
| [setForceValidation(boolean value)](#setForceValidation-boolean-) | Müşteri tarafı doğrulamayı zorlayıp zorlamayacağını ayarlar. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | WebControl içindeki ForeColor'ı ayarlar |
| [setFrameTableStyle(GridTableStyle value)](#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-) | Denetimin çerçeve stilini ayarlar. |
| [setGoonDefaultSaveOperation(boolean value)](#setGoonDefaultSaveOperation-boolean-) | GridWeb'in varsayılan kaydetme işlemini yapıp yapmayacağını ayarlar, varsayılan değer true'tır. |
| [setHeaderBarHeight(Unit value)](#setHeaderBarHeight-com.aspose.gridweb.Unit-) | Denetimin üst başlık çubuğunun yüksekliğini (System.Web.UI.WebControl.Unit) ayarlar. |
| [setHeaderBarStyle(GridTableItemStyle value)](#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-) | Başlık çubuğunun stilini ayarlar. |
| [setHeaderBarTableStyle(GridTableStyle value)](#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-) | Denetimin başlık çubuğu stilini ayarlar. |
| [setHeaderBarWidth(Unit value)](#setHeaderBarWidth-com.aspose.gridweb.Unit-) | Denetimin sol başlık çubuğunun genişliğini (System.Web.UI.WebControl.Unit) ayarlar. |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Denetimin yüksekliğini (System.Web.UI.WebControl.Unit) ayarlar. |
| [setIgnoreStyleWithNoData(boolean value)](#setIgnoreStyleWithNoData-boolean-) | GridWeb'in hücre değeri içermeyen ancak stillendirilmiş satır ve sütunları göstermeyi göz ardı edip etmeyeceğini ayarlar. |
| [setLoadOptions(GridLoadOptions value)](#setLoadOptions-com.aspose.gridweb.GridLoadOptions-) | GridWeb için yükleme seçeneklerini temsil eder. |
| [setMaxColumn(int value)](#setMaxColumn-int-) | Web sayfasının maksimum görüntülenen sütun indeksini (sıfır tabanlı) ayarlar. |
| [setMaxRow(int value)](#setMaxRow-int-) | Web sayfasının maksimum görüntülenen satır indeksini (sıfır tabanlı) ayarlar. |
| [setMessage(String value)](#setMessage-java.lang.String-) | Izgara için mesajı ayarlar. |
| [setMinColumn(int value)](#setMinColumn-int-) | Web sayfasının minimum görüntülenen sütun indeksini (sıfır tabanlı) ayarlar. |
| [setMinRow(int value)](#setMinRow-int-) | Web sayfasının minimum görüntülenen satır indeksini (sıfır tabanlı) ayarlar. |
| [setNeedRenderGroupRows(boolean value)](#setNeedRenderGroupRows-boolean-) | Grup satırlarını gösterip göstermeyeceğini ayarlar. |
| [setNoHScroll(boolean value)](#setNoHScroll-boolean-) | Yatay kaydırma çubuğunun gizli olup olmadığını gösteren bir değeri ayarlar. |
| [setNoScroll(boolean value)](#setNoScroll-boolean-) | Kaydırma çubuğunu gösterip göstermeyeceğini ayarlar. |
| [setNoVScroll(boolean value)](#setNoVScroll-boolean-) | Dikey kaydırma çubuğunun gizli olup olmadığını gösteren bir değeri ayarlar. |
| [setOnAjaxCallFinishedClientFunction(String value)](#setOnAjaxCallFinishedClientFunction-java.lang.String-) | ajaxcall tamamlandığında çağrılacak istemci tarafı işlev adını ayarlar. |
| [setOnCellErrorClientFunction(String value)](#setOnCellErrorClientFunction-java.lang.String-) | Bir hücrenin doğrulaması başarısız olduğunda çağrılacak istemci tarafı işlev adını ayarlar. |
| [setOnCellSelectedAjaxCallBackClientFunction(String value)](#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-) | Bir hücre seçildiğinde çağrılacak istemci tarafı işlevi ayarlar. |
| [setOnCellSelectedClientFunction(String value)](#setOnCellSelectedClientFunction-java.lang.String-) | Bir hücre seçildiğinde çağrılacak istemci tarafı işlevi ayarlar. |
| [setOnCellUnselectedClientFunction(String value)](#setOnCellUnselectedClientFunction-java.lang.String-) | Bir hücrenin seçimi kaldırıldığında çağrılacak istemci tarafı işlevi ayarlar. |
| [setOnCellUpdatedClientFunction(String value)](#setOnCellUpdatedClientFunction-java.lang.String-) | Bir hücrenin değeri güncellendiğinde çağrılacak istemci tarafı işlev adını ayarlar. |
| [setOnContextMenuShowClientFunction(String value)](#setOnContextMenuShowClientFunction-java.lang.String-) | Bağlam menüsü gösterildiğinde çağrılacak istemci tarafı işlevi ayarlar. |
| [setOnDoubleClickCellClientFunction(String value)](#setOnDoubleClickCellClientFunction-java.lang.String-) | Bir hücre çift tıklandığında çağrılacak istemci tarafı işlevi ayarlar. |
| [setOnDoubleClickRowClientFunction(String value)](#setOnDoubleClickRowClientFunction-java.lang.String-) | Bir satır çift tıklandığında çağrılacak istemci tarafı işlevi ayarlar. |
| [setOnGridInitClientFunction(String value)](#setOnGridInitClientFunction-java.lang.String-) | Izgara başlatıldığında çağrılacak istemci tarafı işlev adını ayarlar. |
| [setOnPageChangeClientFunction(String value)](#setOnPageChangeClientFunction-java.lang.String-) | Sayfa indeksi değiştikten sonra çağrılacak istemci tarafı işlevi ayarlar. Yalnızca EnablePaging true olduğunda etkili olur. |
| [setOnPageSubmitClientFunction(String value)](#setOnPageSubmitClientFunction-java.lang.String-) | Sayfa istemci tarafında gönderilmeden önce çağrılacak istemci işlevini ayarlar. |
| [setOnShapeSelectedClientFunction(String value)](#setOnShapeSelectedClientFunction-java.lang.String-) | Bir şekil seçildiğinde çağrılacak istemci tarafı işlevi ayarlar. |
| [setOnSubmitClientFunction(String value)](#setOnSubmitClientFunction-java.lang.String-) | Denetim istemci tarafında gönderilmeden önce çağrılacak istemci işlevini ayarlar. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Yüksekliği özelleştirilmemiş satırların yalnızca sığdırılıp sığdırılmayacağını ayarlar, varsayılan değer false'tur. |
| [setPageSize(int value)](#setPageSize-int-) | Sayfalama modunda sayfa boyutunu ayarlar. |
| [setPictureCachePath(String value)](#setPictureCachePath-java.lang.String-) | Çalışma kitabı için görüntü depolama yolunu ayarlar, tüm şekiller ve görüntüler bu dizinde saklanır, varsayılan yol geçerli uygulamanın temel dizini altındaki acwcache'tir; kullanıcıların oturum süresi dışındaki dosyaları temizlemek için bir zamanlayıcı hizmeti uygulamaları gerekir. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Ön ayarlı stili ayarlar. |
| [setRefreshValidation(boolean value)](#setRefreshValidation-boolean-) | Hücre değeri değiştikten sonra doğrulama değerinin yenilenip yenilenmeyeceğini ayarlar. |
| [setRenderHiddenRow(boolean value)](#setRenderHiddenRow-boolean-) | Gizli satırın GridControl içinde render edilip edilmeyeceğini ayarlar, varsayılan değer false'tur. |
| [setRowHeightForCSV(double value)](#setRowHeightForCSV-double-) | CSV dosyası için satır yüksekliği değerini point biriminde ayarlar, varsayılan değer 14.5'tir. |
| [setScrollBarArrowColor(Color value)](#setScrollBarArrowColor-com.aspose.gridweb.Color-) | Kaydırma çubuğunun ok düğmesinin rengini belirtir. |
| [setScrollBarBaseColor(Color value)](#setScrollBarBaseColor-com.aspose.gridweb.Color-) | Denetimin kaydırma çubuğunun rengini belirtir. |
| [setSelectCellBgColor(Color value)](#setSelectCellBgColor-com.aspose.gridweb.Color-) | Çoklu seçim aralığındaki seçili hücrelerin arka plan rengini belirtir. |
| [setSelectCellColor(Color value)](#setSelectCellColor-com.aspose.gridweb.Color-) | Çoklu seçim aralığındaki seçili hücrelerin rengini belirtir. |
| [setSessionStorePath(String value)](#setSessionStorePath-java.lang.String-) | Oturum modu File veya ViewState olduğunda oturum önbellek depolama yolunu ayarlar, örnek: gridweb.SessionStorePath=\"c:/mytempdir/session\"; böylece oturum verileri c:/mytempdir/session içinde saklanır. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridweb.GridWorkbookSettings-) | Çalışma kitabı ayarlarını temsil eder. |
| [setShowAddButton(boolean value)](#setShowAddButton-boolean-) | Çalışma sayfası ekleme düğmesinin gösterilip gösterilmeyeceğini ayarlar. |
| [setShowBottomBar(boolean value)](#setShowBottomBar-boolean-) | Denetimin alt kısmında komut çubuğunun (komut çubuğu ve sekme çubuğu dahil) gösterilip gösterilmeyeceğini belirtir. |
| [setShowCellEditBox(boolean value)](#setShowCellEditBox-boolean-) | Gridweb'in MS-EXCEL gibi düzenleme kutusu araç çubuğunu gösterip göstermediği. Etkinleştirilirse, geçerli hücre için bir düzenleme kutusu Gridweb'de görüntülenir. |
| [setShowCommandBarAtTop(boolean value)](#setShowCommandBarAtTop-boolean-) | Denetimin üst kısmında komut çubuğunun (komut çubuğu ve sekme çubuğu dahil) gösterilip gösterilmeyeceğini belirtir. |
| [setShowContextMenu(boolean value)](#setShowContextMenu-boolean-) | Bağlam menüsünün gösterilip gösterilmeyeceğini ayarlar. Varsayılan değer true'tır. |
| [setShowDefaultGridLine(boolean value)](#setShowDefaultGridLine-boolean-) | Hücrelerin varsayılan ızgara çizgilerinin gösterilip gösterilmeyeceğini ayarlar. |
| [setShowHeaderBar(boolean value)](#setShowHeaderBar-boolean-) | Başlık çubuğunun gösterilip gösterilmeyeceğini ayarlar. |
| [setShowLoading(boolean value)](#setShowLoading-boolean-) | Sunucuya postback yapılırken bir yükleme iletişim kutusunun gösterilip gösterilmeyeceğini belirtir. |
| [setShowLoadingPosition(String value)](#setShowLoadingPosition-java.lang.String-) | Sunucuya postback yapılırken yükleme iletişim kutusunun gösterileceği sol, üst konumunu (px cinsinden) belirtir, vb. 100,200 ifadesi, yükleme iletişim kutusunun sol, üst konumunun 100px,200px olduğu anlamına gelir. |
| [setShowSaveButton(boolean value)](#setShowSaveButton-boolean-) | Kaydet düğmesinin gösterilip gösterilmeyeceğini ayarlar. |
| [setShowSubmitButton(boolean value)](#setShowSubmitButton-boolean-) | Gönder düğmesinin gösterilip gösterilmeyeceğini ayarlar. |
| [setShowTabBar(boolean value)](#setShowTabBar-boolean-) | Sekme çubuğunun gösterilip gösterilmeyeceğini ayarlar. |
| [setShowTabNavigation(boolean value)](#setShowTabNavigation-boolean-) | Sekme gezinme düğmesinin gösterilip gösterilmeyeceğini ayarlar, varsayılan değer true'dur. |
| [setShowUndoButton(boolean value)](#setShowUndoButton-boolean-) | Geri al düğmesinin gösterilip gösterilmeyeceğini ayarlar. |
| [setSpanWrap(boolean value)](#setSpanWrap-boolean-) | İçeriğin hücre aralığında sarılıp sarılmayacağını belirtir, varsayılan değer true'dur. |
| [setTabIndex(short value)](#setTabIndex-short-) | WebControl içindeki TabIndex'i ayarlar |
| [setTabStyle(GridTableItemStyle value)](#setTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Sekme çubuğunun stilini ayarlar. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | WebControl içindeki ToolTip'i ayarlar |
| [setUseClientPageHeight(boolean value)](#setUseClientPageHeight-boolean-) | GridWeb'ün istemci sayfa yüksekliğini kontrol yüksekliği olarak kullanıp kullanmayacağını ayarlar, Height="100%" olarak ayarlandığında uygundur, varsayılan değer false'tur. |
| [setViewPanelScrollLeft(String value)](#setViewPanelScrollLeft-java.lang.String-) | Izgaranın görüntü panelindeki kaydırma çubuğunun konumunu ayarlar. |
| [setViewPanelScrollTop(String value)](#setViewPanelScrollTop-java.lang.String-) | Izgaranın görüntü panelindeki kaydırma çubuğunun konumunu ayarlar. |
| [setViewTableStyle(GridTableStyle value)](#setViewTableStyle-com.aspose.gridweb.GridTableStyle-) | Veri görüntü panelinin stilini ayarlar. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Denetimin genişliğini (System.Web.UI.WebControl.Unit) ayarlar. |
| [setXhtmlMode(boolean value)](#setXhtmlMode-boolean-) | XHTML stilinin kullanılıp kullanılmayacağını ayarlar, varsayılan değer true'dur. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWeb() {#GridWeb--}
```
public GridWeb()
```


### AfterColumnFilter {#AfterColumnFilter}
```
public RowColumnEventHandler AfterColumnFilter
```


Sütun filtrelendikten sonra gerçekleşir.

### AjaxCallFinished {#AjaxCallFinished}
```
public WorkbookEventHandler AjaxCallFinished
```


Denetimin ajax güncellemesi tamamlandığında tetiklenir.(EnableAJAX true olarak ayarlanmalıdır)

### BeforeColumnFilter {#BeforeColumnFilter}
```
public RowColumnEventHandler BeforeColumnFilter
```


Filtrelenecek sütundan önce gerçekleşir.

### CellClickOnAjax {#CellClickOnAjax}
```
public CellEventStringHandler CellClickOnAjax
```


Hücre tıklandığında gerçekleşir ve bu olay için ajaxcallback yapılması gerekir.

### CellClientUpdate {#CellClientUpdate}
```
public CellEventHandler CellClientUpdate
```


Bir istemci hücre güncellemesi gerçekleştiğinde meydana gelir. Bu olay tetiklendiğinde, e.Argument parametresi komutun adını içerir.

### CellCommand {#CellCommand}
```
public CellEventHandler CellCommand
```


Bir hücrenin komut bağlantısına tıklandığında meydana gelir. Bu olay tetiklendiğinde, e.Argument parametresi komutun adını içerir.

### CellDoubleClick {#CellDoubleClick}
```
public CellEventHandler CellDoubleClick
```


Hücre çift tıklandığında gerçekleşir.

### CellModifiedOnAjax {#CellModifiedOnAjax}
```
public CellEventHandler CellModifiedOnAjax
```


Hücre ajax çağrısında değiştirildiğinde gerçekleşir.

### ColumnDeleted {#ColumnDeleted}
```
public RowColumnEventHandler ColumnDeleted
```


Kullanıcı istemci tarafı menüsünden bir sütunu sildiğinde gerçekleşir.

### ColumnDeleting {#ColumnDeleting}
```
public RowColumnEventHandler ColumnDeleting
```


Kullanıcı istemci tarafı menüsünden bir sütunu silmeye çalıştığında meydana gelir. Bu olayı işleyebilir ve iptal parametresini True olarak ayarlayarak silme işlemini iptal edebilirsiniz.

### ColumnDoubleClick {#ColumnDoubleClick}
```
public RowColumnEventHandler ColumnDoubleClick
```


Sütun başlığı çift tıklandığında gerçekleşir.

### ColumnInserted {#ColumnInserted}
```
public RowColumnEventHandler ColumnInserted
```


Kullanıcı istemci tarafı menüsünden bir sütun eklediğinde gerçekleşir.

### CustomCommand {#CustomCommand}
```
public CustomCommandEventHandler CustomCommand
```


Kullanıcı özel bir komut düğmesine tıkladığında gerçekleşir.

### LoadCustomData {#LoadCustomData}
```
public WorkbookEventHandler LoadCustomData
```


Denetimin SessionMode'u Custom olarak ayarlandığında ve sayfa verilerini yüklemesi gerektiğinde tetiklenir. Bu olayı Custom Session modunda dosya veya veritabanından sayfa verilerini yüklemek için işleyebilirsiniz.

### PageIndexChanged {#PageIndexChanged}
```
public WorkbookEventHandler PageIndexChanged
```


Denetimin sayfa dizini değiştiğinde oluşur.

### RowDeleted {#RowDeleted}
```
public RowColumnEventHandler RowDeleted
```


Kullanıcı istemci tarafı menüsünden bir satırı sildiğinde oluşur.

### RowDeleting {#RowDeleting}
```
public RowColumnEventHandler RowDeleting
```


Kullanıcı istemci tarafı menüsünden bir satırı silmeye çalıştığında meydana gelir. Bu olayı işleyebilir ve silme işlemini iptal etmek için bir RejectDeleteException istisnası fırlatabilirsiniz.

### RowDoubleClick {#RowDoubleClick}
```
public RowColumnEventHandler RowDoubleClick
```


Satır başlığı çift tıklandığında oluşur.

### RowInserted {#RowInserted}
```
public RowColumnEventHandler RowInserted
```


Kullanıcı istemci tarafı menüsünden bir satır eklediğinde oluşur.

### SaveCommand {#SaveCommand}
```
public WorkbookEventHandler SaveCommand
```


\"save\" düğmesi tıklandığında oluşur.

### SheetAdded {#SheetAdded}
```
public SheetEventHandler SheetAdded
```


Kullanıcı araç çubuğu menüsünden bir çalışma sayfası eklediğinde oluşur.

### SheetTabClick {#SheetTabClick}
```
public WorkbookEventHandler SheetTabClick
```


Sayfa sekmesi tıklandığında oluşur.

### SubmitCommand {#SubmitCommand}
```
public WorkbookEventHandler SubmitCommand
```


\"submit\" düğmesi tıklandığında oluşur.

### UndoCommand {#UndoCommand}
```
public WorkbookEventHandler UndoCommand
```


\"undo\" düğmesi tıklandığında oluşur.

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Formüllerin sonucunu hesaplar.

### createChildControls() {#createChildControls--}
```
public void createChildControls()
```


WebControl'dan CreateChildControls uygular, yalnızca dahili kullanım içindir.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getACWClientPath() {#getACWClientPath--}
```
public String getACWClientPath()
```


Denetimin script/görsel dosyalarının web yolunu alır. Örneğin: "http://localhost/acw\_client". Bu değeri web.config dosyasında da ayarlayabilirsiniz. Bu bölümü `<configuration>` bölümüne ekleyin:
`<appSettings>`
`<add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" />`
`</appSettings>`


**Returns:**
java.lang.String
### getACWLanguageFileUrl() {#getACWLanguageFileUrl--}
```
public String getACWLanguageFileUrl()
```


Denetimin dil dosyasının web URL'sini alır. Örneğin: "/acw\_client/lang\_en.js".
Varsayılan olarak, yerleşik bir İngilizce dosya kullanılır.


**Returns:**
java.lang.String
### getActiveCell() {#getActiveCell--}
```
public GridCell getActiveCell()
```


Mevcut sayfanın aktif hücresini alır. 1.9.0.1 sürümünden beri yazılabilir olarak değiştirildi.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getActiveCellBgColor() {#getActiveCellBgColor--}
```
public Color getActiveCellBgColor()
```


Etkin hücrenin arka plan rengini belirtir.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveCellColor() {#getActiveCellColor--}
```
public Color getActiveCellColor()
```


Etkin hücrenin rengini belirtir.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderBgColor() {#getActiveHeaderBgColor--}
```
public Color getActiveHeaderBgColor()
```


Etkin satır/sütun başlığının arka plan rengini belirtir.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderColor() {#getActiveHeaderColor--}
```
public Color getActiveHeaderColor()
```


Etkin satır/sütun başlığının rengini belirtir.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveSheet() {#getActiveSheet--}
```
public GridWorksheet getActiveSheet()
```


Etkin sayfayı alır

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Aktif sayfa indeksini alır. WebWorksheets.ActiveSheetIndex'e eşittir.

**Returns:**
int
### getActiveTabStyle() {#getActiveTabStyle--}
```
public GridTableItemStyle getActiveTabStyle()
```


Etkin sekmenin stilini belirtir.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getAutoRefreshChart() {#getAutoRefreshChart--}
```
public boolean getAutoRefreshChart()
```


Hücre değerini güncellerken Grafik görüntüsünün güncellenip güncellenmediğini alır. Varsayılan değer true'tur.

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


WebControl içinde BackColor'i alır

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


WebControl içinde BorderColor'i alır

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


WebControl içinde BorderStyle'i alır

Bakınız [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


WebControl içinde BorderWidth'i alır

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomTableStyle() {#getBottomTableStyle--}
```
public GridTableStyle getBottomTableStyle()
```


Denetimin alt çubuğunun stilini alır.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```


WebControl içindeki CssClass'i alır

**Returns:**
java.lang.String
### getCurrentPageIndex() {#getCurrentPageIndex--}
```
public int getCurrentPageIndex()
```


Sayfalama modunda geçerli sayfa dizinini alır.

**Remarks**

Sayfalama modundayken, kontrol bir kez PageSize satır veri gösterir ve sekme çubuğunda sayfa seçme kontrolünü gösterir.

**Returns:**
int
### getCustomCalculationEngine() {#getCustomCalculationEngine--}
```
public GridAbstractCalculationEngine getCustomCalculationEngine()
```


Kullanıcının, Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel hesaplama motorunu temsil eder.

**Returns:**
[GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine)
### getCustomCommandButtons() {#getCustomCommandButtons--}
```
public CustomCommandButtonCollection getCustomCommandButtons()
```


Özel komut düğmesi koleksiyonunu alır

**Returns:**
[CustomCommandButtonCollection](../../com.aspose.gridweb/customcommandbuttoncollection)
### getCustomStyleFileName() {#getCustomStyleFileName--}
```
public String getCustomStyleFileName()
```


Özel stil dosya adını alır.

**Remarks**

Özel stil dosyası bir XML dosyasıdır. Dosya adı ayarlandığında, dosya hemen yüklenecektir. İşte "standard preset style" içeriği ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Example**

```
         		GridWeb1.setCustomStyleFileName("c:\\style\\mystyle.xml");
```

**Returns:**
java.lang.String
### getDPI() {#getDPI--}
```
public static double getDPI()
```


Makinenin DPI değerini alır/ayarlar.

**Remarks**

**Returns:**
double
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Denetimin varsayılan yazı tipi adını alır.

**Example**

```
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


Denetimin varsayılan yazı tipi boyutunu alır.

**Example**

```
         		GridWeb1.setDefaultFontSize(new FontUnit("10pt"));
```

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getDefaultGridLineColor() {#getDefaultGridLineColor--}
```
public Color getDefaultGridLineColor()
```


Varsayılan ızgara çizgisinin rengini alır.

**Example**

```
         		GridWeb1.setDefaultGridLineColor(Color.getRed());
```

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getDisplayCellTip() {#getDisplayCellTip--}
```
public boolean getDisplayCellTip()
```


İpuçlarının gösterilip gösterilmeyeceğini alır. Varsayılan değer doğrudur.

**Returns:**
boolean
### getEditMode() {#getEditMode--}
```
public boolean getEditMode()
```


Denetimin düzenleme modunu alır.

**Remarks**

True olarak ayarlandığında, kontrolün hücreleri düzenlenebilir ve "save" ve "undo" simgeleri gösterilir. False olarak ayarlandığında, kontrolün hücreleri yalnızca okunur olur ve "save" ve "undo" simgeleri gösterilmez.

**Returns:**
boolean
### getEnableAJAX() {#getEnableAJAX--}
```
public boolean getEnableAJAX()
```


AJAX çağrısının kullanılıp kullanılmayacağını alır. Varsayılan değer doğrudur.

**Returns:**
boolean
### getEnableAsync() {#getEnableAsync--}
```
public boolean getEnableAsync()
```


Hücre verilerinin asenkron şekilde yüklenip yüklenmeyeceğini alır, 10.000'den fazla hücre içeren bir sayfa için uygulanması önerilir.

**Returns:**
boolean
### getEnableClientColumnOperations() {#getEnableClientColumnOperations--}
```
public boolean getEnableClientColumnOperations()
```


İstemci tarafı sütun işlemlerinin etkinleştirilip etkinleştirilmeyeceğini alır.

**Remarks**

True olarak ayarlandığında, kullanıcı sağ tıklama menüsünü kullanarak sütun ekleyebilir/kaldırabilir.

**Returns:**
boolean
### getEnableClientFreeze() {#getEnableClientFreeze--}
```
public boolean getEnableClientFreeze()
```


İstemci tarafı dondurma işlemlerinin etkinleştirilip etkinleştirilmeyeceğini alır.

**Remarks**

True olarak ayarlandığında, kullanıcı sağ tıklama menüsünü kullanarak bölmeleri dondurabilir/birleştirme dondurmasını kaldırabilir.

**Returns:**
boolean
### getEnableClientMergeOperations() {#getEnableClientMergeOperations--}
```
public boolean getEnableClientMergeOperations()
```


İstemci tarafı birleştirme işlemlerinin etkinleştirilip etkinleştirilmeyeceğini alır.

**Remarks**

True olarak ayarlandığında, kullanıcı sağ tıklama menüsünü kullanarak hücreleri birleştirebilir/birleştirmeyi kaldırabilir.

**Returns:**
boolean
### getEnableClientResizeColumnRow() {#getEnableClientResizeColumnRow--}
```
public boolean getEnableClientResizeColumnRow()
```


İstemci tarafı sütun ve satır yeniden boyutlandırmanın etkinleştirilip etkinleştirilmeyeceğini alır.

**Remarks**

True olarak ayarlandığında, kullanıcı istemci tarafında sütun ve satırı yeniden boyutlandırabilir.

**Returns:**
boolean
### getEnableClientRowOperations() {#getEnableClientRowOperations--}
```
public boolean getEnableClientRowOperations()
```


İstemci tarafı satır işlemlerinin etkinleştirilip etkinleştirilmeyeceğini alır.

**Remarks**

True olarak ayarlandığında, kullanıcı sağ tıklama menüsünü kullanarak satır ekleyebilir/kaldırabilir.

**Returns:**
boolean
### getEnableDoubleClickEvent() {#getEnableDoubleClickEvent--}
```
public boolean getEnableDoubleClickEvent()
```


Müşteri tarafı çift tıklama olayının etkinleştirilip etkinleştirilmeyeceğini alır.

**Remarks**

True olarak ayarlandığında, kontrol müşteri tarafı çift tıklama olaylarını alır ve bu olayları sunucu tarafında işleyebilirsiniz. Aksi takdirde kontrol herhangi bir çift tıklama olayını yok sayar.

**Returns:**
boolean
### getEnableMetalLightEffect() {#getEnableMetalLightEffect--}
```
public boolean getEnableMetalLightEffect()
```


Metal ışık etkisinin uygulanıp uygulanmayacağını alır.

**Returns:**
boolean
### getEnablePaging() {#getEnablePaging--}
```
public boolean getEnablePaging()
```


Denetimin sayfalama modunun etkinleştirilip etkinleştirilmeyeceğini alır.

**Remarks**

True olarak ayarlandığında, kontrol bir kez PageSize satır veri gösterir ve sekme çubuğunda sayfa seçme kontrolünü gösterir.

**Returns:**
boolean
### getEnableStyleDialogbox() {#getEnableStyleDialogbox--}
```
public boolean getEnableStyleDialogbox()
```


İstemci tarafı stil iletişim kutusunun etkinleştirilip etkinleştirilmeyeceğini alır.

**Remarks**

True olarak ayarlandığında, kullanıcı açılır menüden "Format Cell..." seçerek bir hücrenin stilini ayarlamak için stil iletişim kutusunu kullanabilir.

**Returns:**
boolean
### getEnabled() {#getEnabled--}
```
public boolean getEnabled()
```


WebControl içindeki Enabled'ı alır

**Returns:**
boolean
### getFilteredPaging() {#getFilteredPaging--}
```
public boolean getFilteredPaging()
```


Veri filtrelendikten sonra sayfalamanın etkinleştirilip etkinleştirilmeyeceğini alır, EnablePaging true olduğunda etkili olur.

**Remarks**

True olarak ayarlandığında, kontrol filtrelenmiş verilere göre sayfalama yapar, varsayılan değer false'tur.

**Returns:**
boolean
### getFont() {#getFont--}
```
public FontInfo getFont()
```


WebControl içindeki Font'u alır

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForceValidation() {#getForceValidation--}
```
public boolean getForceValidation()
```


Müşteri tarafı doğrulamanın zorunlu olup olmadığını alır.

**Remarks**

True olarak ayarlandığında, tüm giriş alanları geçerli olana kadar veri sunucuya gönderilmez.

**Returns:**
boolean
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


WebControl içindeki ForeColor'ı alır

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getFrameTableStyle() {#getFrameTableStyle--}
```
public GridTableStyle getFrameTableStyle()
```


Denetimin çerçeve stilini alır.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getGoonDefaultSaveOperation() {#getGoonDefaultSaveOperation--}
```
public boolean getGoonDefaultSaveOperation()
```


GridWeb'in varsayılan kaydetme işlemini yapıp yapmayacağını alır, varsayılan değer doğrudur.

**Returns:**
boolean
### getHeaderBarHeight() {#getHeaderBarHeight--}
```
public Unit getHeaderBarHeight()
```


Denetimin üst başlık çubuğunun yüksekliğini (System.Web.UI.WebControl.Unit) alır.

**Example**

```
         		GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeaderBarStyle() {#getHeaderBarStyle--}
```
public GridTableItemStyle getHeaderBarStyle()
```


Başlık çubuğunun stilini alır.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getHeaderBarTableStyle() {#getHeaderBarTableStyle--}
```
public GridTableStyle getHeaderBarTableStyle()
```


Denetimin başlık çubuğu stilini alır.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getHeaderBarWidth() {#getHeaderBarWidth--}
```
public Unit getHeaderBarWidth()
```


Denetimin genişliğini (System.Web.UI.WebControl.Unit) veya sol başlık çubuğunu alır.

**Example**

```
         		GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


Denetimin yüksekliğini (System.Web.UI.WebControl.Unit) alır.

**Example**

```
         		GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getIgnoreStyleWithNoData() {#getIgnoreStyleWithNoData--}
```
public boolean getIgnoreStyleWithNoData()
```


GridWeb'in hücre değeri içermeyen ancak stillendirilmiş satır veya sütunları göstermeyi görmezden gelip gelmediğini alır. True olarak ayarlandığında performans daha iyi olur. Varsayılan değer false'tur; bu, son ardışık satır/sütunun hücre değeri olmasa da stillendirilmişse yine de gösterileceği anlamına gelir. Bu seçenek yalnızca EnableAsync false olduğunda geçerlidir. EnableAsync true olduğunda bu seçeneğin etkisi yoktur; bu da GridWeb'in tüm satır/sütunları stil ile göstereceği anlamına gelir.

**Returns:**
boolean
### getLoadOptions() {#getLoadOptions--}
```
public GridLoadOptions getLoadOptions()
```


GridWeb için yükleme seçeneklerini temsil eder.

**Returns:**
[GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Web sayfasının maksimum görüntülenen sütun indeksini (sıfır tabanlı) alır. Kontrol, MaxColumn ve sayfa verisinin maksimum sütun değerinden büyük olanı kullanır.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Web sayfasının maksimum görüntülenen satır indeksini (sıfır tabanlı) alır. Kontrol, MaxRow ve sayfa verisinin maksimum satır değerinden büyük olanı kullanır.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMessage() {#getMessage--}
```
public String getMessage()
```


Izgara için mesajı alır.

**Returns:**
java.lang.String
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Web sayfasının minimum görüntülenen sütun indeksini (sıfır tabanlı) alır. Kontrol, MinColumn ve sayfa verisinin minimum sütun değerinden küçük olanı kullanır.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Web sayfasının minimum görüntülenen satır indeksini (sıfır tabanlı) alır. Kontrol, MinRow ve sayfa verisinin minimum satır değerinden küçük olanı kullanır.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getModifiedCells() {#getModifiedCells--}
```
public ArrayList getModifiedCells()
```


İstemci tarafından değiştirilen hücrelerin koleksiyonunu alır.

**Returns:**
java.util.ArrayList
### getNeedRenderGroupRows() {#getNeedRenderGroupRows--}
```
public boolean getNeedRenderGroupRows()
```


Grup satırlarının gösterilip gösterilmeyeceğini alır.

**Returns:**
boolean
### getNoHScroll() {#getNoHScroll--}
```
public boolean getNoHScroll()
```


Yatay kaydırma çubuğunun gizli olup olmadığını belirten bir değeri alır.

**Returns:**
boolean
### getNoScroll() {#getNoScroll--}
```
public boolean getNoScroll()
```


Kaydırma çubuğunun gösterilip gösterilmeyeceğini alır.

**Returns:**
boolean
### getNoVScroll() {#getNoVScroll--}
```
public boolean getNoVScroll()
```


Dikey kaydırma çubuğunun gizli olup olmadığını belirten bir değeri alır.

**Returns:**
boolean
### getOnAjaxCallFinishedClientFunction() {#getOnAjaxCallFinishedClientFunction--}
```
public String getOnAjaxCallFinishedClientFunction()
```


Ajax çağrısı tamamlandığında çağrılacak istemci tarafı fonksiyon adını alır. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnCellErrorClientFunction() {#getOnCellErrorClientFunction--}
```
public String getOnCellErrorClientFunction()
```


Bir hücrenin doğrulaması başarısız olduğunda çağrılacak istemci tarafı fonksiyon adını alır. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnCellSelectedAjaxCallBackClientFunction() {#getOnCellSelectedAjaxCallBackClientFunction--}
```
public String getOnCellSelectedAjaxCallBackClientFunction()
```


Bir hücre seçildiğinde çağrılacak istemci tarafı işlevi alır. İstemci işlevi şu şekilde tanımlanmalıdır:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnCellSelectedClientFunction() {#getOnCellSelectedClientFunction--}
```
public String getOnCellSelectedClientFunction()
```


Bir hücre seçildiğinde çağrılacak istemci tarafı işlevi alır. İstemci işlevi şu şekilde tanımlanmalıdır:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, \"test\");
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnCellUnselectedClientFunction() {#getOnCellUnselectedClientFunction--}
```
public String getOnCellUnselectedClientFunction()
```


Bir hücre seçimi kaldırıldığında çağrılacak istemci tarafı işlevi alır. İstemci işlevi şu şekilde tanımlanmalıdır:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, \"test\");
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnCellUpdatedClientFunction() {#getOnCellUpdatedClientFunction--}
```
public String getOnCellUpdatedClientFunction()
```


Bir hücrenin değeri güncellendiğinde çağrılacak istemci tarafı işlev adını alır. İstemci işlevi şu şekilde tanımlanmalıdır:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnContextMenuShowClientFunction() {#getOnContextMenuShowClientFunction--}
```
public String getOnContextMenuShowClientFunction()
```


Bağlam menüsü gösterildiğinde çağrılacak istemci tarafı işlevi alır. İstemci işlevi şu şekilde tanımlanmalıdır:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility(\"Delete\", \"block\");
menu.setItemVisibility(\"Update\", \"none\");
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnDoubleClickCellClientFunction() {#getOnDoubleClickCellClientFunction--}
```
public String getOnDoubleClickCellClientFunction()
```


Bir hücre çift tıklandığında çağrılacak istemci tarafı işlevi alır. İstemci işlevi şu şekilde tanımlanmalıdır:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, \"test\");
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnDoubleClickRowClientFunction() {#getOnDoubleClickRowClientFunction--}
```
public String getOnDoubleClickRowClientFunction()
```


Bir satır çift tıklandığında çağrılacak istemci tarafı işlevi alır. İstemci işlevi şu şekilde tanımlanmalıdır:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnGridInitClientFunction() {#getOnGridInitClientFunction--}
```
public String getOnGridInitClientFunction()
```


Izgara başlatıldığında çağrılacak istemci tarafı işlev adını alır. İstemci işlevi şu şekilde tanımlanmalıdır:
function MyOnGridInit(grid)
\{
alert(\"The grid is initialized: \" + grid.id);
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnPageChangeClientFunction() {#getOnPageChangeClientFunction--}
```
public String getOnPageChangeClientFunction()
```


Sayfa indeksi değiştikten sonra çağrılacak istemci tarafı işlevi alır. Yalnızca EnablePaging true olduğunda etkili olur. İstemci işlevi şu şekilde tanımlanmalıdır:
function MyOnPageChange(index)
\{
console.log(\"current page is:\"+index);
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnPageSubmitClientFunction() {#getOnPageSubmitClientFunction--}
```
public String getOnPageSubmitClientFunction()
```


Sayfa istemci tarafında gönderilmeden önce çağrılacak istemci fonksiyonunu alır.

**Returns:**
java.lang.String
### getOnShapeSelectedClientFunction() {#getOnShapeSelectedClientFunction--}
```
public String getOnShapeSelectedClientFunction()
```


Bir şekil seçildiğinde çağrılacak istemci tarafı işlevi alır. İstemci işlevi şu şekilde tanımlanmalıdır:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnSubmitClientFunction() {#getOnSubmitClientFunction--}
```
public String getOnSubmitClientFunction()
```


Denetim istemci tarafında gönderilmeden önce çağrılacak istemci işlevini alır. İstemci işlevi şu şekilde tanımlanmalıdır:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
arg, sunucuya gönderilecek komutu içeren gönderim argümanıdır. cancelEdit, denetimin gönderimden önce kullanıcı girişini iptal edip etmediğini gösteren boolean bir değerdir. Fonksiyon true döndürürse denetim gönderime devam eder.
Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Returns:**
java.lang.String
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Yüksekliği özelleştirilmemiş satırların yalnızca sığdırılıp sığdırılmayacağını alır, varsayılan değer false'tur.

**Returns:**
boolean
### getPageSize() {#getPageSize--}
```
public int getPageSize()
```


Sayfalama modundaki sayfa boyutunu alır.

**Remarks**

Sayfalama modundayken, kontrol bir kez PageSize satır veri gösterir ve sekme çubuğunda sayfa seçme kontrolünü gösterir.

**Returns:**
int
### getPictureCachePath() {#getPictureCachePath--}
```
public static String getPictureCachePath()
```


Çalışma kitabı için görüntü depolama yolunu alır, tüm şekiller ve görüntüler bu dizinde saklanır, varsayılan yol geçerli uygulamanın temel dizini altındaki acwcache'tir, kullanıcıların oturum süresi dışındaki dosyaları temizlemek için bir zamanlama hizmeti uygulamaları gerekir.

**Returns:**
java.lang.String
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Ön ayarlı stili alır.

[PresetStyle](../../com.aspose.gridweb/presetstyle) sayfasına bakın.

**Example**

```
         		GridWeb1.setPresetStyle(PresetStyle.TRADITIONAL_1);
```

**Returns:**
int
### getRefreshValidation() {#getRefreshValidation--}
```
public boolean getRefreshValidation()
```


Hücre değeri değiştikten sonra doğrulama değerinin yenilenip yenilenmeyeceğini alır.

**Returns:**
boolean
### getRenderHiddenRow() {#getRenderHiddenRow--}
```
public boolean getRenderHiddenRow()
```


Gizli satırın GridControl içinde render edilip edilmediğini alır, varsayılan değer false'tur. Daha sonra gizli satırı göstermek isterseniz, true olarak ayarlamalısınız.

**Returns:**
boolean
### getRowHeightForCSV() {#getRowHeightForCSV--}
```
public double getRowHeightForCSV()
```


CSV dosyası için satır yüksekliği değerini puan cinsinden alır, varsayılan değer 14.5'tir.

**Returns:**
double
### getScrollBarArrowColor() {#getScrollBarArrowColor--}
```
public Color getScrollBarArrowColor()
```


Kaydırma çubuğunun ok düğmesinin rengini belirtir.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getScrollBarBaseColor() {#getScrollBarBaseColor--}
```
public Color getScrollBarBaseColor()
```


Denetimin kaydırma çubuğunun rengini belirtir.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellBgColor() {#getSelectCellBgColor--}
```
public Color getSelectCellBgColor()
```


Çoklu seçim aralığındaki seçili hücrelerin arka plan rengini belirtir.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellColor() {#getSelectCellColor--}
```
public Color getSelectCellColor()
```


Çoklu seçim aralığındaki seçili hücrelerin rengini belirtir.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCells() {#getSelectCells--}
```
public ArrayList getSelectCells()
```


Seçili hücre koleksiyonunu alır.

**Returns:**
java.util.ArrayList
### getSessionStorePath() {#getSessionStorePath--}
```
public String getSessionStorePath()
```


Oturum modu File veya ViewState olduğunda oturum önbellek depolama yolunu alır, örnek: gridweb.SessionStorePath="c:/mytempdir/session"; ardından oturum verileri c:/mytempdir/session içinde saklanır.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Çalışma kitabı ayarlarını temsil eder.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings)
### getShowAddButton() {#getShowAddButton--}
```
public boolean getShowAddButton()
```


Çalışma sayfası ekleme düğmesinin gösterilip gösterilmeyeceğini alır.

**Returns:**
boolean
### getShowBottomBar() {#getShowBottomBar--}
```
public boolean getShowBottomBar()
```


Denetimin alt kısmında komut çubuğunun (komut çubuğu ve sekme çubuğu dahil) gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getShowCellEditBox() {#getShowCellEditBox--}
```
public boolean getShowCellEditBox()
```


Gridweb'in MS-EXCEL'deki gibi düzenleme kutusu araç çubuğunu gösterip göstermediği. Etkinleştirilirse, mevcut hücre için bir düzenleme kutusu Gridweb'te görüntülenir. Bu özelliği etkinleştirirsek, yeni özelliği desteklemek için aspx dosyalarınıza jquery js kütüphanesini eklemeniz gerekir. En son jquery sürümleri uygundur, vb.

**Returns:**
boolean
### getShowCommandBarAtTop() {#getShowCommandBarAtTop--}
```
public boolean getShowCommandBarAtTop()
```


Denetimin üst kısmında komut çubuğunun (komut çubuğu ve sekme çubuğu dahil) gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getShowContextMenu() {#getShowContextMenu--}
```
public boolean getShowContextMenu()
```


Bağlam menüsünün gösterilip gösterilmeyeceğini alır. Varsayılan değer true'tur.

**Returns:**
boolean
### getShowDefaultGridLine() {#getShowDefaultGridLine--}
```
public boolean getShowDefaultGridLine()
```


Hücrelerin varsayılan ızgara çizgilerinin gösterilip gösterilmeyeceğini alır.

**Returns:**
boolean
### getShowHeaderBar() {#getShowHeaderBar--}
```
public boolean getShowHeaderBar()
```


Başlık çubuğunun gösterilip gösterilmeyeceğini alır.

**Returns:**
boolean
### getShowLoading() {#getShowLoading--}
```
public boolean getShowLoading()
```


Sunucuya postback yapılırken bir yükleme iletişim kutusunun gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getShowLoadingPosition() {#getShowLoadingPosition--}
```
public String getShowLoadingPosition()
```


Sunucuya postback yapılırken yükleme iletişim kutusunun gösterileceği sol, üst konumunu (px cinsinden) belirtir, vb. 100,200 ifadesi, yükleme iletişim kutusunun sol, üst konumunun 100px,200px olduğu anlamına gelir.

**Returns:**
java.lang.String
### getShowSaveButton() {#getShowSaveButton--}
```
public boolean getShowSaveButton()
```


Kaydet düğmesinin gösterilip gösterilmeyeceğini alır.

**Returns:**
boolean
### getShowSubmitButton() {#getShowSubmitButton--}
```
public boolean getShowSubmitButton()
```


Gönder düğmesinin gösterilip gösterilmeyeceğini alır.

**Returns:**
boolean
### getShowTabBar() {#getShowTabBar--}
```
public boolean getShowTabBar()
```


Sekme çubuğunun gösterilip gösterilmeyeceğini alır.

**Returns:**
boolean
### getShowTabNavigation() {#getShowTabNavigation--}
```
public boolean getShowTabNavigation()
```


Sekme gezinme düğmesinin gösterilip gösterilmeyeceğini alır, varsayılan değer true'dur.

**Returns:**
boolean
### getShowUndoButton() {#getShowUndoButton--}
```
public boolean getShowUndoButton()
```


Geri al düğmesinin gösterilip gösterilmeyeceğini alır.

**Returns:**
boolean
### getSpanWrap() {#getSpanWrap--}
```
public boolean getSpanWrap()
```


İçeriğin hücre aralığında sarılıp sarılmayacağını belirtir, varsayılan değer true'dur.

**Returns:**
boolean
### getTabIndex() {#getTabIndex--}
```
public short getTabIndex()
```


WebControl içindeki TabIndex'i alır

**Returns:**
short
### getTabStyle() {#getTabStyle--}
```
public GridTableItemStyle getTabStyle()
```


Sekme çubuğunun stilini alır.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


WebControl içindeki ToolTip'i alır

**Returns:**
java.lang.String
### getUseClientPageHeight() {#getUseClientPageHeight--}
```
public boolean getUseClientPageHeight()
```


GridWeb'ün istemci sayfa yüksekliğini kontrol yüksekliği olarak kullanıp kullanmayacağını alır, Height=\"100%\" ayarlandığında uygundur, varsayılan değer false'tur.

**Returns:**
boolean
### getVersion() {#getVersion--}
```
public static String getVersion()
```


Sürüm numarasını al.

**Returns:**
java.lang.String - Yayın sürümü.
### getViewPanelScrollLeft() {#getViewPanelScrollLeft--}
```
public String getViewPanelScrollLeft()
```


Izgaranın görünüm panelindeki kaydırma çubuğunun konumunu alır.

**Returns:**
java.lang.String
### getViewPanelScrollTop() {#getViewPanelScrollTop--}
```
public String getViewPanelScrollTop()
```


Izgaranın görünüm panelindeki kaydırma çubuğunun konumunu alır.

**Returns:**
java.lang.String
### getViewTableStyle() {#getViewTableStyle--}
```
public GridTableStyle getViewTableStyle()
```


Veri görünüm panelinin stilini alır.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Denetimin genişliğini (System.Web.UI.WebControl.Unit) alır.

**Example**

```
         		GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWorkSheets() {#getWorkSheets--}
```
public GridWorksheetCollection getWorkSheets()
```


Çalışma sayfalarının koleksiyonunu alır.

**Returns:**
[GridWorksheetCollection](../../com.aspose.gridweb/gridworksheetcollection)
### getXhtmlMode() {#getXhtmlMode--}
```
public boolean getXhtmlMode()
```


XHTML stilinin kullanılıp kullanılmayacağını alır, varsayılan değer true'dur.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream stream) {#importExcelFile-java.io.InputStream-}
```
public void importExcelFile(InputStream stream)
```


Disk dosyası akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışından içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Excel dosyasının akışı, disk dosyası akışı veya bellek akışı dahil. |

### importExcelFile(InputStream stream, String passwordtoOpen) {#importExcelFile-java.io.InputStream-java.lang.String-}
```
public void importExcelFile(InputStream stream, String passwordtoOpen)
```


Disk dosyası akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışından içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Excel dosyasının akışı, disk dosyası akışı veya bellek akışı dahil. |
| passwordtoOpen | java.lang.String | Şifrelenmiş dosyanın açma şifresi. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Bir Excel dosyasından içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Excel dosyasının adı. |

### importExcelFile(String fileName, String passwordtoOpen) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String fileName, String passwordtoOpen)
```


Bir Excel dosyasından içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Excel dosyasının adı. |
| passwordtoOpen | java.lang.String | Şifrelenmiş dosyanın açma şifresi. |

### isCalculateFormula() {#isCalculateFormula--}
```
public boolean isCalculateFormula()
```


Hücre değeri değiştikten sonra veya dosya içe aktarıldıktan sonra formülün hesaplanıp hesaplanmayacağını alır. Varsayılan değer true'tur.

**Returns:**
boolean
### loadCSVFile(InputStream stream) {#loadCSVFile-java.io.InputStream-}
```
public void loadCSVFile(InputStream stream)
```


CSV dosyası akışından verileri yükler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Dosya akışı. |

### loadCSVFile(String fileName) {#loadCSVFile-java.lang.String-}
```
public void loadCSVFile(String fileName)
```


CSV dosyasından verileri yükler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Dosyanın adı. |

### loadHTMLFile(InputStream stream) {#loadHTMLFile-java.io.InputStream-}
```
public void loadHTMLFile(InputStream stream)
```


HTML dosyası akışından verileri yükler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Dosya akışı. |

### loadHTMLFile(String fileName) {#loadHTMLFile-java.lang.String-}
```
public void loadHTMLFile(String fileName)
```


HTML dosyasından verileri yükler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Dosyanın adı. |

### loadSpreadSheetMLFile(InputStream stream) {#loadSpreadSheetMLFile-java.io.InputStream-}
```
public void loadSpreadSheetMLFile(InputStream stream)
```


SpreadSheetML dosyası akışından verileri yükler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Dosyanın akışı. |

### loadSpreadSheetMLFile(String fileName) {#loadSpreadSheetMLFile-java.lang.String-}
```
public void loadSpreadSheetMLFile(String fileName)
```


SpreadSheetML dosyasından verileri yükler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Dosyanın adı. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshChartShape() {#refreshChartShape--}
```
public void refreshChartShape()
```


Etkin çalışma sayfası için tüm grafik görüntülerini yeniler.

### saveCSVFile(OutputStream stream) {#saveCSVFile-java.io.OutputStream-}
```
public void saveCSVFile(OutputStream stream)
```


Verileri CSV dosyası akışına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Dosya akışı. |

### saveCSVFile(String targetFile) {#saveCSVFile-java.lang.String-}
```
public void saveCSVFile(String targetFile)
```


Verileri CSV dosyasına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| targetFile | java.lang.String | Dosyanın adı. |

### saveCustomStyleFile(String fileName) {#saveCustomStyleFile-java.lang.String-}
```
public void saveCustomStyleFile(String fileName)
```


Denetimin mevcut stil verilerini bir xml dosyasına kaydeder. Özelleştirilmiş stil dosyanızı oluşturmak için kullanılabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Stil dosyasının adı. |

### saveHTMLFile(OutputStream stream) {#saveHTMLFile-java.io.OutputStream-}
```
public void saveHTMLFile(OutputStream stream)
```


Verileri bir HTML dosya akışına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Dosya akışı. |

### saveHTMLFile(String targetFile) {#saveHTMLFile-java.lang.String-}
```
public void saveHTMLFile(String targetFile)
```


Verileri bir HTML dosyasına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| targetFile | java.lang.String | Dosyanın adı. |

### saveSpreadSheetMLFile(OutputStream stream) {#saveSpreadSheetMLFile-java.io.OutputStream-}
```
public void saveSpreadSheetMLFile(OutputStream stream)
```


Verileri bir SpreadSheetML dosya akışına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Dosya akışı. |

### saveSpreadSheetMLFile(String targetFile) {#saveSpreadSheetMLFile-java.lang.String-}
```
public void saveSpreadSheetMLFile(String targetFile)
```


Verileri bir SpreadSheetML dosyasına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| targetFile | java.lang.String | Dosyanın adı. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Çalışma sayfalarını bir Excel dosyasına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Yazılacak akış. |

### saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions) {#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)
```


Çalışma sayfalarını bir Excel dosyasına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Yazılacak akış. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Kaydetme seçenekleri. |

### saveToExcelFile(OutputStream stream, int format) {#saveToExcelFile-java.io.OutputStream-int-}
```
public void saveToExcelFile(OutputStream stream, int format)
```


Çalışma sayfalarını bir Excel dosyasına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Yazılacak akış. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Dosya formatı (Excel2003, Excel2007, CSV, SpreadsheetML) |

### saveToExcelFile(String targetFile) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String targetFile)
```


Çalışma sayfalarını Excel 2003 formatında bir Excel dosyasına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| targetFile | java.lang.String | Yazılacak hedef dosyanın adı. |

### saveToExcelFile(String targetFile, GridSaveOptions saveOptions) {#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(String targetFile, GridSaveOptions saveOptions)
```


Çalışma sayfalarını bir Excel dosyasına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| targetFile | java.lang.String | Yazılacak hedef dosyanın adı. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Kaydetme seçenekleri. |

### saveToExcelFile(String targetFile, int format) {#saveToExcelFile-java.lang.String-int-}
```
public void saveToExcelFile(String targetFile, int format)
```


Çalışma sayfalarını bir Excel dosyasına kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| targetFile | java.lang.String | Yazılacak hedef dosyanın adı. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Dosya formatı (Excel2003, Excel2007, CSV, SpreadsheetML) |

### setACWClientPath(String value) {#setACWClientPath-java.lang.String-}
```
public void setACWClientPath(String value)
```


Denetimin script/görsel dosyalarının web yolunu ayarlar. Örneğin: "http://localhost/acw\_client". Bu değeri ayrıca web.config dosyasında da ayarlayabilirsiniz. Bu bölümü `<configuration>` bölümüne ekleyin:
`<appSettings>`
`<add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" />`
`</appSettings>`


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setACWLanguageFileUrl(String value) {#setACWLanguageFileUrl-java.lang.String-}
```
public void setACWLanguageFileUrl(String value)
```


Denetimin dil dosyasının web URL'sini ayarlar. Örneğin: "/acw\_client/lang\_en.js".
Varsayılan olarak, yerleşik bir İngilizce dosya kullanılır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setActiveCell(GridCell value) {#setActiveCell-com.aspose.gridweb.GridCell-}
```
public void setActiveCell(GridCell value)
```


Geçerli sayfanın aktif hücresini ayarlar. 1.9.0.1 sürümünden itibaren yazılabilir olarak değiştirildi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setActiveCellBgColor(Color value) {#setActiveCellBgColor-com.aspose.gridweb.Color-}
```
public void setActiveCellBgColor(Color value)
```


Etkin hücrenin arka plan rengini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveCellColor(Color value) {#setActiveCellColor-com.aspose.gridweb.Color-}
```
public void setActiveCellColor(Color value)
```


Etkin hücrenin rengini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderBgColor(Color value) {#setActiveHeaderBgColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderBgColor(Color value)
```


Etkin satır/sütun başlığının arka plan rengini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderColor(Color value) {#setActiveHeaderColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderColor(Color value)
```


Etkin satır/sütun başlığının rengini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Aktif sayfa indeksini ayarlar. WebWorksheets.ActiveSheetIndex'e eşittir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setActiveTabStyle(GridTableItemStyle value) {#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setActiveTabStyle(GridTableItemStyle value)
```


Etkin sekmenin stilini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoRefreshChart(boolean value) {#setAutoRefreshChart-boolean-}
```
public void setAutoRefreshChart(boolean value)
```


Hücre değeri güncellenirken Grafik görüntüsünün güncellenip güncellenmeyeceğini ayarlar. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


WebControl içindeki BackColor'ı ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


WebControl içindeki BorderColor'ı ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


WebControl içindeki BorderStyle'ı ayarlar

Bakınız [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


WebControl içindeki BorderWidth'ı ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomTableStyle(GridTableStyle value) {#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setBottomTableStyle(GridTableStyle value)
```


Denetimin alt çubuğunun stilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Hücre değeri değiştikten sonra veya dosya içe aktarıldıktan sonra formülün hesaplanıp hesaplanmayacağını ayarlar. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


WebControl içindeki CssClass'i ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCurrentPageIndex(int value) {#setCurrentPageIndex-int-}
```
public void setCurrentPageIndex(int value)
```


Sayfalama modunda geçerli sayfa dizinini ayarlar.

**Remarks**

Sayfalama modundayken, kontrol bir kez PageSize satır veri gösterir ve sekme çubuğunda sayfa seçme kontrolünü gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCustomCalculationEngine(GridAbstractCalculationEngine value) {#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-}
```
public void setCustomCalculationEngine(GridAbstractCalculationEngine value)
```


Kullanıcının, Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel hesaplama motorunu temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine) |  |

### setCustomStyle(InputStream stream) {#setCustomStyle-java.io.InputStream-}
```
public void setCustomStyle(InputStream stream)
```


Disk dosya akışı veya bellek akışı dahil olmak üzere akıştan özel stil dosyasını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Dosyanın akışı, disk dosyası akışı veya bellek akışı dahil. |

### setCustomStyleFileName(String value) {#setCustomStyleFileName-java.lang.String-}
```
public void setCustomStyleFileName(String value)
```


Özel stil dosyasının adını ayarlar.

**Remarks**

Özel stil dosyası bir XML dosyasıdır. Dosya adı ayarlandığında, dosya hemen yüklenecektir. İşte "standard preset style" içeriği ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Makinenin DPI değerini alır/ayarlar.

**Remarks**

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Denetimin varsayılan yazı tipi adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


Denetimin varsayılan yazı tipi boyutunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setDefaultGridLineColor(Color value) {#setDefaultGridLineColor-com.aspose.gridweb.Color-}
```
public void setDefaultGridLineColor(Color value)
```


Varsayılan ızgara çizgisi rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setDisplayCellTip(boolean value) {#setDisplayCellTip-boolean-}
```
public void setDisplayCellTip(boolean value)
```


İpuçlarının gösterilip gösterilmeyeceğini ayarlar. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEditMode(boolean value) {#setEditMode-boolean-}
```
public void setEditMode(boolean value)
```


Denetimin düzenleme modunu ayarlar.

**Remarks**

True olarak ayarlandığında, kontrolün hücreleri düzenlenebilir ve "save" ve "undo" simgeleri gösterilir. False olarak ayarlandığında, kontrolün hücreleri yalnızca okunur olur ve "save" ve "undo" simgeleri gösterilmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableAJAX(boolean value) {#setEnableAJAX-boolean-}
```
public void setEnableAJAX(boolean value)
```


AJAX çağrısının kullanılıp kullanılmayacağını ayarlar. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableAsync(boolean value) {#setEnableAsync-boolean-}
```
public void setEnableAsync(boolean value)
```


Hücre verilerinin eşzamansız şekilde yüklenip yüklenmeyeceğini ayarlar, 10.000'den fazla hücre içeren bir sayfa için uygulanması önerilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableClientColumnOperations(boolean value) {#setEnableClientColumnOperations-boolean-}
```
public void setEnableClientColumnOperations(boolean value)
```


İstemci tarafı sütun işlemlerinin etkinleştirilip etkinleştirilmeyeceğini ayarlar.

**Remarks**

True olarak ayarlandığında, kullanıcı sağ tıklama menüsünü kullanarak sütun ekleyebilir/kaldırabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableClientFreeze(boolean value) {#setEnableClientFreeze-boolean-}
```
public void setEnableClientFreeze(boolean value)
```


İstemci tarafı dondurma işlemlerinin etkinleştirilip etkinleştirilmeyeceğini ayarlar.

**Remarks**

True olarak ayarlandığında, kullanıcı sağ tıklama menüsünü kullanarak bölmeleri dondurabilir/birleştirme dondurmasını kaldırabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableClientMergeOperations(boolean value) {#setEnableClientMergeOperations-boolean-}
```
public void setEnableClientMergeOperations(boolean value)
```


İstemci tarafı birleştirme işlemlerinin etkinleştirilip etkinleştirilmeyeceğini ayarlar.

**Remarks**

True olarak ayarlandığında, kullanıcı sağ tıklama menüsünü kullanarak hücreleri birleştirebilir/birleştirmeyi kaldırabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableClientResizeColumnRow(boolean value) {#setEnableClientResizeColumnRow-boolean-}
```
public void setEnableClientResizeColumnRow(boolean value)
```


İstemci tarafı sütun ve satır yeniden boyutlandırmayı etkinleştirip etkinleştirmeyeceğini ayarlar.

**Remarks**

True olarak ayarlandığında, kullanıcı istemci tarafında sütun ve satırı yeniden boyutlandırabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableClientRowOperations(boolean value) {#setEnableClientRowOperations-boolean-}
```
public void setEnableClientRowOperations(boolean value)
```


İstemci tarafı satır işlemlerini etkinleştirip etkinleştirmeyeceğini ayarlar.

**Remarks**

True olarak ayarlandığında, kullanıcı sağ tıklama menüsünü kullanarak satır ekleyebilir/kaldırabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableDoubleClickEvent(boolean value) {#setEnableDoubleClickEvent-boolean-}
```
public void setEnableDoubleClickEvent(boolean value)
```


Müşteri tarafı çift tıklama olayını etkinleştirip etkinleştirmeyeceğini ayarlar.

**Remarks**

True olarak ayarlandığında, kontrol müşteri tarafı çift tıklama olaylarını alır ve bu olayları sunucu tarafında işleyebilirsiniz. Aksi takdirde kontrol herhangi bir çift tıklama olayını yok sayar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableMetalLightEffect(boolean value) {#setEnableMetalLightEffect-boolean-}
```
public void setEnableMetalLightEffect(boolean value)
```


Metal ışık etkisini uygulayıp uygulamayacağını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnablePaging(boolean value) {#setEnablePaging-boolean-}
```
public void setEnablePaging(boolean value)
```


Denetimin sayfalama modunu etkinleştirip etkinleştirmeyeceğini ayarlar.

**Remarks**

True olarak ayarlandığında, kontrol bir kez PageSize satır veri gösterir ve sekme çubuğunda sayfa seçme kontrolünü gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableStyleDialogbox(boolean value) {#setEnableStyleDialogbox-boolean-}
```
public void setEnableStyleDialogbox(boolean value)
```


İstemci tarafı stil iletişim kutusunu etkinleştirip etkinleştirmeyeceğini ayarlar.

**Remarks**

True olarak ayarlandığında, kullanıcı açılır menüden "Format Cell..." seçerek bir hücrenin stilini ayarlamak için stil iletişim kutusunu kullanabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


WebControl içindeki Enabled'ı ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFilteredPaging(boolean value) {#setFilteredPaging-boolean-}
```
public void setFilteredPaging(boolean value)
```


Veri filtrelendikten sonra sayfalama özelliğini etkinleştirip etkinleştirmeyeceğini ayarlar; EnablePaging true olduğunda etkili olur.

**Remarks**

True olarak ayarlandığında, kontrol filtrelenmiş verilere göre sayfalama yapar, varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Yazı tipi klasörünü ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolder | java.lang.String | TrueType yazı tiplerini içeren klasör. |
| recursive | boolean | Alt klasörlerin taranıp taranmayacağını belirler. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Yazı tipleri klasörlerini ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolders | java.lang.String[] | TrueType yazı tiplerini içeren klasörler. |
| recursive | boolean | Alt klasörlerin taranıp taranmayacağını belirler. |

### setForceValidation(boolean value) {#setForceValidation-boolean-}
```
public void setForceValidation(boolean value)
```


Müşteri tarafı doğrulamayı zorlayıp zorlamayacağını ayarlar.

**Remarks**

True olarak ayarlandığında, tüm giriş alanları geçerli olana kadar veri sunucuya gönderilmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


WebControl içindeki ForeColor'ı ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setFrameTableStyle(GridTableStyle value) {#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setFrameTableStyle(GridTableStyle value)
```


Denetimin çerçeve stilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setGoonDefaultSaveOperation(boolean value) {#setGoonDefaultSaveOperation-boolean-}
```
public void setGoonDefaultSaveOperation(boolean value)
```


GridWeb'in varsayılan kaydetme işlemini yapıp yapmayacağını ayarlar, varsayılan değer true'tır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHeaderBarHeight(Unit value) {#setHeaderBarHeight-com.aspose.gridweb.Unit-}
```
public void setHeaderBarHeight(Unit value)
```


Denetimin üst başlık çubuğunun yüksekliğini (System.Web.UI.WebControl.Unit) ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeaderBarStyle(GridTableItemStyle value) {#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setHeaderBarStyle(GridTableItemStyle value)
```


Başlık çubuğunun stilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setHeaderBarTableStyle(GridTableStyle value) {#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setHeaderBarTableStyle(GridTableStyle value)
```


Denetimin başlık çubuğu stilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setHeaderBarWidth(Unit value) {#setHeaderBarWidth-com.aspose.gridweb.Unit-}
```
public void setHeaderBarWidth(Unit value)
```


Denetimin sol başlık çubuğunun genişliğini (System.Web.UI.WebControl.Unit) ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Denetimin yüksekliğini (System.Web.UI.WebControl.Unit) ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setIgnoreStyleWithNoData(boolean value) {#setIgnoreStyleWithNoData-boolean-}
```
public void setIgnoreStyleWithNoData(boolean value)
```


GridWeb'in hücre değeri içermeyen ancak stillendirilmiş satırları veya sütunları göstermeyi görmezden gelip gelmeyeceğini ayarlar. true olarak ayarlanırsa performans daha iyi olur. Varsayılan değer false'tur; bu, son ardışık satır/sütunda hücre değeri olmasa da stil varsa yine de gösterileceği anlamına gelir. Bu seçenek yalnızca EnableAsync false olduğunda geçerlidir. EnableAsync true olduğunda bu seçeneğin etkisi yoktur; bu durumda GridWeb stil içeren tüm satırları/sütunları gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLoadOptions(GridLoadOptions value) {#setLoadOptions-com.aspose.gridweb.GridLoadOptions-}
```
public void setLoadOptions(GridLoadOptions value)
```


GridWeb için yükleme seçeneklerini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridLoadOptions](../../com.aspose.gridweb/gridloadoptions) |  |

### setMaxColumn(int value) {#setMaxColumn-int-}
```
public void setMaxColumn(int value)
```


Web sayfasının maksimum görüntülenen sütun indeksini (sıfır tabanlı) ayarlar. Denetim, MaxColumn ile sayfa verisinin maksimum sütunu arasındaki büyük değeri kullanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMaxRow(int value) {#setMaxRow-int-}
```
public void setMaxRow(int value)
```


Web sayfasının maksimum görüntülenen satır indeksini (sıfır tabanlı) ayarlar. Denetim, MaxRow ile sayfa verisinin maksimum satırı arasındaki büyük değeri kullanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMessage(String value) {#setMessage-java.lang.String-}
```
public void setMessage(String value)
```


Izgara için mesajı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setMinColumn(int value) {#setMinColumn-int-}
```
public void setMinColumn(int value)
```


Web sayfasının minimum görüntülenen sütun indeksini (sıfır tabanlı) ayarlar. Denetim, MinColumn ile sayfa verisinin minimum sütunu arasındaki küçük değeri kullanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMinRow(int value) {#setMinRow-int-}
```
public void setMinRow(int value)
```


Web sayfasının minimum görüntülenen satır indeksini (sıfır tabanlı) ayarlar. Denetim, MinRow ile sayfa verisinin minimum satırı arasındaki küçük değeri kullanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setNeedRenderGroupRows(boolean value) {#setNeedRenderGroupRows-boolean-}
```
public void setNeedRenderGroupRows(boolean value)
```


Grup satırlarını gösterip göstermeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setNoHScroll(boolean value) {#setNoHScroll-boolean-}
```
public void setNoHScroll(boolean value)
```


Yatay kaydırma çubuğunun gizli olup olmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setNoScroll(boolean value) {#setNoScroll-boolean-}
```
public void setNoScroll(boolean value)
```


Kaydırma çubuğunu gösterip göstermeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setNoVScroll(boolean value) {#setNoVScroll-boolean-}
```
public void setNoVScroll(boolean value)
```


Dikey kaydırma çubuğunun gizli olup olmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOnAjaxCallFinishedClientFunction(String value) {#setOnAjaxCallFinishedClientFunction-java.lang.String-}
```
public void setOnAjaxCallFinishedClientFunction(String value)
```


ajaxcall tamamlandığında çağrılacak istemci tarafı fonksiyon adını ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnCellErrorClientFunction(String value) {#setOnCellErrorClientFunction-java.lang.String-}
```
public void setOnCellErrorClientFunction(String value)
```


Bir hücrenin doğrulaması başarısız olduğunda çağrılacak istemci tarafı fonksiyon adını ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnCellSelectedAjaxCallBackClientFunction(String value) {#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-}
```
public void setOnCellSelectedAjaxCallBackClientFunction(String value)
```


Bir hücre seçildiğinde çağrılacak istemci tarafı fonksiyonu ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnCellSelectedClientFunction(String value) {#setOnCellSelectedClientFunction-java.lang.String-}
```
public void setOnCellSelectedClientFunction(String value)
```


Bir hücre seçildiğinde çağrılacak istemci tarafı fonksiyonu ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, \"test\");
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnCellUnselectedClientFunction(String value) {#setOnCellUnselectedClientFunction-java.lang.String-}
```
public void setOnCellUnselectedClientFunction(String value)
```


Bir hücre seçimi kaldırıldığında çağrılacak istemci tarafı fonksiyonu ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, \"test\");
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnCellUpdatedClientFunction(String value) {#setOnCellUpdatedClientFunction-java.lang.String-}
```
public void setOnCellUpdatedClientFunction(String value)
```


Bir hücrenin değeri güncellendiğinde çağrılacak istemci tarafı fonksiyon adını ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnContextMenuShowClientFunction(String value) {#setOnContextMenuShowClientFunction-java.lang.String-}
```
public void setOnContextMenuShowClientFunction(String value)
```


Bağlam menüsü gösterildiğinde çağrılacak istemci tarafı fonksiyonu ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility(\"Delete\", \"block\");
menu.setItemVisibility(\"Update\", \"none\");
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnDoubleClickCellClientFunction(String value) {#setOnDoubleClickCellClientFunction-java.lang.String-}
```
public void setOnDoubleClickCellClientFunction(String value)
```


Bir hücre çift tıklandığında çağrılacak istemci tarafı fonksiyonu ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, \"test\");
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnDoubleClickRowClientFunction(String value) {#setOnDoubleClickRowClientFunction-java.lang.String-}
```
public void setOnDoubleClickRowClientFunction(String value)
```


Bir satır çift tıklandığında çağrılacak istemci tarafı fonksiyonu ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnGridInitClientFunction(String value) {#setOnGridInitClientFunction-java.lang.String-}
```
public void setOnGridInitClientFunction(String value)
```


Izgara başlatıldığında çağrılacak istemci tarafı fonksiyon adını ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function MyOnGridInit(grid)
\{
alert(\"The grid is initialized: \" + grid.id);
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnPageChangeClientFunction(String value) {#setOnPageChangeClientFunction-java.lang.String-}
```
public void setOnPageChangeClientFunction(String value)
```


Sayfa indeksi değiştikten sonra çağrılacak istemci tarafı fonksiyonu ayarlar. Yalnızca EnablePaging true olduğunda etkili olur. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function MyOnPageChange(index)
\{
console.log(\"current page is:\"+index);
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnPageSubmitClientFunction(String value) {#setOnPageSubmitClientFunction-java.lang.String-}
```
public void setOnPageSubmitClientFunction(String value)
```


Sayfa istemci tarafında gönderilmeden önce çağrılacak istemci işlevini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnShapeSelectedClientFunction(String value) {#setOnShapeSelectedClientFunction-java.lang.String-}
```
public void setOnShapeSelectedClientFunction(String value)
```


Bir şekil seçildiğinde çağrılacak istemci tarafı fonksiyonu ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnSubmitClientFunction(String value) {#setOnSubmitClientFunction-java.lang.String-}
```
public void setOnSubmitClientFunction(String value)
```


Denetim istemci tarafında gönderilmeden önce çağrılacak istemci fonksiyonunu ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
arg, sunucuya gönderilecek komutu içeren gönderim argümanıdır. cancelEdit, denetimin gönderimden önce kullanıcı girişini iptal edip etmediğini gösteren boolean bir değerdir. Fonksiyon true döndürürse denetim gönderime devam eder.
Not: Olayı tetikleyen grid kontrolunu işaret etmek için istemci fonksiyonunda "this" işaretçisini kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Yüksekliği özelleştirilmemiş satırların yalnızca sığdırılıp sığdırılmayacağını ayarlar, varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPageSize(int value) {#setPageSize-int-}
```
public void setPageSize(int value)
```


Sayfalama modunda sayfa boyutunu ayarlar.

**Remarks**

Sayfalama modundayken, kontrol bir kez PageSize satır veri gösterir ve sekme çubuğunda sayfa seçme kontrolünü gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPictureCachePath(String value) {#setPictureCachePath-java.lang.String-}
```
public static void setPictureCachePath(String value)
```


Çalışma kitabı için görüntü depolama yolunu ayarlar, tüm şekiller ve görüntüler bu dizinde saklanır, varsayılan yol geçerli uygulamanın temel dizini altındaki acwcache'tir; kullanıcıların oturum süresi dışındaki dosyaları temizlemek için bir zamanlayıcı hizmeti uygulamaları gerekir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Ön ayarlı stili ayarlar.

[PresetStyle](../../com.aspose.gridweb/presetstyle) sayfasına bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRefreshValidation(boolean value) {#setRefreshValidation-boolean-}
```
public void setRefreshValidation(boolean value)
```


Hücre değeri değiştikten sonra doğrulama değerinin yenilenip yenilenmeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRenderHiddenRow(boolean value) {#setRenderHiddenRow-boolean-}
```
public void setRenderHiddenRow(boolean value)
```


Gizli satırın GridControl içinde render edilip edilmeyeceğini ayarlar, varsayılan değer false'tur. Daha sonra gizli satırı göstermek isterseniz, true olarak ayarlamalısınız.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRowHeightForCSV(double value) {#setRowHeightForCSV-double-}
```
public void setRowHeightForCSV(double value)
```


CSV dosyası için satır yüksekliği değerini point biriminde ayarlar, varsayılan değer 14.5'tir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setScrollBarArrowColor(Color value) {#setScrollBarArrowColor-com.aspose.gridweb.Color-}
```
public void setScrollBarArrowColor(Color value)
```


Kaydırma çubuğunun ok düğmesinin rengini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setScrollBarBaseColor(Color value) {#setScrollBarBaseColor-com.aspose.gridweb.Color-}
```
public void setScrollBarBaseColor(Color value)
```


Denetimin kaydırma çubuğunun rengini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellBgColor(Color value) {#setSelectCellBgColor-com.aspose.gridweb.Color-}
```
public void setSelectCellBgColor(Color value)
```


Çoklu seçim aralığındaki seçili hücrelerin arka plan rengini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellColor(Color value) {#setSelectCellColor-com.aspose.gridweb.Color-}
```
public void setSelectCellColor(Color value)
```


Çoklu seçim aralığındaki seçili hücrelerin rengini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSessionStorePath(String value) {#setSessionStorePath-java.lang.String-}
```
public void setSessionStorePath(String value)
```


Oturum modu File veya ViewState olduğunda oturum önbellek depolama yolunu ayarlar, örnek: gridweb.SessionStorePath=\"c:/mytempdir/session\"; böylece oturum verileri c:/mytempdir/session içinde saklanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridweb.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Çalışma kitabı ayarlarını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings) |  |

### setShowAddButton(boolean value) {#setShowAddButton-boolean-}
```
public void setShowAddButton(boolean value)
```


Çalışma sayfası ekleme düğmesinin gösterilip gösterilmeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowBottomBar(boolean value) {#setShowBottomBar-boolean-}
```
public void setShowBottomBar(boolean value)
```


Denetimin alt kısmında komut çubuğunun (komut çubuğu ve sekme çubuğu dahil) gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowCellEditBox(boolean value) {#setShowCellEditBox-boolean-}
```
public void setShowCellEditBox(boolean value)
```


Gridweb'in MS-EXCEL'deki gibi düzenleme kutusu araç çubuğunu gösterip göstermediği. Etkinleştirilirse, mevcut hücre için bir düzenleme kutusu Gridweb'te görüntülenir. Bu özelliği etkinleştirirsek, yeni özelliği desteklemek için aspx dosyalarınıza jquery js kütüphanesini eklemeniz gerekir. En son jquery sürümleri uygundur, vb.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowCommandBarAtTop(boolean value) {#setShowCommandBarAtTop-boolean-}
```
public void setShowCommandBarAtTop(boolean value)
```


Denetimin üst kısmında komut çubuğunun (komut çubuğu ve sekme çubuğu dahil) gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowContextMenu(boolean value) {#setShowContextMenu-boolean-}
```
public void setShowContextMenu(boolean value)
```


Bağlam menüsünün gösterilip gösterilmeyeceğini ayarlar. Varsayılan değer true'tır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowDefaultGridLine(boolean value) {#setShowDefaultGridLine-boolean-}
```
public void setShowDefaultGridLine(boolean value)
```


Hücrelerin varsayılan ızgara çizgilerinin gösterilip gösterilmeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowHeaderBar(boolean value) {#setShowHeaderBar-boolean-}
```
public void setShowHeaderBar(boolean value)
```


Başlık çubuğunun gösterilip gösterilmeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowLoading(boolean value) {#setShowLoading-boolean-}
```
public void setShowLoading(boolean value)
```


Sunucuya postback yapılırken bir yükleme iletişim kutusunun gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowLoadingPosition(String value) {#setShowLoadingPosition-java.lang.String-}
```
public void setShowLoadingPosition(String value)
```


Sunucuya postback yapılırken yükleme iletişim kutusunun gösterileceği sol, üst konumunu (px cinsinden) belirtir, vb. 100,200 ifadesi, yükleme iletişim kutusunun sol, üst konumunun 100px,200px olduğu anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setShowSaveButton(boolean value) {#setShowSaveButton-boolean-}
```
public void setShowSaveButton(boolean value)
```


Kaydet düğmesinin gösterilip gösterilmeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowSubmitButton(boolean value) {#setShowSubmitButton-boolean-}
```
public void setShowSubmitButton(boolean value)
```


Gönder düğmesinin gösterilip gösterilmeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowTabBar(boolean value) {#setShowTabBar-boolean-}
```
public void setShowTabBar(boolean value)
```


Sekme çubuğunun gösterilip gösterilmeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowTabNavigation(boolean value) {#setShowTabNavigation-boolean-}
```
public void setShowTabNavigation(boolean value)
```


Sekme gezinme düğmesinin gösterilip gösterilmeyeceğini ayarlar, varsayılan değer true'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowUndoButton(boolean value) {#setShowUndoButton-boolean-}
```
public void setShowUndoButton(boolean value)
```


Geri al düğmesinin gösterilip gösterilmeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSpanWrap(boolean value) {#setSpanWrap-boolean-}
```
public void setSpanWrap(boolean value)
```


İçeriğin hücre aralığında sarılıp sarılmayacağını belirtir, varsayılan değer true'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTabIndex(short value) {#setTabIndex-short-}
```
public void setTabIndex(short value)
```


WebControl içindeki TabIndex'i ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | short |  |

### setTabStyle(GridTableItemStyle value) {#setTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setTabStyle(GridTableItemStyle value)
```


Sekme çubuğunun stilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


WebControl içindeki ToolTip'i ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setUseClientPageHeight(boolean value) {#setUseClientPageHeight-boolean-}
```
public void setUseClientPageHeight(boolean value)
```


GridWeb'ün istemci sayfa yüksekliğini kontrol yüksekliği olarak kullanıp kullanmayacağını ayarlar, Height="100%" olarak ayarlandığında uygundur, varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setViewPanelScrollLeft(String value) {#setViewPanelScrollLeft-java.lang.String-}
```
public void setViewPanelScrollLeft(String value)
```


Izgaranın görüntü panelindeki kaydırma çubuğunun konumunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setViewPanelScrollTop(String value) {#setViewPanelScrollTop-java.lang.String-}
```
public void setViewPanelScrollTop(String value)
```


Izgaranın görüntü panelindeki kaydırma çubuğunun konumunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setViewTableStyle(GridTableStyle value) {#setViewTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setViewTableStyle(GridTableStyle value)
```


Veri görüntü panelinin stilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Denetimin genişliğini (System.Web.UI.WebControl.Unit) ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setXhtmlMode(boolean value) {#setXhtmlMode-boolean-}
```
public void setXhtmlMode(boolean value)
```


XHTML stilinin kullanılıp kullanılmayacağını ayarlar, varsayılan değer true'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

