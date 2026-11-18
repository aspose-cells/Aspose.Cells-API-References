---
title: "Cell Sınıfı"
linktitle: "Cell"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Cell sınıfı. Go'da cell'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/cell/
---

## Cell class

Tek bir Çalışma Kitabı hücresini temsil eden nesneyi kapsüller.

```go

type Cell struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [Calculate](./calculate/) | Hücrenin formülünü hesaplar. |
| [GetWorksheet](./getworksheet/) | Üst çalışma sayfasını alır. |
| [PutValue_Bool](./putvalue_bool/) | Hücreye bir boolean değer koyar. |
| [PutValue_Int](./putvalue_int/) | Hücreye bir tam sayı değeri koyar. |
| [PutValue_Double](./putvalue_double/) | Hücreye bir double değer koyar. |
| [PutValue_String_Bool_Bool](./putvalue_string_bool_bool/) | Hücreye bir değer koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [PutValue_String_Bool](./putvalue_string_bool/) | Hücreye bir string değeri koyar ve uygun olduğunda değeri başka bir veri tipine dönüştürür. |
| [PutValue_String](./putvalue_string/) | Hücreye bir string değeri koyar. |
| [PutValue_Date](./putvalue_date/) | Hücreye bir DateTime değeri koyar. |
| [PutValue_Object](./putvalue_object/) | Hücreye bir nesne değeri koyar. |
| [GetRow](./getrow/) | Hücrenin satır numarasını (sıfır tabanlı) alır. |
| [GetColumn](./getcolumn/) | Hücrenin sütun numarasını (sıfır tabanlı) alır. |
| [IsFormula](./isformula/) | Belirtilen hücrenin formül içerip içermediğini temsil eder. |
| [GetHasCustomFunction](./gethascustomfunction/) | Bu hücrenin formülünde özel işlev (desteklenmeyen işlev) olup olmadığını denetler. |
| [GetType](./gettype/) | Hücre değer tipini temsil eder. |
| [GetName](./getname/) | Hücrenin adını alır. |
| [IsErrorValue](./iserrorvalue/) | Bu hücrenin değerinin bir hata olup olmadığını denetler. |
| [IsNumericValue](./isnumericvalue/) | Bu hücrenin değerinin sayısal (int, double ve datetime) olup olmadığını gösterir. |
| [GetStringValue_CellValueFormatStrategy](./getstringvalue_cellvalueformatstrategy/) | Belirli biçimlendirme stratejisine göre dize değerini alır. |
| [GetStringValue](./getstringvalue/) | Hücrede bulunan dize değerini alır. Eğer bu hücrenin tipi dize ise, dize değerini kendisini döndürür. Diğer hücre tipleri için, biçimlendirilmiş dize değeri (bu hücrenin belirtilen stiliyle biçimlendirilmiş) döndürülür. Biçimlendirilmiş hücre değeri, bir hücreyi metin olarak kopyaladığınızda Excel'den alabileceğiniz şeyle aynıdır (örneğin hücreyi metin düzenleyiciye kopyalama veya csv'ye dışa aktarma). |
| [GetNumberCategoryType](./getnumbercategorytype/) | Bu hücrenin sayı biçimlendirmesinin kategori tipini temsil eder. |
| [GetDisplayStringValue](./getdisplaystringvalue/) | Hücrenin görüntüleme stiliyle biçimlendirilmiş dize değerini alır. |
| [GetIntValue](./getintvalue/) | Hücrede bulunan tam sayı değerini alır. |
| [GetDoubleValue](./getdoublevalue/) | Hücrede bulunan double değerini alır. |
| [GetFloatValue](./getfloatvalue/) | Hücrede bulunan float değerini alır. |
| [GetDateTimeValue](./getdatetimevalue/) | Hücrede bulunan DateTime değerini alır. |
| [GetBoolValue](./getboolvalue/) | Hücrede bulunan boolean değerini alır. |
| [GetWidthOfValue](./getwidthofvalue/) | Değerin piksel birimindeki genişliğini alır. |
| [GetHeightOfValue](./getheightofvalue/) | Değerin piksel birimindeki yüksekliğini alır. |
| [GetDisplayStyle](./getdisplaystyle/) | Bu hücrenin görüntüleme stilini alır. |
| [GetDisplayStyle_Bool](./getdisplaystyle_bool/) | Bu hücrenin görüntüleme stilini alır. |
| [GetDisplayStyle_BorderType](./getdisplaystyle_bordertype/) | Bu hücrenin görüntüleme stilini alır. |
| [GetFormatConditions](./getformatconditions/) | Bu hücreye uygulanan biçim koşullarını alır. |
| [GetStyle](./getstyle/) | Hücre stilini alır. |
| [GetStyle_Bool](./getstyle_bool/) | checkBorders true ise, diğer hücrelerin kenarlıklarının bu hücrenin stilini etkileyip etkilemeyeceğini denetler. |
| [SetStyle_Style](./setstyle_style/) | Hücre stilini ayarlar. |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | Stilin değiştirilen özelliğini hücreye uygular. |
| [SetStyle_Style_StyleFlag](./setstyle_style_styleflag/) | Bayraklara göre hücre stilini uygular. |
| [GetHasCustomStyle](./gethascustomstyle/) | Bu hücrenin, ilgili satır, sütun veya çalışma kitabından devralınan varsayılan ayarlardan farklı özelleştirilmiş stil ayarlarına sahip olup olmadığını gösterir. |
| [GetSharedStyleIndex](./getsharedstyleindex/) | Hücrenin stil havuzundaki paylaşılan stil indeksini alır. |
| [GetFormula](./getformula/) | Hücrenin formülünü alır veya ayarlar. |
| [SetFormula_String](./setformula_string/) | Hücrenin formülünü alır veya ayarlar. |
| [GetFormulaLocal](./getformulalocal/) | Hücrenin yerel ayarlara göre biçimlendirilmiş formülünü al. |
| [SetFormulaLocal](./setformulalocal/) | Hücrenin yerel ayarlara göre biçimlendirilmiş formülünü al. |
| [GetR1C1Formula](./getr1c1formula/) | Hücrenin R1C1 formülünü alır veya ayarlar. |
| [SetR1C1Formula](./setr1c1formula/) | Hücrenin R1C1 formülünü alır veya ayarlar. |
| [SetFormula_String_Object](./setformula_string_object/) | Formülü ve formülün değerini (hesaplanan sonuç) ayarlar. |
| [SetFormula_String_FormulaParseOptions](./setformula_string_formulaparseoptions/) | Formülü ve formülün değerini (hesaplanan sonuç) ayarlar. |
| [GetFormula_Bool_Bool](./getformula_bool_bool/) | Bu hücrenin formülünü al. |
| [SetFormula_String_FormulaParseOptions_Object](./setformula_string_formulaparseoptions_object/) | Formülü ve formülün değerini (hesaplanan sonuç) ayarlar. |
| [SetArrayFormula_String_Int_Int](./setarrayformula_string_int_int/) | Bir hücre aralığına dizi formülü (MS Excel'de CTRL+SHIFT+ENTER ile girilen eski dizi formülü) ayarlar. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions](./setarrayformula_string_int_int_formulaparseoptions/) | Bir hücre aralığına dizi formülü ayarlar. |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setarrayformula_string_int_int_formulaparseoptions_object2array/) | Bir hücre aralığına dizi formülü ayarlar. |
| [SetSharedFormula_String_Int_Int](./setsharedformula_string_int_int/) | Bir hücre aralığına paylaşılan formüller ayarlar. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions](./setsharedformula_string_int_int_formulaparseoptions/) | Bir hücre aralığına paylaşılan formüller ayarlar. |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setsharedformula_string_int_int_formulaparseoptions_object2array/) | Bir hücre aralığına paylaşılan formüller ayarlar. |
| [GetContainsExternalLink](./getcontainsexternallink/) | Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. Yalnızca hücre bir formül hücresi olduğunda geçerlidir. |
| [GetPrecedents](./getprecedents/) | Bu hücrenin formülünde görünen tüm referansları alır. |
| [GetDependents](./getdependents/) | Formülü doğrudan bu hücreye referans veren tüm hücreleri al. |
| [GetPrecedentsInCalculation](./getprecedentsincalculation/) | Bu hücrenin formülü hesaplanırken kullandığı tüm önceki hücreleri (geçerli çalışma kitabındaki hücre referansları) alır. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | Hesaplanan sonucu bu hücreye bağlı olan tüm hücreleri alır. |
| [IsArrayHeader](./isarrayheader/) | Hücrenin formülünün bir dizi formülü olduğunu ve dizinin ilk hücresi olduğunu gösterir. |
| [IsDynamicArrayFormula](./isdynamicarrayformula/) | Hücrenin formülünün dinamik dizi formülü (doğru) mu yoksa eski dizi formülü (yanlış) mu olduğunu gösterir. |
| [GetArrayRange](./getarrayrange/) | Hücrenin formülü bir dizi formülü ise dizi aralığını alır. |
| [IsArrayFormula](./isarrayformula/) | Hücre formülünün bir dizi formülü olup olmadığını gösterir. |
| [IsSharedFormula](./issharedformula/) | Hücre formülünün paylaşılan formülün bir parçası olup olmadığını gösterir. |
| [IsTableFormula](./istableformula/) | Bu hücrenin tablo formülünün bir parçası olup olmadığını gösterir. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Bool](./setdynamicarrayformula_string_formulaparseoptions_bool/) | Dinamik dizi formülü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool/) | Dinamik dizi formülü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar. |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool_CalculationOptions](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool_calculationoptions/) | Dinamik dizi formülü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar. |
| [SetTableFormula_Int_Int_String_String_Object2Array](./settableformula_int_int_string_string_object2array/) | Bu hücreden başlayan verilen aralık için iki değişkenli veri tablosu oluştur. |
| [SetTableFormula_Int_Int_String_Bool_Object2Array](./settableformula_int_int_string_bool_object2array/) | Bu hücreden başlayan verilen aralık için tek değişkenli veri tablosu oluştur. |
| [SetTableFormula_Int_Int_Int_Int_Int_Int_Object2Array](./settableformula_int_int_int_int_int_int_object2array/) | Bu hücreden başlayan verilen aralık için iki değişkenli veri tablosu oluştur. |
| [SetTableFormula_Int_Int_Int_Int_Bool_Object2Array](./settableformula_int_int_int_int_bool_object2array/) | Bu hücreden başlayan verilen aralık için tek değişkenli veri tablosu oluştur. |
| [RemoveArrayFormula](./removearrayformula/) | Dizi formülünü kaldır. |
| [Copy](./copy/) | Bir kaynak hücreden verileri kopyalar. |
| [GetValue](./getvalue/) | Bu hücredeki değeri alır/ayar. |
| [SetValue](./setvalue/) | Bu hücredeki değeri alır/ayar. |
| [IsStyleSet](./isstyleset/) | Hücrenin stilinin ayarlanıp ayarlanmadığını gösterir. false dönerse, bu hücrenin varsayılan hücre biçimine sahip olduğu anlamına gelir. |
| [Characters](./characters/) | Hücre metni içindeki bir karakter aralığını temsil eden bir Characters nesnesi döndürür. |
| [Replace](./replace/) | Hücrenin metnini seçeneklerle değiştirir. |
| [InsertText](./inserttext/) | Hücreye bazı karakterler ekler. Hücre zengin biçimlendirilmişse, bu yöntem orijinal biçimlendirmeyi koruyabilir. |
| [IsRichText](./isrichtext/) | Bu hücrenin string değerinin zengin biçimlendirilmiş bir metin olup olmadığını gösterir. |
| [GetCharacters](./getcharacters/) | Hücre metni içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür. |
| [GetCharacters_Bool](./getcharacters_bool/) | Hücre metni içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür. |
| [SetCharacters](./setcharacters/) | Hücrenin zengin metin biçimini ayarlar. |
| [IsMerged](./ismerged/) | Bir hücrenin birleştirilmiş bir aralığın parçası olup olmadığını kontrol eder. |
| [GetMergedRange](./getmergedrange/) | Birleştirilmiş aralığı temsil eden bir Range nesnesi döndürür. |
| [GetComment](./getcomment/) | Bu hücrenin yorumunu alır. |
| [GetHtmlString](./gethtmlstring/) | Bu hücrede veri ve bazı biçimlendirmeler içeren html dizesini alır ve ayarlar. |
| [SetHtmlString](./sethtmlstring/) | Bu hücrede veri ve bazı biçimlendirmeler içeren html dizesini alır ve ayarlar. |
| [GetHtmlString_Bool](./gethtmlstring_bool/) | Bu hücrede veri ve bazı biçimlendirmeler içeren html dizesini alır. |
| [ToString](./tostring/) | Geçerli Cell nesnesini temsil eden bir dize döndürür. |
| [ToJson](./tojson/) | Hücreyi JSON yapı verisine dönüştür. |
| [Equals_Object](./equals_object/) | Bu nesnenin başka bir nesneyle aynı hücreye referans olup olmadığını kontrol eder. |
| [GetHashCode](./gethashcode/) | Belirli bir tip için hash işlevi olarak hizmet eder. |
| [Equals_Cell](./equals_cell/) | Bu nesnenin başka bir hücre nesnesiyle aynı hücreye referans olup olmadığını kontrol eder. |
| [GetConditionalFormattingResult](./getconditionalformattingresult/) | Koşullu biçimlendirme sonucunu al. |
| [GetValidation](./getvalidation/) | Bu hücreye uygulanan doğrulamayı alır. |
| [GetValidationValue](./getvalidationvalue/) | Bu hücreye uygulanan doğrulamanın değerini alır. |
| [GetTable](./gettable/) | Bu hücreyi içeren tabloyu alır. |
| [IsCheckBoxStyle](./ischeckboxstyle/) | Bu hücrenin bir onay kutusu olarak ayarlanıp ayarlanmadığını gösterir. |
| [SetIsCheckBoxStyle](./setischeckboxstyle/) | Bu hücrenin bir onay kutusu olarak ayarlanıp ayarlanmadığını gösterir. |
| [GetRichValue](./getrichvalue/) | Hücrenin zengin değerini alır. |
| [GetEmbeddedImage](./getembeddedimage/) | Hücredeki gömülü resmi alır ve ayarlar. |
| [SetEmbeddedImage](./setembeddedimage/) | Hücredeki gömülü resmi alır ve ayarlar. |
| [GetPicture](./getpicture/) | Bu hücrede gömülü resmi temsil eden bir Aspose.Cells.Drawing.Picture örneğini alır; eğer bu hücrede gömülü resim yoksa null döner. |
|[Dispose](./dispose/) |  | 
