---
title: "TextBoxActiveXControl Class"
linktitle: "TextBoxActiveXControl"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "TextBoxActiveXControl class. Go'da textboxactivexcontrol'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/textboxactivexcontrol/
---

## TextBoxActiveXControl class

Bir metin kutusu ActiveX denetimini temsil eder.

```go

type TextBoxActiveXControl struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewTextBoxActiveXControl](./newtextboxactivexcontrol/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetType](./gettype/) | ActiveX kontrolünün türünü alır. |
| [GetBorderStyle](./getborderstyle/) | Denetim tarafından kullanılan kenarlık tipini alır ve ayarlar. |
| [SetBorderStyle](./setborderstyle/) | Denetim tarafından kullanılan kenarlık tipini alır ve ayarlar. |
| [GetBorderOleColor](./getborderolecolor/) | Arka planın OLE rengini alır ve ayarlar. |
| [SetBorderOleColor](./setborderolecolor/) | Arka planın OLE rengini alır ve ayarlar. |
| [GetSpecialEffect](./getspecialeffect/) | Denetimin özel efektini alır ve ayarlar. |
| [SetSpecialEffect](./setspecialeffect/) | Denetimin özel efektini alır ve ayarlar. |
| [GetMaxLength](./getmaxlength/) | Maksimum karakter sayısını alır ve ayarlar. |
| [SetMaxLength](./setmaxlength/) | Maksimum karakter sayısını alır ve ayarlar. |
| [GetScrollBars](./getscrollbars/) | Kontrolün dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi veya hiçbiri olup olmadığını belirtir. |
| [SetScrollBars](./setscrollbars/) | Kontrolün dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi veya hiçbiri olup olmadığını belirtir. |
| [GetPasswordChar](./getpasswordchar/) | Girilen karakterlerin yerine görüntülenecek bir karakteri alır ve ayarlar. |
| [SetPasswordChar](./setpasswordchar/) | Girilen karakterlerin yerine görüntülenecek bir karakteri alır ve ayarlar. |
| [IsEditable](./iseditable/) | Kullanıcının denetime yazıp yazamayacağını gösterir. |
| [SetIsEditable](./setiseditable/) | Kullanıcının denetime yazıp yazamayacağını gösterir. |
| [GetIntegralHeight](./getintegralheight/) | Denetimin yalnızca tam metin satırlarını gösterip kısmi satırları göstermeyeceğini gösterir. |
| [SetIntegralHeight](./setintegralheight/) | Denetimin yalnızca tam metin satırlarını gösterip kısmi satırları göstermeyeceğini gösterir. |
| [IsDragBehaviorEnabled](./isdragbehaviorenabled/) | Denetim için sürükle ve bırakın etkin olup olmadığını gösterir. |
| [SetIsDragBehaviorEnabled](./setisdragbehaviorenabled/) | Denetim için sürükle ve bırakın etkin olup olmadığını gösterir. |
| [GetEnterKeyBehavior](./getenterkeybehavior/) | ENTER tuşunun davranışını belirtir. True, ENTER'a basmanın yeni bir satır oluşturacağını belirtir. False, ENTER'a basmanın odak noktasını sekme sırasındaki bir sonraki nesneye taşıyacağını belirtir. |
| [SetEnterKeyBehavior](./setenterkeybehavior/) | ENTER tuşunun davranışını belirtir. True, ENTER'a basmanın yeni bir satır oluşturacağını belirtir. False, ENTER'a basmanın odak noktasını sekme sırasındaki bir sonraki nesneye taşıyacağını belirtir. |
| [GetEnterFieldBehavior](./getenterfieldbehavior/) | Denetime girildiğinde seçim davranışını belirtir. True, seçimin denetim son kez aktif olduğunda olduğu gibi değişmeden kalacağını belirtir. False, denetime girildiğinde denetimdeki tüm metnin seçileceğini belirtir. |
| [SetEnterFieldBehavior](./setenterfieldbehavior/) | Denetime girildiğinde seçim davranışını belirtir. True, seçimin denetim son kez aktif olduğunda olduğu gibi değişmeden kalacağını belirtir. False, denetime girildiğinde denetimdeki tüm metnin seçileceğini belirtir. |
| [GetTabKeyBehavior](./gettabkeybehavior/) | Denetimin metninde sekme karakterlerine izin verilip verilmediğini gösterir. |
| [SetTabKeyBehavior](./settabkeybehavior/) | Denetimin metninde sekme karakterlerine izin verilip verilmediğini gösterir. |
| [GetHideSelection](./gethideselection/) | Denetimin odaklanmadığında seçili metnin vurgulanıp vurgulanmadığını gösterir. |
| [SetHideSelection](./sethideselection/) | Denetimin odaklanmadığında seçili metnin vurgulanıp vurgulanmadığını gösterir. |
| [IsAutoTab](./isautotab/) | Kullanıcı maksimum karakter sayısını girdiğinde odak noktasının otomatik olarak bir sonraki denetime geçip geçmeyeceğini gösterir. |
| [SetIsAutoTab](./setisautotab/) | Kullanıcı maksimum karakter sayısını girdiğinde odak noktasının otomatik olarak bir sonraki denetime geçip geçmeyeceğini gösterir. |
| [IsMultiLine](./ismultiline/) | Denetimin birden fazla satır metin görüntüleyip görüntüleyemeyeceğini gösterir. |
| [SetIsMultiLine](./setismultiline/) | Denetimin birden fazla satır metin görüntüleyip görüntüleyemeyeceğini gösterir. |
| [IsWordWrapped](./iswordwrapped/) | Denetimin içeriğinin bir satırın sonunda otomatik olarak kaydırılıp kaydırılmayacağını gösterir. |
| [SetIsWordWrapped](./setiswordwrapped/) | Denetimin içeriğinin bir satırın sonunda otomatik olarak kaydırılıp kaydırılmayacağını gösterir. |
| [GetText](./gettext/) | Denetimin metnini alır ve ayarlar. |
| [SetText](./settext/) | Denetimin metnini alır ve ayarlar. |
| [GetDropButtonStyle](./getdropbuttonstyle/) | Açılır düğmede gösterilen sembolü belirtir. |
| [SetDropButtonStyle](./setdropbuttonstyle/) | Açılır düğmede gösterilen sembolü belirtir. |
| [GetShowDropButtonTypeWhen](./getshowdropbuttontypewhen/) | Açılır düğmede gösterilen sembolü belirtir. |
| [SetShowDropButtonTypeWhen](./setshowdropbuttontypewhen/) | Açılır düğmede gösterilen sembolü belirtir. |
| [IsAutoWordSelected](./isautowordselected/) | Bir seçimi genişletmek için kullanılan temel birimi belirtir. True, temel birimin tek bir karakter olduğunu belirtir. false, temel birimin tam bir kelime olduğunu belirtir. |
| [SetIsAutoWordSelected](./setisautowordselected/) | Bir seçimi genişletmek için kullanılan temel birimi belirtir. True, temel birimin tek bir karakter olduğunu belirtir. false, temel birimin tam bir kelime olduğunu belirtir. |
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
