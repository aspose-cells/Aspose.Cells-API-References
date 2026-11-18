---
title: "ListBoxActiveXControl Sınıfı"
linktitle: "ListBoxActiveXControl"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ListBoxActiveXControl sınıfı. Go'da listboxactivexcontrol'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/listboxactivexcontrol/
---

## ListBoxActiveXControl class

Bir ListBox ActiveX kontrolünü temsil eder.

```go

type ListBoxActiveXControl struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewListBoxActiveXControl](./newlistboxactivexcontrol/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetType](./gettype/) | ActiveX kontrolünün türünü alır. |
| [GetScrollBars](./getscrollbars/) | Kontrolün dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi veya hiçbiri olup olmadığını belirtir. |
| [SetScrollBars](./setscrollbars/) | Kontrolün dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi veya hiçbiri olup olmadığını belirtir. |
| [GetListWidth](./getlistwidth/) | Genişliği puan biriminde alır ve ayarlar. |
| [SetListWidth](./setlistwidth/) | Genişliği puan biriminde alır ve ayarlar. |
| [GetBoundColumn](./getboundcolumn/) | Bir ComboBox veya ListBox için Value özelliğinin MultiSelect özelliğinin değeri (fmMultiSelectSingle) olduğunda nasıl belirlendiğini temsil eder. |
| [SetBoundColumn](./setboundcolumn/) | Bir ComboBox veya ListBox için Value özelliğinin MultiSelect özelliğinin değeri (fmMultiSelectSingle) olduğunda nasıl belirlendiğini temsil eder. |
| [GetTextColumn](./gettextcolumn/) | Kullanıcıya gösterilecek bir ComboBox veya ListBox içindeki sütunu temsil eder. |
| [SetTextColumn](./settextcolumn/) | Kullanıcıya gösterilecek bir ComboBox veya ListBox içindeki sütunu temsil eder. |
| [GetColumnCount](./getcolumncount/) | Bir ComboBox veya ListBox içinde gösterilecek sütun sayısını temsil eder. |
| [SetColumnCount](./setcolumncount/) | Bir ComboBox veya ListBox içinde gösterilecek sütun sayısını temsil eder. |
| [GetMatchEntry](./getmatchentry/) | Kullanıcı yazdıkça bir ListBox veya ComboBox'un listesini nasıl aradığını gösterir. |
| [SetMatchEntry](./setmatchentry/) | Kullanıcı yazdıkça bir ListBox veya ComboBox'un listesini nasıl aradığını gösterir. |
| [GetListStyle](./getliststyle/) | Görsel görünümü alır ve ayarlar. |
| [SetListStyle](./setliststyle/) | Görsel görünümü alır ve ayarlar. |
| [GetSelectionType](./getselectiontype/) | Denetimin birden fazla seçim yapmasına izin verip vermediğini gösterir. |
| [SetSelectionType](./setselectiontype/) | Denetimin birden fazla seçim yapmasına izin verip vermediğini gösterir. |
| [GetValue](./getvalue/) | Denetimin değerini alır ve ayarlar. |
| [SetValue](./setvalue/) | Denetimin değerini alır ve ayarlar. |
| [GetBorderStyle](./getborderstyle/) | Denetim tarafından kullanılan kenarlık tipini alır ve ayarlar. |
| [SetBorderStyle](./setborderstyle/) | Denetim tarafından kullanılan kenarlık tipini alır ve ayarlar. |
| [GetBorderOleColor](./getborderolecolor/) | Arka planın OLE rengini alır ve ayarlar. |
| [SetBorderOleColor](./setborderolecolor/) | Arka planın OLE rengini alır ve ayarlar. |
| [GetSpecialEffect](./getspecialeffect/) | Denetimin özel efektini alır ve ayarlar. |
| [SetSpecialEffect](./setspecialeffect/) | Denetimin özel efektini alır ve ayarlar. |
| [GetShowColumnHeads](./getshowcolumnheads/) | Sütun başlıklarının gösterilip gösterilmediğini belirtir. |
| [SetShowColumnHeads](./setshowcolumnheads/) | Sütun başlıklarının gösterilip gösterilmediğini belirtir. |
| [GetIntegralHeight](./getintegralheight/) | Denetimin yalnızca tam metin satırlarını gösterip kısmi satırları göstermeyeceğini gösterir. |
| [SetIntegralHeight](./setintegralheight/) | Denetimin yalnızca tam metin satırlarını gösterip kısmi satırları göstermeyeceğini gösterir. |
| [GetColumnWidths](./getcolumnwidths/) | Sütunun genişliğini alır ve ayarlar. |
| [SetColumnWidths](./setcolumnwidths/) | Sütunun genişliğini alır ve ayarlar. |
| [IsEnabled](./isenabled/) | Denetimin odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir. |
| [SetIsEnabled](./setisenabled/) | Denetimin odağı alıp kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini gösterir. |
| [IsLocked](./islocked/) | Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir. |
| [SetIsLocked](./setislocked/) | Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir. |
| [IsTransparent](./istransparent/) | Denetimin şeffaf olup olmadığını gösterir. |
| [SetIsTransparent](./setistransparent/) | Denetimin şeffaf olup olmadığını gösterir. |
| [GetIMEMode](./getimemode/) | Denetim odaklandığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zamanı modunu alır ve ayarlar. |
| [SetIMEMode](./setimemode/) | Denetim odaklandığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zamanı modunu alır ve ayarlar. |
| [GetFont](./getfont/) | Denetimin yazı tipini temsil eder. |
| [GetTextAlign](./gettextalign/) | Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder. |
| [SetTextAlign](./settextalign/) | Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder. |
| [GetData](./getdata/) | Kontrolün ikili verisini alır ve ayarlar. |
| [IsAutoSize](./isautosize/) | Denetimin tüm içeriğini gösterecek şekilde otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını gösterir. |
| [SetIsAutoSize](./setisautosize/) | Denetimin tüm içeriğini gösterecek şekilde otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını gösterir. |
| [GetWorkbook](./getworkbook/) | Workbook nesnesini alır. |
| [GetMouseIcon](./getmouseicon/) | Kontrol için fare imleci olarak görüntülenecek özel bir simgeyi alır ve ayarlar. |
| [SetMouseIcon](./setmouseicon/) | Kontrol için fare imleci olarak görüntülenecek özel bir simgeyi alır ve ayarlar. |
| [GetMousePointer](./getmousepointer/) | Kontrol için fare imleci olarak görüntülenecek simge türünü alır ve ayarlar. |
| [SetMousePointer](./setmousepointer/) | Kontrol için fare imleci olarak görüntülenecek simge türünü alır ve ayarlar. |
| [GetLinkedCell](./getlinkedcell/) | Bağlantılı hücreyi alır ve ayarlar. |
| [SetLinkedCell](./setlinkedcell/) | Bağlantılı hücreyi alır ve ayarlar. |
| [GetListFillRange](./getlistfillrange/) | Liste doldurma aralığını alır ve ayarlar. |
| [SetListFillRange](./setlistfillrange/) | Liste doldurma aralığını alır ve ayarlar. |
| [GetWidth](./getwidth/) | Kontrolün genişliğini puan biriminde alır ve ayarlar. |
| [SetWidth](./setwidth/) | Kontrolün genişliğini puan biriminde alır ve ayarlar. |
| [GetHeight](./getheight/) | Kontrolün yüksekliğini puan biriminde alır ve ayarlar. |
| [SetHeight](./setheight/) | Kontrolün yüksekliğini puan biriminde alır ve ayarlar. |
| [GetForeOleColor](./getforeolecolor/) | Ön planın OLE rengini alır ve ayarlar. |
| [SetForeOleColor](./setforeolecolor/) | Ön planın OLE rengini alır ve ayarlar. |
| [GetBackOleColor](./getbackolecolor/) | Arka planın OLE rengini alır ve ayarlar. |
| [SetBackOleColor](./setbackolecolor/) | Arka planın OLE rengini alır ve ayarlar. |
| [IsVisible](./isvisible/) | Bu kontrolün görünür olup olmadığını gösterir. |
| [SetIsVisible](./setisvisible/) | Bu kontrolün görünür olup olmadığını gösterir. |
| [GetShadow](./getshadow/) | Gölgenin gösterilip gösterilmeyeceğini belirtir. |
| [SetShadow](./setshadow/) | Gölgenin gösterilip gösterilmeyeceğini belirtir. |
