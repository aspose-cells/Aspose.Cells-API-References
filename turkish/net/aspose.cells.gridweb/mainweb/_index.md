---
title: "Sınıf MainWeb"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.MainWeb sınıfı. GridWeb kontrolünün üst sınıfı. Yalnızca dahili kullanım için"
type: docs
url: /tr/net/aspose.cells.gridweb/mainweb/
---
## MainWeb class

GridWeb denetiminin üst sınıfı. Yalnızca dahili kullanım için.

```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler, 
    IPostBackEventHandler, ISerializable
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [MainWeb](mainweb/)() | MainWeb kontrolünün varsayılan yapıcı yöntemi. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell/) { get; set; } | Mevcut sayfanın aktif hücresini alır veya ayarlar. 1.9.0.1 sürümünden itibaren yazılabilir olarak değiştirildi. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor/) { get; set; } | Etkin hücrenin arka plan rengini belirtir. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor/) { get; set; } | Etkin hücrenin rengini belirtir. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor/) { get; set; } | Etkin satır/sütun başlığının arka plan rengini belirtir. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor/) { get; set; } | Etkin satır/sütun başlığının rengini belirtir. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet/) { get; } | Aktif sayfayı alır |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex/) { get; set; } | Aktif sayfa indeksini alır veya ayarlar. WebWorksheets.ActiveSheetIndex'e eşittir. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle/) { get; set; } | Aktif sekmenin stilini belirtir. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath/) { get; set; } | Denetimin script/görüntü dosyalarının web yolunu alır veya ayarlar. Örneğin: "http://localhost/acw_client". Bu değeri web.config dosyasında da ayarlayabilirsiniz. Bu bölümü `<configuration>` bölümüne ekleyin:`<appSettings>``<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />``</appSettings>` |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl/) { get; set; } | Denetimin dil dosyasının web URL'sini alır veya ayarlar. Örneğin: "/acw_client/lang_en.js". Varsayılan olarak, yerleşik bir İngilizce dosya kullanılır. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart/) { get; set; } | Hücre değeri güncellenirken Grafik görüntüsünün güncellenip güncellenmeyeceğini alır veya ayarlar. Varsayılan değer true'tır. |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle/) { get; set; } | Denetimin alt çubuğunun stilini alır veya ayarlar. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex/) { get; set; } | Sayfalama modunda geçerli sayfa dizinini alır veya ayarlar. |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine/) { get; set; } | Kullanıcının, Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel hesaplama motorunu temsil eder. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons/) { get; } | Özel komut düğmesi koleksiyonunu alır |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename/) { get; set; } | Özel stil dosya adını alır veya ayarlar. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname/) { get; set; } | Denetimin varsayılan yazı tipi adını alır veya ayarlar. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize/) { get; set; } | Denetimin varsayılan yazı tipi boyutunu alır veya ayarlar. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor/) { get; set; } | Varsayılan ızgara çizgisinin rengini alır veya ayarlar. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip/) { get; set; } | İpuçlarını gösterip göstermeyeceğini alır veya ayarlar. Varsayılan değer doğrudur. |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode/) { get; set; } | Denetimin düzenleme modunu alır veya ayarlar. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax/) { get; set; } | AJAX çağrısı kullanılıp kullanılmayacağını alır veya ayarlar. Varsayılan değer doğrudur. |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync/) { get; set; } | Hücre verilerinin eşzamansız şekilde yüklenip yüklenmeyeceğini alır veya ayarlar, 10.000'den fazla hücresi olan bir sayfa için uygulanması önerilir |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations/) { get; set; } | İstemci tarafı sütun işlemlerinin etkinleştirilip etkinleştirilmeyeceğini alır veya ayarlar. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze/) { get; set; } | İstemci tarafı dondurma işlemlerinin etkinleştirilip etkinleştirilmeyeceğini alır veya ayarlar. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations/) { get; set; } | İstemci tarafı birleştirme işlemlerinin etkinleştirilip etkinleştirilmeyeceğini alır veya ayarlar. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow/) { get; set; } | İstemci tarafı sütun ve satır yeniden boyutlandırmanın etkinleştirilip etkinleştirilmeyeceğini alır veya ayarlar. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations/) { get; set; } | İstemci tarafı satır işlemlerinin etkinleştirilip etkinleştirilmeyeceğini alır veya ayarlar. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent/) { get; set; } | Müşteri tarafı çift tıklama olayının etkinleştirilip etkinleştirilmeyeceğini alır veya ayarlar. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect/) { get; set; } | Metal ışık etkisinin uygulanıp uygulanmayacağını alır veya ayarlar. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging/) { get; set; } | Denetimin sayfalama modunun etkinleştirilip etkinleştirilmeyeceğini alır veya ayarlar. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox/) { get; set; } | İstemci tarafı stil iletişim kutusunun etkinleştirilip etkinleştirilmeyeceğini alır veya ayarlar. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging/) { get; set; } | Veri filtrelendikten sonra sayfalamanın etkinleştirilip etkinleştirilmeyeceğini alır veya ayarlar, EnablePaging true olduğunda etkili olur |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation/) { get; set; } | Müşteri tarafı doğrulamanın zorunlu olup olmayacağını alır veya ayarlar. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle/) { get; set; } | Denetimin çerçeve stilini alır veya ayarlar. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation/) { get; set; } | GridWeb'in varsayılan kaydetme işlemini yapıp yapmayacağını alır veya ayarlar, varsayılan değer doğrudur. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight/) { get; set; } | Denetimin üst başlık çubuğunun yüksekliğini (System.Web.UI.WebControl.Unit) alır veya ayarlar. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle/) { get; set; } | Başlık çubuğunun stilini alır veya ayarlar. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle/) { get; set; } | Denetimin başlık çubuğu stilini alır veya ayarlar. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth/) { get; set; } | Denetimin genişliğini (System.Web.UI.WebControl.Unit) veya sol başlık çubuğunu alır veya ayarlar. |
| override [Height](../../aspose.cells.gridweb/mainweb/height/) { get; set; } | Denetimin yüksekliğini (System.Web.UI.WebControl.Unit) alır veya ayarlar. |
| [IgnoreStyleWithNoData](../../aspose.cells.gridweb/mainweb/ignorestylewithnodata/) { get; set; } | GridWeb'in hücre değeri içermeyen ancak stillendirilmiş satırları veya sütunları göstermeyi göz ardı edip etmeyeceğini alır veya ayarlar. true olarak ayarlanırsa performans daha iyi olur. Varsayılan değer false'tur; bu, son ardışık satır/sütunun hücre değeri olmaması ancak stillendirilmiş olması durumunda yine de görüntüleneceği anlamına gelir. Bu seçenek yalnızca EnableAsync false olduğunda geçerlidir. EnableAsync true olduğunda bu seçeneğin etkisi yoktur; bu, GridWeb'in stil uygulanmış tüm satırları/sütunları göstereceği anlamına gelir. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula/) { get; set; } | Hücre değeri değiştikten sonra veya dosya içe aktarıldıktan sonra formülün hesaplanıp hesaplanmayacağını alır veya ayarlar. Varsayılan değer true'tur. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback/) { get; } | GridWeb'in istemci postback'ine yanıt olarak mı yoksa ilk kez yüklenip erişiliyor mu olduğunu gösteren bir değeri alır. |
| [LoadOptions](../../aspose.cells.gridweb/mainweb/loadoptions/) { get; set; } | GridWeb için yükleme seçeneklerini temsil eder. |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn/) { get; set; } | Web sayfasının maksimum görüntüleme sütun indeksini (sıfır tabanlı) alır veya ayarlar. Denetim, MaxColumn ve sayfa verisinin maksimum sütun değerinden daha büyük olanı kullanır. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow/) { get; set; } | Web sayfasının maksimum görüntüleme satır indeksini (sıfır tabanlı) alır veya ayarlar. Denetim, MaxRow ve sayfa verisinin maksimum satır değerinden daha büyük olanı kullanır. |
| [Message](../../aspose.cells.gridweb/mainweb/message/) { get; set; } | Izgara için mesajı alır veya ayarlar. |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn/) { get; set; } | Web sayfasının minimum görüntüleme sütun indeksini (sıfır tabanlı) alır veya ayarlar. Denetim, MinColumn ve sayfa verisinin minimum sütun değerinden daha küçük olanı kullanır. |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow/) { get; set; } | Web sayfasının minimum görüntüleme satır indeksini (sıfır tabanlı) alır veya ayarlar. Denetim, MinRow ve sayfa verisinin minimum satır değerinden daha küçük olanı kullanır. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells/) { get; } | İstemci tarafından değiştirilen hücrelerin koleksiyonunu alır. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows/) { get; set; } | Grup satırlarının gösterilip gösterilmeyeceğini alır veya ayarlar. |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll/) { get; set; } | Yatay kaydırma çubuğunun gizli olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll/) { get; set; } | Kaydırma çubuğunun gösterilip gösterilmeyeceğini alır veya ayarlar. |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll/) { get; set; } | Dikey kaydırma çubuğunun gizli olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction/) { get; set; } | Ajax çağrısı tamamlandığında çağrılacak istemci tarafı fonksiyon adını alır veya ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır: function GridAjaxcallFinished() { alert(this.id+\" ajaxcall finished \"); } Not: Olayı tetikleyen ızgara denetimini işaret etmek için istemci fonksiyonunda \"this\" işaretçisini kullanabilirsiniz. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction/) { get; set; } | Bir hücrenin doğrulaması başarısız olduğunda çağrılacak istemci tarafı fonksiyon adını alır veya ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır: function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); } Not: Olayı tetikleyen ızgara denetimini işaret etmek için istemci fonksiyonunda \"this\" işaretçisini kullanabilirsiniz. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction/) { get; set; } | Bir hücre seçildiğinde çağrılacak istemci tarafı fonksiyonunu alır veya ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır: function MyOnSelectCellAjaxCallBack(cell,customerdata) { } Not: Olayı tetikleyen ızgara denetimini işaret etmek için istemci fonksiyonunda \"this\" işaretçisini kullanabilirsiniz. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction/) { get; set; } | Bir hücre seçildiğinde çağrılacak istemci tarafı fonksiyonunu alır veya ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır: function MyOnSelectCell(cell) { GridWeb1.setCellValueByCell(cell, \"test\"); } Not: Olayı tetikleyen ızgara denetimini işaret etmek için istemci fonksiyonunda \"this\" işaretçisini kullanabilirsiniz. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction/) { get; set; } | Bir hücrenin seçimi kaldırıldığında çağrılacak istemci tarafı fonksiyonunu alır veya ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır: function MyOnUnselectCell(cell) { this.setCellValueByCell(cell, \"test\"); } Not: Olayı tetikleyen ızgara denetimini işaret etmek için istemci fonksiyonunda \"this\" işaretçisini kullanabilirsiniz. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/) { get; set; } | Bir hücrenin değeri güncellendiğinde çağrılacak istemci tarafı fonksiyon adını alır veya ayarlar. İstemci fonksiyonu şu şekilde tanımlanmalıdır: function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); } Not: Olayı tetikleyen ızgara denetimini işaret etmek için istemci fonksiyonunda \"this\" işaretçisini kullanabilirsiniz. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/) { get; set; } | İçerik menüsü gösterildiğinde çağrılacak istemci tarafı işlevi alır veya ayarlar. İstemci işlevi şu şekilde tanımlanmalıdır: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }Not: İstemci işlevinde "this" işaretçisini, olayı tetikleyen ızgara kontrolüne işaret etmek için kullanabilirsiniz. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction/) { get; set; } | Bir hücre çift tıklandığında çağrılacak istemci tarafı işlevi alır veya ayarlar. İstemci işlevi şu şekilde tanımlanmalıdır: function MyOnDoubleClickCell(cell) { this.setCellValueByCell(cell, "test"); }Not: İstemci işlevinde "this" işaretçisini, olayı tetikleyen ızgara kontrolüne işaret etmek için kullanabilirsiniz. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction/) { get; set; } | Bir satır çift tıklandığında çağrılacak istemci tarafı işlevi alır veya ayarlar. İstemci işlevi şu şekilde tanımlanmalıdır: function MyOnRowDoubleClick(row) { alert(row); }Not: İstemci işlevinde "this" işaretçisini, olayı tetikleyen ızgara kontrolüne işaret etmek için kullanabilirsiniz. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction/) { get; set; } | Izgara başlatıldığında çağrılacak istemci tarafı işlev adını alır veya ayarlar. İstemci işlevi şu şekilde tanımlanmalıdır: function MyOnGridInit(grid) { alert("The grid is initialized: " + grid.id); }Not: İstemci işlevinde "this" işaretçisini, olayı tetikleyen ızgara kontrolüne işaret etmek için kullanabilirsiniz. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto/) { get; set; } | Yalnızca yüksekliği özelleştirilmemiş satırları sığdırıp sığdırmayacağını alır veya ayarlar, varsayılan değer false'tur. |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction/) { get; set; } | Sayfa indeksi değiştikten sonra çağrılacak istemci tarafı işlevi alır veya ayarlar. Yalnızca EnablePaging true olduğunda etkili olur. İstemci işlevi şu şekilde tanımlanmalıdır: function MyOnPageChange(index) { console.log("current page is:"+index); }Not: İstemci işlevinde "this" işaretçisini, olayı tetikleyen ızgara kontrolüne işaret etmek için kullanabilirsiniz. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction/) { get; set; } | İstemci tarafında sayfa gönderilmeden önce çağrılacak istemci işlevi alır veya ayarlar. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/) { get; set; } | Bir şekil seçildiğinde çağrılacak istemci tarafı işlevi alır veya ayarlar. İstemci işlevi şu şekilde tanımlanmalıdır: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }Not: İstemci işlevinde "this" işaretçisini, olayı tetikleyen ızgara kontrolüne işaret etmek için kullanabilirsiniz. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction/) { get; set; } | İstemci tarafında kontrol gönderilmeden önce çağrılacak istemci işlevi alır veya ayarlar. İstemci işlevi şu şekilde tanımlanmalıdır: function MyOnSubmit(arg, cancelEdit) { return true;} Arg, gönderim argümanıdır ve sunucuya gönderilecek komutu içerir. cancelEdit, kontrolün gönderimden önce kullanıcı girdisini iptal edip etmediğini gösteren boolean değerdir. İşlev true döndürürse kontrol gönderime devam eder. Not: İstemci işlevinde "this" işaretçisini, olayı tetikleyen ızgara kontrolüne işaret etmek için kullanabilirsiniz. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize/) { get; set; } | Sayfalama modunda sayfa boyutunu alır veya ayarlar. |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle/) { get; set; } | Ön ayar stilini alır veya ayarlar. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation/) { get; set; } | Hücre değeri değiştikten sonra doğrulama değerinin yenilenip yenilenmeyeceğini alır veya ayarlar. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow/) { get; set; } | Gizli satırın GridControl içinde render edilip edilmeyeceğini alır veya ayarlar, varsayılan değer false'tur. Gizli satırı daha sonra göstermek isterseniz, bunu true olarak ayarlamalısınız. |
| [RowHeightForCSV](../../aspose.cells.gridweb/mainweb/rowheightforcsv/) { get; set; } | CSV dosyası için satır yüksekliği değerini nokta cinsinden alır veya ayarlar, varsayılan değer 14.5'tir. |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor/) { get; set; } | Kaydırma çubuğunun ok düğmesinin rengini belirtir. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor/) { get; set; } | Kontrolün kaydırma çubuğunun rengini belirtir. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor/) { get; set; } | Seçili hücrelerin çoklu seçim aralığındaki arka plan rengini belirler. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor/) { get; set; } | Seçili hücrelerin çoklu seçim aralığındaki rengini belirler. |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode/) { get; set; } | Izgaranın oturum modunu alır veya ayarlar. |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath/) { get; set; } | Oturum modu File veya ViewState olduğunda oturum önbellek depolama yolunu alır veya ayarlar, örnek: gridweb.SessionStorePath="c:/mytempdir/session"; ardından oturum verileri c:/mytempdir/session içinde depolanır. |
| [Settings](../../aspose.cells.gridweb/mainweb/settings/) { get; set; } | Çalışma kitabı ayarlarını temsil eder. |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton/) { get; set; } | Çalışma sayfası ekleme düğmesinin gösterilip gösterilmeyeceğini alır veya ayarlar. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar/) { get; set; } | Kontrolün alt kısmında komut çubuğunun (komut çubuğu ve sekme çubuğu dahil) gösterilip gösterilmeyeceğini belirtir. |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox/) { get; set; } | Gridweb'in MS-EXCEL gibi düzenleme kutusu araç çubuğunu gösterip göstermediği. Etkinleştirilirse, geçerli hücre için bir düzenleme kutusu Gridweb içinde görüntülenir. Bu özelliği etkinleştirirsek, bu yeni özelliği desteklemek için aspx dosyalarınıza jquery js kütüphanesini eklemeniz gerekir. En son jquery sürümü uygundur, vb. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop/) { get; set; } | Denetimin üst kısmında komut çubuğunun (komut çubuğu ve sekme çubuğu dahil) gösterilip gösterilmeyeceğini belirtir. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu/) { get; set; } | Bağlam menüsünün gösterilip gösterilmeyeceğini alır veya ayarlar. Varsayılan değer true'tur. |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline/) { get; set; } | Hücrelerin varsayılan ızgara çizgilerinin gösterilip gösterilmeyeceğini alır veya ayarlar. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar/) { get; set; } | Başlık çubuğunun gösterilip gösterilmeyeceğini alır veya ayarlar. |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading/) { get; set; } | Sunucuya postback yapılırken bir yükleme iletişim kutusunun gösterilip gösterilmeyeceğini belirtir. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition/) { get; set; } | Sunucuya postback yapılırken yükleme iletişim kutusunun gösterileceği sol, üst konumunu (px cinsinden) belirtir, vb. 100,200 değeri, yükleme iletişim kutusunun sol, üst konumunun 100px,200px olduğunu gösterir. |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton/) { get; set; } | Kaydet düğmesinin gösterilip gösterilmeyeceğini alır veya ayarlar. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton/) { get; set; } | Gönder düğmesinin gösterilip gösterilmeyeceğini alır veya ayarlar. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar/) { get; set; } | Sekme çubuğunun gösterilip gösterilmeyeceğini alır veya ayarlar. |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation/) { get; set; } | Sekme gezinme düğmesinin gösterilip gösterilmeyeceğini alır veya ayarlar, varsayılan değer true'tur. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton/) { get; set; } | Geri al düğmesinin gösterilip gösterilmeyeceğini alır veya ayarlar. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap/) { get; set; } | Hücre aralığında içeriğin kaydırılıp kaydırılmayacağını belirtir. Varsayılan değer true'tur. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle/) { get; set; } | Sekme çubuğunun stilini alır veya ayarlar. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight/) { get; set; } | GridWeb'in istemci sayfa yüksekliğini kontrol yüksekliği olarak kullanıp kullanmayacağını alır veya ayarlar, Height=\"100%\" ayarlandığında uygundur, varsayılan değer false'tur. |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft/) { get; set; } | Izgaranın görüntü panelinin kaydırma çubuğu konumunu alır veya ayarlar. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop/) { get; set; } | Izgaranın görüntü panelinin kaydırma çubuğu konumunu alır veya ayarlar. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle/) { get; set; } | Veri görüntü panelinin stilini alır veya ayarlar. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets/) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width/) { get; set; } | Denetimin genişliğini (System.Web.UI.WebControl.Unit) alır veya ayarlar. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets/) { get; } | Çalışma sayfalarının koleksiyonunu alır veya ayarlar. |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode/) { get; set; } | XHTML stilinin kullanılıp kullanılmayacağını alır veya ayarlar, varsayılan değer true'tur. |
| static [DPI](../../aspose.cells.gridweb/mainweb/dpi/) { get; set; } | Makinenin DPI değerini alır/ayarlar. |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath/) { get; set; } | Çalışma kitabı için görüntü depolama yolunu alır veya ayarlar, tüm şekil ve görüntüler bu dizinde saklanır, varsayılan yol mevcut uygulama temel dizini altında acwcache'tir, kullanıcıların oturum süresi dışındaki dosyaları temizlemek için bir zamanlayıcı hizmeti uygulamaları gerekir. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula/)() | Formüllerin sonucunu hesaplar. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind/)() | Denetimi ve tüm alt denetimlerini veri kaynağına bağlar. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose/)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile)(Stream) | Disk dosya akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_2)(string) | Bir Excel dosyasından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_1)(Stream, string) | Disk dosya akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_3)(string, string) | Bir Excel dosyasından içe aktarır. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile)(Stream) | CSV dosya akışından veri yükler. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile_1)(string) | CSV dosyasından veri yükler. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile)(Stream) | HTML dosya akışından veri yükler. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile_1)(string) | HTML dosyasından veri yükler. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | SpreadSheetML dosya akışından veri yükler. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | SpreadSheetML dosyasından veri yükler. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape/)() | Etkin çalışma sayfası için tüm grafik görüntülerini yeniler. |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag/)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile)(Stream) | Verileri CSV dosya akışına kaydeder. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile_1)(string) | Verileri CSV dosyasına kaydeder. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile/)(string) | Denetimin mevcut stil verilerini bir xml dosyasına kaydeder. Özelleştirilmiş stil dosyanızı oluşturmak için kullanılabilir. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile)(Stream) | Verileri HTML dosya akışına kaydeder. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile_1)(string) | Verileri HTML dosyasına kaydeder. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Verileri SpreadSheetML dosya akışına kaydeder. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Verileri SpreadSheetML dosyasına kaydeder. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile)(Stream) | Çalışma sayfalarını bir Excel dosyasına kaydeder. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_3)(string) | Çalışma sayfalarını Excel 2003 formatında bir Excel dosyasına kaydeder. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Çalışma sayfalarını bir Excel dosyasına kaydeder. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_2)(Stream, GridSaveOptions) | Çalışma sayfalarını bir Excel dosyasına kaydeder. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_4)(string, GridSaveFormat) | Çalışma sayfalarını bir Excel dosyasına kaydeder. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_5)(string, GridSaveOptions) | Çalışma sayfalarını bir Excel dosyasına kaydeder. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle/)(Stream) | Disk dosya akışı veya bellek akışı dahil olmak üzere akıştan özel stil dosyasını ayarlar. |

## Olaylar

| Ad | Açıklama |
| --- | --- |
| event [AfterColumnFilter](../../aspose.cells.gridweb/mainweb/aftercolumnfilter/) | Sütun filtrelendikten sonra meydana gelir. |
| event [AjaxCallFinished](../../aspose.cells.gridweb/mainweb/ajaxcallfinished/) | Denetimin ajax güncellemesi tamamlandığında tetiklenir.(EnableAJAX true olarak ayarlanmalıdır) |
| event [BeforeColumnFilter](../../aspose.cells.gridweb/mainweb/beforecolumnfilter/) | Filtrelenecek sütundan önce meydana gelir. |
| event [CellClickOnAjax](../../aspose.cells.gridweb/mainweb/cellclickonajax/) | Hücre tıklandığında meydana gelir, ve bu olay için ajaxcallback yapılması gerekir. |
| event [CellClientUpdate](../../aspose.cells.gridweb/mainweb/cellclientupdate/) | İstemci hücre güncellemesi gerçekleştiğinde meydana gelir. Bu olay tetiklendiğinde, parametresi e.Argument komutun adını içerir. |
| event [CellCommand](../../aspose.cells.gridweb/mainweb/cellcommand/) | Hücrenin komut bağlantısına tıklandığında meydana gelir. Bu olay tetiklendiğinde, parametresi e.Argument komutun adını içerir. |
| event [CellDoubleClick](../../aspose.cells.gridweb/mainweb/celldoubleclick/) | Hücre çift tıklandığında meydana gelir. |
| event [CellError](../../aspose.cells.gridweb/mainweb/cellerror/) | Hücrenin giriş değeri hatalı olduğunda meydana gelir. |
| event [CellModifiedOnAjax](../../aspose.cells.gridweb/mainweb/cellmodifiedonajax/) | Hücre ajax çağrısında değiştirildiğinde meydana gelir. |
| event [ColumnDeleted](../../aspose.cells.gridweb/mainweb/columndeleted/) | Kullanıcı istemci tarafı menüsünden bir sütunu sildiğinde meydana gelir. |
| event [ColumnDeleting](../../aspose.cells.gridweb/mainweb/columndeleting/) | Kullanıcı istemci tarafı menüsünden bir sütunu silmeye çalıştığında meydana gelir. Bu olayı işleyebilir ve iptal parametresini True olarak ayarlayarak silme işlemini iptal edebilirsiniz. |
| event [ColumnDoubleClick](../../aspose.cells.gridweb/mainweb/columndoubleclick/) | Sütun başlığı çift tıklandığında meydana gelir. |
| event [ColumnInserted](../../aspose.cells.gridweb/mainweb/columninserted/) | Kullanıcı istemci tarafı menüsünden bir sütun eklediğinde meydana gelir. |
| event [CustomCommand](../../aspose.cells.gridweb/mainweb/customcommand/) | Kullanıcı özel bir komut düğmesine tıkladığında meydana gelir. |
| event [LoadCustomData](../../aspose.cells.gridweb/mainweb/loadcustomdata/) | Denetimin SessionMode'u Custom olarak ayarlandığında ve sayfa verilerini yüklemesi gerektiğinde tetiklenir. Bu olayı Custom Session modunda dosya veya veritabanından sayfa verilerini yüklemek için işleyebilirsiniz. |
| event [PageIndexChanged](../../aspose.cells.gridweb/mainweb/pageindexchanged/) | Denetimin sayfa sekmesi indeksi değiştiğinde meydana gelir. |
| event [RowDeleted](../../aspose.cells.gridweb/mainweb/rowdeleted/) | Kullanıcı istemci tarafı menüsünden bir satırı sildiğinde meydana gelir. |
| event [RowDeleting](../../aspose.cells.gridweb/mainweb/rowdeleting/) | Kullanıcı istemci tarafı menüsünden bir satırı silmeye çalıştığında meydana gelir. Bu olayı işleyebilir ve silme işlemini iptal etmek için bir RejectDeleteException istisnası fırlatabilirsiniz. |
| event [RowDoubleClick](../../aspose.cells.gridweb/mainweb/rowdoubleclick/) | Satır başlığı çift tıklandığında meydana gelir. |
| event [RowInserted](../../aspose.cells.gridweb/mainweb/rowinserted/) | Kullanıcı istemci tarafı menüsünden bir satır eklediğinde meydana gelir. |
| event [SaveCommand](../../aspose.cells.gridweb/mainweb/savecommand/) | "save" düğmesine tıklandığında meydana gelir. |
| event [SheetAdded](../../aspose.cells.gridweb/mainweb/sheetadded/) | Kullanıcı araç çubuğu menüsünden bir çalışma sayfası eklediğinde meydana gelir. |
| event [SheetDataUpdated](../../aspose.cells.gridweb/mainweb/sheetdataupdated/) | Denetim gönderilen verileri yüklediğinde ve sayfa verilerini güncellediğinde meydana gelir. |
| event [SheetTabClick](../../aspose.cells.gridweb/mainweb/sheettabclick/) | Sayfa sekmesi tıklandığında meydana gelir. |
| event [SubmitCommand](../../aspose.cells.gridweb/mainweb/submitcommand/) | "submit" düğmesine tıklandığında meydana gelir. |
| event [UndoCommand](../../aspose.cells.gridweb/mainweb/undocommand/) | "undo" düğmesi tıklandığında oluşur. |

### Örnekler

```csharp
[C#]
	GridWeb GridWeb1 = new GridWeb();
//işinizi yapın
```

### Ayrıca Bakınız

* class [ExtWebControl](../extwebcontrol/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


