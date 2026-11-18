---
title: "CellsDrawing Sınıfı"
linktitle: "CellsDrawing"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "CellsDrawing sınıfı. Go'da cellsdrawing'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/cellsdrawing/
---

## CellsDrawing class

Otomatik şekli ve çizim nesnesini temsil eder.

```go

type CellsDrawing struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewCellsDrawing](./newcellsdrawing/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetMacroName](./getmacroname/) | Makronun adını alır ve ayarlar. |
| [SetMacroName](./setmacroname/) | Makronun adını alır ve ayarlar. |
| [IsEquation](./isequation/) | Şeklin yalnızca bir denklem içerip içermediğini gösterir. |
| [IsSmartArt](./issmartart/) | Şeklin akıllı sanat olup olmadığını gösterir. |
| [ToFrontOrBack](./tofrontorback/) | Şekli öne getirir veya şekli arkaya gönderir. |
| [GetZOrderPosition](./getzorderposition/) | Şeklin z-sırasındaki konumunu döndürür. |
| [SetZOrderPosition](./setzorderposition/) | Şeklin z-sırasındaki konumunu döndürür. |
| [GetName](./getname/) | Şeklin adını alır ve ayarlar. |
| [SetName](./setname/) | Şeklin adını alır ve ayarlar. |
| [GetAlternativeText](./getalternativetext/) | Shape nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar. |
| [SetAlternativeText](./setalternativetext/) | Shape nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar. |
| [GetTitle](./gettitle/) | Mevcut şekil nesnesinin başlığını (alt yazısını) belirtir. |
| [SetTitle](./settitle/) | Mevcut şekil nesnesinin başlığını (alt yazısını) belirtir. |
| [GetLine](./getline/) | Çizgi stilini alır |
| [GetFill](./getfill/) | Belirtilen şekil için dolgu biçimlendirme özelliklerini içeren bir FillFormat nesnesi döndürür. |
| [GetShadowEffect](./getshadoweffect/) | Chart öğesi veya şekil için gölge etkisini belirten bir Drawing.ShadowEffect nesnesini temsil eder. |
| [GetReflection](./getreflection/) | Chart öğesi veya şekil için yansıma etkisini belirten bir ReflectionEffect nesnesini temsil eder. |
| [GetGlow](./getglow/) | Chart öğesi veya şekil için parıltı etkisini belirten bir GlowEffect nesnesini temsil eder. |
| [GetSoftEdges](./getsoftedges/) | Kenarlar için uygulanacak bulanıklık yarıçapını, puan biriminde alır ve ayarlar. |
| [SetSoftEdges](./setsoftedges/) | Kenarlar için uygulanacak bulanıklık yarıçapını, puan biriminde alır ve ayarlar. |
| [GetThreeDFormat](./getthreedformat/) | Şeklin 3D biçimini alır ve ayarlar. |
| [GetFormatPicture](./getformatpicture/) | Resim formatının seçeneklerini alır ve ayarlar. |
| [IsHidden](./ishidden/) | Nesnenin görünür olup olmadığını gösterir. |
| [SetIsHidden](./setishidden/) | Nesnenin görünür olup olmadığını gösterir. |
| [IsAspectRatioLocked](./isaspectratiolocked/) | Doğru, şeklin en‑boy oranının kilitlendiği anlamına gelir. |
| [SetIsAspectRatioLocked](./setisaspectratiolocked/) | Doğru, şeklin en‑boy oranının kilitlendiği anlamına gelir. |
| [GetLockedProperty](./getlockedproperty/) | Kilitli özelliğinin değerini alır. |
| [SetLockedProperty](./setlockedproperty/) | Kilitli özelliğini ayarla. |
| [GetRotationAngle](./getrotationangle/) | Şeklin dönüşünü alır ve ayarlar. |
| [SetRotationAngle](./setrotationangle/) | Şeklin dönüşünü alır ve ayarlar. |
| [AddHyperlink](./addhyperlink/) | Şekle bir köprü ekler. |
| [RemoveHyperlink](./removehyperlink/) | Şeklin köprüsünü kaldırır. |
| [GetHyperlink](./gethyperlink/) | Şeklin köprüsünü alır. |
| [MoveToRange](./movetorange/) | Şekli belirtilen bir aralığa taşır. |
| [AlignTopRightCorner](./aligntoprightcorner/) | Resmi sağ üst köşeye taşır. |
| [GetId](./getid/) | Bu şeklin tanımlayıcısını alır. |
| [GetSpid](./getspid/) | Uygulamanın belirli şekli tanımlamak için kullanabileceği isteğe bağlı bir dize tanımlayıcısını belirtir. |
| [GetSpt](./getspt/) | Uygulamanın belirli şekli tanımlı bir şekil türüyle ilişkilendirmek için kullanabileceği isteğe bağlı bir sayı belirtir. |
| [GetWorksheet](./getworksheet/) | Bu şekli içeren Aspose.Cells.Worksheet nesnesini alır. |
| [IsGroup](./isgroup/) | Bu şeklin bir grup şekli olup olmadığını gösterir. |
| [IsInGroup](./isingroup/) | Şeklin gruplanıp gruplanmadığını gösterir. |
| [IsWordArt](./iswordart/) | Bu şeklin bir word art olup olmadığını gösterir. |
| [GetTextEffect](./gettexteffect/) | Belirtilen şekil için metin efekti biçimlendirme özelliklerini içeren bir TextEffectFormat nesnesi döndürür. WordArt'ı temsil eden Shape nesneleri için geçerlidir. |
| [IsLocked](./islocked/) | True, sayfa korunduğunda nesnenin değiştirilemeyeceği anlamına gelir. Bu değerin yalnızca çalışma sayfası veya çalışma sayfasındaki nesneler korunduğunda anlamlı olduğunu unutmayın. |
| [SetIsLocked](./setislocked/) | True, sayfa korunduğunda nesnenin değiştirilemeyeceği anlamına gelir. Bu değerin yalnızca çalışma sayfası veya çalışma sayfasındaki nesneler korunduğunda anlamlı olduğunu unutmayın. |
| [IsPrintable](./isprintable/) | Nesnenin yazdırılabilir olup olmadığını gösterir. False ise, bu şekil yazdırma sırasında basılmaz. |
| [SetIsPrintable](./setisprintable/) | Nesnenin yazdırılabilir olup olmadığını gösterir. False ise, bu şekil yazdırma sırasında basılmaz. |
| [GetMsoDrawingType](./getmsodrawingtype/) | Çizim tipini alır. |
| [GetAutoShapeType](./getautoshapetype/) | Otomatik şekil tipini alır ve ayarlar. |
| [SetAutoShapeType](./setautoshapetype/) | Otomatik şekil tipini alır ve ayarlar. |
| [GetAnchorType](./getanchortype/) | Şekil ankraj yer tutucusunun tipini alır ve ayarlar. |
| [SetAnchorType](./setanchortype/) | Şekil ankraj yer tutucusunun tipini alır ve ayarlar. |
| [GetPlacement](./getplacement/) | Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder. Bu özellik, bir nesnenin çalışma sayfasındaki konumunu kontrol eder. |
| [SetPlacement](./setplacement/) | Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder. Bu özellik, bir nesnenin çalışma sayfasındaki konumunu kontrol eder. |
| [GetUpperLeftRow](./getupperleftrow/) | Üst satır indeksini temsil eder. |
| [SetUpperLeftRow](./setupperleftrow/) | Üst satır indeksini temsil eder. |
| [GetUpperDeltaY](./getupperdeltay/) | Şeklin sol üst köşe satırından dikey ofsetini alır veya ayarlar. |
| [SetUpperDeltaY](./setupperdeltay/) | Şeklin sol üst köşe satırından dikey ofsetini alır veya ayarlar. |
| [GetUpperLeftColumn](./getupperleftcolumn/) | Sol üst köşe sütun indeksini temsil eder. |
| [SetUpperLeftColumn](./setupperleftcolumn/) | Sol üst köşe sütun indeksini temsil eder. |
| [GetUpperDeltaX](./getupperdeltax/) | Şeklin sol üst köşe sütunundan yatay ofsetini alır veya ayarlar. |
| [SetUpperDeltaX](./setupperdeltax/) | Şeklin sol üst köşe sütunundan yatay ofsetini alır veya ayarlar. |
| [GetLowerRightRow](./getlowerrightrow/) | Alt sağ köşe satır indeksini temsil eder. |
| [SetLowerRightRow](./setlowerrightrow/) | Alt sağ köşe satır indeksini temsil eder. |
| [GetLowerDeltaY](./getlowerdeltay/) | Şeklin alt sağ köşe satırından dikey ofsetini alır veya ayarlar. |
| [SetLowerDeltaY](./setlowerdeltay/) | Şeklin alt sağ köşe satırından dikey ofsetini alır veya ayarlar. |
| [GetLowerRightColumn](./getlowerrightcolumn/) | Alt sağ köşe sütun indeksini temsil eder. |
| [SetLowerRightColumn](./setlowerrightcolumn/) | Alt sağ köşe sütun indeksini temsil eder. |
| [GetLowerDeltaX](./getlowerdeltax/) | Şeklin alt sağ köşe sütunundan yatay ofsetini alır veya ayarlar. |
| [SetLowerDeltaX](./setlowerdeltax/) | Şeklin alt sağ köşe sütunundan yatay ofsetini alır veya ayarlar. |
| [GetRight](./getright/) | Şeklin alt sağ köşe sütunundan yatay ofsetinin genişliğini piksel biriminde temsil eder. |
| [SetRight](./setright/) | Şeklin alt sağ köşe sütunundan yatay ofsetinin genişliğini piksel biriminde temsil eder. |
| [GetBottom](./getbottom/) | Şeklin alt alt köşe satırından dikey ofsetinin genişliğini piksel biriminde temsil eder. |
| [SetBottom](./setbottom/) | Şeklin alt alt köşe satırından dikey ofsetinin genişliğini piksel biriminde temsil eder. |
| [GetWidth](./getwidth/) | Şeklin genişliğini piksel biriminde temsil eder. |
| [SetWidth](./setwidth/) | Şeklin genişliğini piksel biriminde temsil eder. |
| [GetWidthInch](./getwidthinch/) | Şeklin genişliğini inç biriminde temsil eder. |
| [SetWidthInch](./setwidthinch/) | Şeklin genişliğini inç biriminde temsil eder. |
| [GetWidthPt](./getwidthpt/) | Şeklin genişliğini puan (point) biriminde temsil eder. |
| [SetWidthPt](./setwidthpt/) | Şeklin genişliğini puan (point) biriminde temsil eder. |
| [GetWidthCM](./getwidthcm/) | Şeklin genişliğini santimetre biriminde temsil eder. |
| [SetWidthCM](./setwidthcm/) | Şeklin genişliğini santimetre biriminde temsil eder. |
| [GetHeight](./getheight/) | Şeklin yüksekliğini temsil eder, birim olarak piksel. |
| [SetHeight](./setheight/) | Şeklin yüksekliğini temsil eder, birim olarak piksel. |
| [GetHeightInch](./getheightinch/) | Şeklin yüksekliğini temsil eder, birim olarak inç. |
| [SetHeightInch](./setheightinch/) | Şeklin yüksekliğini temsil eder, birim olarak inç. |
| [GetHeightPt](./getheightpt/) | Şeklin yüksekliğini temsil eder, birim olarak nokta. |
| [SetHeightPt](./setheightpt/) | Şeklin yüksekliğini temsil eder, birim olarak nokta. |
| [GetHeightCM](./getheightcm/) | Şeklin yüksekliğini temsil eder, birim olarak santimetre. |
| [SetHeightCM](./setheightcm/) | Şeklin yüksekliğini temsil eder, birim olarak santimetre. |
| [GetLeft](./getleft/) | Şeklin sol sütunundan yatay ofsetini temsil eder, birim olarak piksel. |
| [SetLeft](./setleft/) | Şeklin sol sütunundan yatay ofsetini temsil eder, birim olarak piksel. |
| [GetLeftInch](./getleftinch/) | Şeklin sol sütunundan yatay ofsetini temsil eder, birim olarak inç. |
| [SetLeftInch](./setleftinch/) | Şeklin sol sütunundan yatay ofsetini temsil eder, birim olarak inç. |
| [GetLeftCM](./getleftcm/) | Şeklin sol sütunundan yatay ofsetini temsil eder, birim olarak santimetre. |
| [SetLeftCM](./setleftcm/) | Şeklin sol sütunundan yatay ofsetini temsil eder, birim olarak santimetre. |
| [GetTop](./gettop/) | Şeklin üst satırından dikey ofsetini temsil eder, birim olarak piksel. |
| [SetTop](./settop/) | Şeklin üst satırından dikey ofsetini temsil eder, birim olarak piksel. |
| [GetTopInch](./gettopinch/) | Şeklin üst satırından dikey ofsetini temsil eder, birim olarak inç. |
| [SetTopInch](./settopinch/) | Şeklin üst satırından dikey ofsetini temsil eder, birim olarak inç. |
| [GetTopCM](./gettopcm/) | Şeklin üst satırından dikey ofsetini temsil eder, birim olarak santimetre. |
| [SetTopCM](./settopcm/) | Şeklin üst satırından dikey ofsetini temsil eder, birim olarak santimetre. |
| [GetTopToCorner](./gettoptocorner/) | Şeklin çalışma sayfası üst kenarından dikey ofsetini alır ve ayarlar, birim olarak piksel. |
| [SetTopToCorner](./settoptocorner/) | Şeklin çalışma sayfası üst kenarından dikey ofsetini alır ve ayarlar, birim olarak piksel. |
| [GetLeftToCorner](./getlefttocorner/) | Şeklin çalışma sayfası sol kenarından yatay ofsetini alır ve ayarlar. |
| [SetLeftToCorner](./setlefttocorner/) | Şeklin çalışma sayfası sol kenarından yatay ofsetini alır ve ayarlar. |
| [GetX](./getx/) | Şeklin çalışma sayfası sol kenarından yatay ofsetini alır ve ayarlar, birim olarak piksel. |
| [SetX](./setx/) | Şeklin çalışma sayfası sol kenarından yatay ofsetini alır ve ayarlar, birim olarak piksel. |
| [GetY](./gety/) | Şeklin çalışma sayfası üst kenarından dikey ofsetini alır ve ayarlar, birim olarak piksel. |
| [SetY](./sety/) | Şeklin çalışma sayfası üst kenarından dikey ofsetini alır ve ayarlar, birim olarak piksel. |
| [GetWidthScale](./getwidthscale/) | Genişlik ölçeğini alır ve ayarlar, birim olarak orijinal resim genişliğinin yüzde değeri. Şekil resim değilse, WidthScale özelliği yalnızca 100 döndürür; |
| [SetWidthScale](./setwidthscale/) | Genişlik ölçeğini alır ve ayarlar, birim olarak orijinal resim genişliğinin yüzde değeri. Şekil resim değilse, WidthScale özelliği yalnızca 100 döndürür; |
| [GetHeightScale](./getheightscale/) | Yükseklik ölçeğini alır ve ayarlar, birim olarak orijinal resim yüksekliğinin yüzde değeri. Şekil resim değilse, HeightScale özelliği yalnızca 100 döndürür; |
| [SetHeightScale](./setheightscale/) | Yükseklik ölçeğini alır ve ayarlar, birim olarak orijinal resim yüksekliğinin yüzde değeri. Şekil resim değilse, HeightScale özelliği yalnızca 100 döndürür; |
| [GetTopInShape](./gettopinshape/) | Şeklin ebeveyn şeklinin üst kenarından dikey ofsetini temsil eder, birim olarak ebeveyn şeklin yüksekliğinin 1/4000'i. |
| [SetTopInShape](./settopinshape/) | Şeklin ebeveyn şeklinin üst kenarından dikey ofsetini temsil eder, birim olarak ebeveyn şeklin yüksekliğinin 1/4000'i. |
| [GetLeftInShape](./getleftinshape/) | Şeklin ebeveyn şeklinin sol kenarından yatay ofsetini temsil eder, birim olarak ebeveyn şeklin genişliğinin 1/4000'i. |
| [SetLeftInShape](./setleftinshape/) | Şeklin ebeveyn şeklinin sol kenarından yatay ofsetini temsil eder, birim olarak ebeveyn şeklin genişliğinin 1/4000'i. |
| [GetWidthInShape](./getwidthinshape/) | Şeklin genişliğini temsil eder, birim olarak ebeveyn şeklinin 1/4000'i. |
| [SetWidthInShape](./setwidthinshape/) | Şeklin genişliğini temsil eder, birim olarak ebeveyn şeklinin 1/4000'i. |
| [GetHeightInShape](./getheightinshape/) | Şeklin ebeveyn şeklinin üst kenarından dikey ofsetini temsil eder, birim olarak ebeveyn şeklin yüksekliğinin 1/4000'i.. |
| [SetHeightInShape](./setheightinshape/) | Şeklin ebeveyn şeklinin üst kenarından dikey ofsetini temsil eder, birim olarak ebeveyn şeklin yüksekliğinin 1/4000'i.. |
| [GetGroup](./getgroup/) | Bu şekli içeren grup şeklini alır. |
| [GetType](./gettype/) | Otomatik şekil tipini alır. |
| [GetHasLine](./gethasline/) | Şeklin çizgi kenarlığının görünür olup olduğunu alır ve ayarlar. |
| [SetHasLine](./sethasline/) | Şeklin çizgi kenarlığının görünür olup olduğunu alır ve ayarlar. |
| [IsFilled](./isfilled/) | Dolgu biçiminin görünür olup olduğunu gösterir. |
| [SetIsFilled](./setisfilled/) | Dolgu biçiminin görünür olup olduğunu gösterir. |
| [IsFlippedHorizontally](./isflippedhorizontally/) | Şeklin yatay olarak çevrilmiş olup olmadığını alır ve ayarlar. |
| [SetIsFlippedHorizontally](./setisflippedhorizontally/) | Şeklin yatay olarak çevrilmiş olup olmadığını alır ve ayarlar. |
| [IsFlippedVertically](./isflippedvertically/) | Şeklin dikey olarak çevrilip çevrilmediğini alır ve ayarlar . |
| [SetIsFlippedVertically](./setisflippedvertically/) | Şeklin dikey olarak çevrilip çevrilmediğini alır ve ayarlar . |
| [GetActualLowerRightRow](./getactuallowerrightrow/) | Gerçek alt satırı al. |
| [GetConnectionPoints](./getconnectionpoints/) | Bağlantı noktalarını al |
| [ToImage_ImageType](./toimage_imagetype/) | Şekil görüntüsünü oluşturur ve belirtilen formatta bir akışa kaydeder. |
| [GetRelativeToOriginalPictureSize](./getrelativetooriginalpicturesize/) | Şeklin orijinal resim boyutuna göre olup olmadığını gösterir. |
| [SetRelativeToOriginalPictureSize](./setrelativetooriginalpicturesize/) | Şeklin orijinal resim boyutuna göre olup olmadığını gösterir. |
| [GetLinkedCell](./getlinkedcell/) | Denetimin değerine bağlı çalışma sayfası aralığını alır veya ayarlar. |
| [SetLinkedCell_String](./setlinkedcell_string/) | Denetimin değerine bağlı çalışma sayfası aralığını alır veya ayarlar. |
| [GetInputRange](./getinputrange/) | Belirtilen combo kutusunu doldurmak için kullanılan çalışma sayfası aralığını alır veya ayarlar. |
| [SetInputRange_String](./setinputrange_string/) | Belirtilen combo kutusunu doldurmak için kullanılan çalışma sayfası aralığını alır veya ayarlar. |
| [UpdateSelectedValue](./updateselectedvalue/) | Seçili değeri, bağlı hücrenin değeriyle günceller. |
| [GetTextShapeType](./gettextshapetype/) | Önceden ayarlanmış metin şekli türünü alır ve ayarlar. |
| [SetTextShapeType](./settextshapetype/) | Önceden ayarlanmış metin şekli türünü alır ve ayarlar. |
| [GetTextBody](./gettextbody/) | Şeklin metin ayarını alır ve ayarlar. |
| [GetFont](./getfont/) | Şeklin yazı tipini temsil eder. |
| [SetFont](./setfont/) | Şeklin yazı tipini temsil eder. |
| [GetTextOptions](./gettextoptions/) | Şeklin metin seçeneklerini temsil eder. |
| [SetTextOptions](./settextoptions/) | Şeklin metin seçeneklerini temsil eder. |
| [CalculateTextSize](./calculatetextsize/) | Metin alanını yeniden hesapla |
| [GetText](./gettext/) | Bu şeklin metnini alır ve ayarlar. |
| [SetText](./settext/) | Bu şeklin metnini alır ve ayarlar. |
| [IsRichText](./isrichtext/) | Metnin zengin metin olup olmadığı. |
| [GetHtmlText](./gethtmltext/) | Bu metin kutusunda veri ve bazı biçimleri içeren html dizesini alır ve ayarlar. |
| [SetHtmlText](./sethtmltext/) | Bu metin kutusunda veri ve bazı biçimleri içeren html dizesini alır ve ayarlar. |
| [FormatCharacters](./formatcharacters/) | Bazı karakterleri yazı tipi ayarıyla biçimlendirir. |
| [Characters](./characters/) | Metin içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür. |
| [GetRichFormattings](./getrichformattings/) | Metin içinde bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür . |
| [GetTextVerticalOverflow](./gettextverticaloverflow/) | Metin içeren şeklin metin dikey taşma türünü alır ve ayarlar. |
| [SetTextVerticalOverflow](./settextverticaloverflow/) | Metin içeren şeklin metin dikey taşma türünü alır ve ayarlar. |
| [GetTextHorizontalOverflow](./gettexthorizontaloverflow/) | Metin içeren şeklin metin yatay taşma türünü alır ve ayarlar. |
| [SetTextHorizontalOverflow](./settexthorizontaloverflow/) | Metin içeren şeklin metin yatay taşma türünü alır ve ayarlar. |
| [IsTextWrapped](./istextwrapped/) | Metin içeren şeklin metin sarma türünü alır ve ayarlar. |
| [SetIsTextWrapped](./setistextwrapped/) | Metin içeren şeklin metin sarma türünü alır ve ayarlar. |
| [GetTextOrientationType](./gettextorientationtype/) | Şeklin metin yönlendirme türünü alır ve ayarlar. |
| [SetTextOrientationType](./settextorientationtype/) | Şeklin metin yönlendirme türünü alır ve ayarlar. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Şeklin metin yatay hizalama türünü alır ve ayarlar. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Şeklin metin yatay hizalama türünü alır ve ayarlar. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Şeklin metin dikey hizalama türünü alır ve ayarlar. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Şeklin metin dikey hizalama türünü alır ve ayarlar. |
| [GetTextDirection](./gettextdirection/) | Bu nesne için metin akışının yönünü alır/ayarlar. |
| [SetTextDirection](./settextdirection/) | Bu nesne için metin akışının yönünü alır/ayarlar. |
| [GetTextBoxOptions](./gettextboxoptions/) | Şekildeki metin bilgilerini alır |
| [GetControlData](./getcontroldata/) | Denetimin verilerini alır. |
| [GetActiveXControl](./getactivexcontrol/) | ActiveX denetimini alır. |
| [RemoveActiveXControl](./removeactivexcontrol/) | ActiveX denetimini kaldır. |
| [GetPaths](./getpaths/) | Özel bir geometrik şeklin yollarını alır. |
| [GetGeometry](./getgeometry/) | Geometriyi alır |
| [GetCreateId](./getcreateid/) | Bu şekil için oluşturma kimliğini alır ve ayarlar. |
| [SetCreateId](./setcreateid/) | Bu şekil için oluşturma kimliğini alır ve ayarlar. |
| [IsDecorative](./isdecorative/) | Nesnenin dekoratif olup olmadığını gösterir. |
| [SetIsDecorative](./setisdecorative/) | Nesnenin dekoratif olup olmadığını gösterir. |
| [GetActualBox](./getactualbox/) | Şeklin gerçek konumunu ve boyutunu al (döndürme, çevirme vb. uygulandıktan sonra). |
| [FitToTextSize](./fittotextsize/) | Tüm metin içeriğini gösterecek uygun bir metin alanını yeniden hesaplar. |
| [GetResultOfSmartArt](./getresultofsmartart/) | Akıllı sanatı gruplanmış şekillere dönüştürür. |
| [IsSameSetting](./issamesetting/) | Şeklin aynı olup olmadığını döndürür. |
