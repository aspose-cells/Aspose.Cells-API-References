---
title: "Cells Sınıfı"
linktitle: "Hücreler"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Cells sınıfı. Go'da hücreleri temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/cells/
---

## Cells class

Hücreyle ilgili nesneler koleksiyonunu kapsüller, örneğin <see cref="Cell"/>, <see cref="Row"/>, vb.

```go

type Cells struct  {
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
| [GetOdsCellFields](./getodscellfields/) | ods'in alan listesine erişir. |
| [Dispose](./dispose/) | Yönetilmeyen kaynakları serbest bırakma, bırakma veya sıfırlama ile ilgili uygulama tanımlı görevleri yürütür. |
| [GetCount](./getcount/) | Oluşturulan Cell nesnelerinin toplam sayısına erişir. |
| [GetCountLarge](./getcountlarge/) | Oluşturulan Cell nesnelerinin toplam sayısına erişir. |
| [GetEnumerator](./getenumerator/) | Hücre enumerator'ına erişir. |
| [GetRows](./getrows/) | Bu çalışma sayfasındaki bireysel satırları temsil eden Row nesnelerinin koleksiyonuna erişir. |
| [GetMergedAreas](./getmergedareas/) | Tüm birleştirilmiş hücrelere erişir. |
| [CheckCell](./checkcell/) | Belirtilen hücre satır indeksi ve sütun indeksi için Cell öğesine veya null değerine erişir. |
| [CheckRow](./checkrow/) | Belirtilen hücre satır indeksi için Row öğesine veya null değerine erişir. |
| [CheckColumn](./checkcolumn/) | Belirtilen sütun indeksi için Column öğesine veya null değerine erişir. |
| [IsRowHidden](./isrowhidden/) | Verilen indeksdeki satırın gizli olup olmadığını kontrol eder. |
| [IsColumnHidden](./iscolumnhidden/) | Verilen indeksdeki sütunun gizli olup olmadığını kontrol eder. |
| [AddRange](./addrange/) | Hücrelere bir aralık nesnesi referansı ekler |
| [CreateRange_String_String](./createrange_string_string/) | Hücre aralığından bir Range nesnesi oluşturur. |
| [CreateRange_Int_Int_Int_Int](./createrange_int_int_int_int/) | Hücre aralığından bir Range nesnesi oluşturur. |
| [CreateRange_String](./createrange_string/) | Aralığın adresinden bir Range nesnesi oluşturur. |
| [CreateRange_Int_Int_Bool](./createrange_int_int_bool/) | Hücre satırlarından veya sütunlarından bir Range nesnesi oluşturur. |
| [Get_Int_Int](./get_int_int/) | Belirtilen hücre satır indeksi ve sütun indeksi konumundaki Cell öğesini alır. |
| [Get_String](./get_string/) | Belirtilen hücre adındaki Cell öğesini alır. |
| [GetMultiThreadReading](./getmultithreadreading/) | Hücre veri modelinin Çoklu İş Parçacığı okumasını destekleyip desteklemeyeceğini alır veya ayarlar. Bu özelliğin varsayılan değeri false'tur. |
| [SetMultiThreadReading](./setmultithreadreading/) | Hücre veri modelinin Çoklu İş Parçacığı okumasını destekleyip desteklemeyeceğini alır veya ayarlar. Bu özelliğin varsayılan değeri false'tur. |
| [GetMemorySetting](./getmemorysetting/) | Bu hücreler için bellek kullanımı seçeneğini alır veya ayarlar. |
| [SetMemorySetting](./setmemorysetting/) | Bu hücreler için bellek kullanımı seçeneğini alır veya ayarlar. |
| [Clear](./clear/) | Çalışma sayfasının tüm verilerini temizler. |
| [GetStyle](./getstyle/) | Çalışma sayfasının varsayılan stilini alır ve ayarlar. |
| [SetStyle](./setstyle/) | Çalışma sayfasının varsayılan stilini alır ve ayarlar. |
|[IsDefaultColumnHidden](./isdefaultcolumnhidden/) |  | 
|[SetIsDefaultColumnHidden](./setisdefaultcolumnhidden/) |  | 
| [GetStandardWidthInch](./getstandardwidthinch/) | Çalışma sayfasındaki varsayılan sütun genişliğini inç biriminde alır veya ayarlar. |
| [SetStandardWidthInch](./setstandardwidthinch/) | Çalışma sayfasındaki varsayılan sütun genişliğini inç biriminde alır veya ayarlar. |
| [GetStandardWidthPixels](./getstandardwidthpixels/) | Çalışma sayfasındaki varsayılan sütun genişliğini piksel biriminde alır veya ayarlar. |
| [SetStandardWidthPixels](./setstandardwidthpixels/) | Çalışma sayfasındaki varsayılan sütun genişliğini piksel biriminde alır veya ayarlar. |
| [GetStandardWidth](./getstandardwidth/) | Çalışma sayfasındaki varsayılan sütun genişliğini karakter biriminde alır veya ayarlar. |
| [SetStandardWidth](./setstandardwidth/) | Çalışma sayfasındaki varsayılan sütun genişliğini karakter biriminde alır veya ayarlar. |
| [GetStandardHeight](./getstandardheight/) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini puan biriminde alır veya ayarlar. |
| [SetStandardHeight](./setstandardheight/) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini puan biriminde alır veya ayarlar. |
| [GetStandardHeightPixels](./getstandardheightpixels/) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini piksel biriminde alır veya ayarlar. |
| [SetStandardHeightPixels](./setstandardheightpixels/) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini piksel biriminde alır veya ayarlar. |
| [GetStandardHeightInch](./getstandardheightinch/) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini inç biriminde alır veya ayarlar. |
| [SetStandardHeightInch](./setstandardheightinch/) | Bu çalışma sayfasındaki varsayılan satır yüksekliğini inç biriminde alır veya ayarlar. |
| [ImportFormulaArray](./importformulaarray/) | Bir çalışma sayfasına formül dizisi aktarır. |
| [TextToColumns](./texttocolumns/) | Belirtilen sütundaki içeriği birden fazla sütuna böler.. |
| [ImportCSV_String_String_Bool_Int_Int](./importcsv_string_string_bool_int_int/) | Hücrelere bir CSV dosyası aktar. |
| [ImportCSV_Stream_String_Bool_Int_Int](./importcsv_stream_string_bool_int_int/) | Hücrelere bir CSV dosyası aktar. |
| [ImportCSV_String_TxtLoadOptions_Int_Int](./importcsv_string_txtloadoptions_int_int/) | Hücrelere bir CSV dosyası aktar. |
| [ImportCSV_Stream_TxtLoadOptions_Int_Int](./importcsv_stream_txtloadoptions_int_int/) | Hücrelere bir CSV dosyası aktar. |
| [GetPreserveString](./getpreservestring/) | Tüm çalışma sayfası değerlerinin dize olarak korunup korunmayacağını belirten bir değeri alır veya ayarlar. Varsayılan false'tur. |
| [SetPreserveString](./setpreservestring/) | Tüm çalışma sayfası değerlerinin dize olarak korunup korunmayacağını belirten bir değeri alır veya ayarlar. Varsayılan false'tur. |
| [Merge_Int_Int_Int_Int](./merge_int_int_int_int/) | Belirtilen hücre aralığını tek bir hücreye birleştirir. |
| [Merge_Int_Int_Int_Int_Bool](./merge_int_int_int_int_bool/) | Belirtilen hücre aralığını tek bir hücreye birleştirir. |
| [Merge_Int_Int_Int_Int_Bool_Bool](./merge_int_int_int_int_bool_bool/) | Belirtilen hücre aralığını tek bir hücreye birleştirir. |
| [UnMerge](./unmerge/) | Belirtilen birleştirilmiş hücre aralığının birleştirmesini kaldırır. |
| [ClearMergedCells](./clearmergedcells/) | Tüm birleştirilmiş aralıkları temizler. |
| [HideRow](./hiderow/) | Bir satırı gizler. |
| [UnhideRow](./unhiderow/) | Bir satırın gizliliğini kaldırır. |
| [HideRows](./hiderows/) | Birden fazla satırı gizler. |
| [UnhideRows](./unhiderows/) | Gizli satırları gösterir. |
| [SetRowHeightPixel](./setrowheightpixel/) | Satır yüksekliğini piksel biriminde ayarlar. |
| [SetRowHeightInch](./setrowheightinch/) | Satır yüksekliğini inç biriminde ayarlar. |
| [SetRowHeight](./setrowheight/) | Belirtilen satırın yüksekliğini ayarlar. |
| [GetRowHeight_Int_Bool_CellsUnitType](./getrowheight_int_bool_cellsunittype/) | Satır yüksekliğini alır. |
| [GetColumnWidth_Int_Bool_CellsUnitType](./getcolumnwidth_int_bool_cellsunittype/) | Sütun genişliğini alır. |
| [HideColumn](./hidecolumn/) | Bir sütunu gizler. |
| [UnhideColumn](./unhidecolumn/) | Bir sütunu gösterir |
| [HideColumns](./hidecolumns/) | Birden fazla sütunu gizler. |
| [UnhideColumns](./unhidecolumns/) | Birden fazla sütunu gösterir. |
| [GetRowHeight_Int](./getrowheight_int/) | Belirtilen bir satırın yüksekliğini puan biriminde alır. |
| [GetViewRowHeight](./getviewrowheight/) | Belirtilen bir satırın yüksekliğini alır. |
| [GetRowHeightInch](./getrowheightinch/) | Belirtilen bir satırın yüksekliğini inç biriminde alır. |
| [GetViewRowHeightInch](./getviewrowheightinch/) | Belirtilen bir satırın yüksekliğini inç biriminde alır. |
| [GetRowHeightPixel](./getrowheightpixel/) | Belirtilen bir satırın yüksekliğini piksel biriminde alır. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | Normal görünümde sütun genişliğini piksel biriminde ayarlar. |
| [SetColumnWidthInch](./setcolumnwidthinch/) | Normal görünümde sütun genişliğini inç biriminde ayarlar. |
| [SetColumnWidth](./setcolumnwidth/) | Normal görünümde belirtilen sütunun genişliğini ayarlar. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | Normal görünümde belirtilen sütunun genişliğini piksel biriminde alır. |
| [GetColumnWidth_Int](./getcolumnwidth_int/) | Normal görünümde belirtilen sütunun genişliğini (karakter biriminde) alır |
| [GetViewColumnWidthPixel](./getviewcolumnwidthpixel/) | Farklı görünüm tipinde genişliği al. |
| [SetViewColumnWidthPixel](./setviewcolumnwidthpixel/) | Farklı görünümde sütunun genişliğini ayarlar. |
| [GetMinRow](./getminrow/) | Veri veya stil içeren hücrenin minimum satır indeksi. |
| [GetMaxRow](./getmaxrow/) | Veri veya stil içeren hücrenin maksimum satır indeksi. |
| [GetMinColumn](./getmincolumn/) | Koleksiyonda örneklenmiş hücrelerin minimum sütun indeksi (tam sütun için stil tanımlı olup, içinde hücre örneklenmemiş sütunlar dahil değildir). |
| [GetMaxColumn](./getmaxcolumn/) | Koleksiyonda örneklenmiş hücrelerin maksimum sütun indeksi (tam sütun için stil tanımlı ancak içinde hücre örneklenmemiş sütunu içermez). |
| [GetMinDataRow](./getmindatarow/) | Veri içeren hücrenin minimum satır indeksi. |
| [GetMaxDataRow](./getmaxdatarow/) | Veri içeren hücrenin maksimum satır indeksi. |
| [GetMinDataColumn](./getmindatacolumn/) | Veri içeren hücrenin minimum sütun indeksi. |
| [GetMaxDataColumn](./getmaxdatacolumn/) | Veri içeren hücrenin maksimum sütun indeksi. |
| [GetLastDataRow](./getlastdatarow/) | Belirtilen sütunda veri içeren hücrenin son satır indeksini alır. |
| [GetFirstDataRow](./getfirstdatarow/) | Belirtilen sütunda veri içeren hücrenin ilk satır indeksini alır. |
| [IsDefaultRowHeightMatched](./isdefaultrowheightmatched/) | Satır yüksekliğinin ve varsayılan yazı tipi yüksekliğinin eşleştiğini gösterir |
| [SetIsDefaultRowHeightMatched](./setisdefaultrowheightmatched/) | Satır yüksekliğinin ve varsayılan yazı tipi yüksekliğinin eşleştiğini gösterir |
| [IsDefaultRowHidden](./isdefaultrowhidden/) | Satırın varsayılan olarak gizli olup olmadığını gösterir. |
| [SetIsDefaultRowHidden](./setisdefaultrowhidden/) | Satırın varsayılan olarak gizli olup olmadığını gösterir. |
| [GetColumns](./getcolumns/) | Bu çalışma sayfasındaki bireysel sütunları temsil eden **Column** nesnelerinin koleksiyonunu alır. |
| [ApplyColumnStyle](./applycolumnstyle/) | Bir bütün sütun için biçimleri uygular. |
| [ApplyRowStyle](./applyrowstyle/) | Bir bütün satır için biçimleri uygular. |
| [ApplyStyle](./applystyle/) | Bir bütün çalışma sayfası için biçimleri uygular. |
| [CopyColumns_Cells_Int_Int_Int_PasteOptions](./copycolumns_cells_int_int_int_pasteoptions/) | Bir bütün sütunun veri ve biçimlerini kopyalar. |
| [CopyColumn](./copycolumn/) | Bir bütün sütunun veri ve biçimlerini kopyalar. |
| [CopyColumns_Cells_Int_Int_Int](./copycolumns_cells_int_int_int/) | Tam sütunların veri ve biçimlerini kopyalar. |
| [CopyColumns_Cells_Int_Int_Int_Int](./copycolumns_cells_int_int_int_int/) | Tam sütunların veri ve biçimlerini kopyalar. |
| [CopyRow](./copyrow/) | Bir bütün satırın veri ve biçimlerini kopyalar. |
| [CopyRows_Cells_Int_Int_Int](./copyrows_cells_int_int_int/) | Bazı bütün satırların veri ve biçimlerini kopyalar. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions](./copyrows_cells_int_int_int_copyoptions/) | Bazı bütün satırların veri ve biçimlerini kopyalar. |
| [CopyRows_Cells_Int_Int_Int_CopyOptions_PasteOptions](./copyrows_cells_int_int_int_copyoptions_pasteoptions/) | Bazı bütün satırların veri ve biçimlerini kopyalar. |
| [GetGroupedRowOutlineLevel](./getgroupedrowoutlinelevel/) | Satırın taslak seviyesini (sıfır tabanlı) alır. |
| [GetGroupedColumnOutlineLevel](./getgroupedcolumnoutlinelevel/) | Sütunun taslak seviyesini (sıfır tabanlı) alır. |
| [GetMaxGroupedColumnOutlineLevel](./getmaxgroupedcolumnoutlinelevel/) | Maksimum gruplanmış sütun taslak seviyesini (sıfır tabanlı) alır. |
| [GetMaxGroupedRowOutlineLevel](./getmaxgroupedrowoutlinelevel/) | Maksimum gruplanmış satır taslak seviyesini (sıfır tabanlı) alır. |
| [ShowGroupDetail](./showgroupdetail/) | Gruplanmış satırları/sütunları genişletir. |
| [HideGroupDetail](./hidegroupdetail/) | Gruplanmış satırları/sütunları daraltır. |
| [UngroupColumns](./ungroupcolumns/) | Sütunların grubunu kaldırır. |
| [GroupColumns_Int_Int](./groupcolumns_int_int/) | Sütunları gruplar. |
| [GroupColumns_Int_Int_Bool](./groupcolumns_int_int_bool/) | Sütunları gruplar. |
| [UngroupRows_Int_Int_Bool](./ungrouprows_int_int_bool/) | Satırların gruplamasını kaldırır. |
| [UngroupRows_Int_Int](./ungrouprows_int_int/) | Satırların gruplamasını kaldırır. |
| [GroupRows_Int_Int_Bool](./grouprows_int_int_bool/) | Satırları gruplar. |
| [GroupRows_Int_Int](./grouprows_int_int/) | Satırları gruplar. |
| [DeleteColumn_Int_Bool](./deletecolumn_int_bool/) | Bir sütunu siler. |
| [DeleteColumn_Int](./deletecolumn_int/) | Bir sütunu siler. |
| [DeleteColumns_Int_Int_Bool](./deletecolumns_int_int_bool/) | Birçok sütunu siler. |
| [DeleteColumns_Int_Int_DeleteOptions](./deletecolumns_int_int_deleteoptions/) | Birçok sütunu siler. |
| [IsDeletingRangeEnabled](./isdeletingrangeenabled/) | Aralığın silinebilir olup olmadığını kontrol eder. |
| [DeleteRow_Int](./deleterow_int/) | Bir satırı siler. |
| [DeleteRow_Int_Bool](./deleterow_int_bool/) | Bir satırı siler. |
| [DeleteRows_Int_Int](./deleterows_int_int/) | Birden fazla satırı siler. |
| [DeleteRows_Int_Int_Bool](./deleterows_int_int_bool/) | Çalışma sayfasındaki birden fazla satırı siler. |
| [DeleteRows_Int_Int_DeleteOptions](./deleterows_int_int_deleteoptions/) | Çalışma sayfasındaki birden fazla satırı siler. |
| [DeleteBlankColumns](./deleteblankcolumns/) | Veri içermeyen tüm boş sütunları sil. |
| [DeleteBlankColumns_DeleteOptions](./deleteblankcolumns_deleteoptions/) | Veri içermeyen tüm boş sütunları sil. |
| [IsBlankColumn](./isblankcolumn/) | Verilen sütunun boş olup olmadığını (veri içermediğini) kontrol eder. |
| [DeleteBlankRows](./deleteblankrows/) | Veri veya başka bir nesne içermeyen tüm boş satırları sil. |
| [DeleteBlankRows_DeleteOptions](./deleteblankrows_deleteoptions/) | Veri veya görünür yorum, özet tablo gibi bazı özel nesneler içermeyen tüm boş satırları sil. |
| [InsertColumns_Int_Int](./insertcolumns_int_int/) | Çalışma sayfasına bazı sütunlar ekler. |
| [InsertColumns_Int_Int_Bool](./insertcolumns_int_int_bool/) | Çalışma sayfasına bazı sütunlar ekler. |
| [InsertColumns_Int_Int_InsertOptions](./insertcolumns_int_int_insertoptions/) | Çalışma sayfasına bazı sütunlar ekler. |
| [InsertColumn_Int_Bool](./insertcolumn_int_bool/) | Çalışma sayfasına yeni bir sütun ekler. |
| [InsertColumn_Int](./insertcolumn_int/) | Çalışma sayfasına yeni bir sütun ekler. |
| [InsertRows_Int_Int_Bool](./insertrows_int_int_bool/) | Çalışma sayfasına birden fazla satır ekler. |
| [InsertRows_Int_Int_InsertOptions](./insertrows_int_int_insertoptions/) | Çalışma sayfasına birden fazla satır ekler. |
| [InsertRows_Int_Int](./insertrows_int_int/) | Çalışma sayfasına birden fazla satır ekler. |
| [InsertRow](./insertrow/) | Çalışma sayfasına yeni bir satır ekler. |
| [GetRanges](./getranges/) | Çalışma zamanında oluşturulan Range nesnelerinin koleksiyonunu alır. |
| [ClearRange_CellArea](./clearrange_cellarea/) | Bir aralığın içeriğini ve biçimlendirmesini temizler. |
| [ClearRange_Int_Int_Int_Int](./clearrange_int_int_int_int/) | Bir aralığın içeriğini ve biçimlendirmesini temizler. |
| [ClearContents_CellArea](./clearcontents_cellarea/) | Bir aralığın içeriğini temizler. |
| [ClearContents_Int_Int_Int_Int](./clearcontents_int_int_int_int/) | Bir aralığın içeriğini temizler. |
| [ClearFormats_CellArea](./clearformats_cellarea/) | Bir aralığın biçimlendirmesini temizler. |
| [ClearFormats_Int_Int_Int_Int](./clearformats_int_int_int_int/) | Bir aralığın biçimlendirmesini temizler. |
| [GetLastCell](./getlastcell/) | Bu çalışma sayfasındaki son hücreyi alır. |
| [LinkToXmlMap](./linktoxmlmap/) | Bir XML haritasına bağla. |
| [GetMaxDisplayRange](./getmaxdisplayrange/) | Veri, birleştirilmiş hücreler ve şekiller içeren maksimum aralığı alır. |
| [GetFirstCell](./getfirstcell/) | Bu çalışma sayfasındaki ilk hücreyi alır. |
| [Find_Object_Cell](./find_object_cell/) | Girdi nesnesiyle içeren hücreyi bulur. |
| [Find_Object_Cell_FindOptions](./find_object_cell_findoptions/) | Girdi nesnesiyle içeren hücreyi bulur. |
| [EndCellInRow_Int](./endcellinrow_int/) | Bu satırdaki son hücreyi alır. |
| [EndCellInColumn_Int](./endcellincolumn_int/) | Bu sütundaki son hücreyi alır. |
| [EndCellInColumn_Int_Int_Int_Int](./endcellincolumn_int_int_int_int/) | Bu aralıktaki maksimum sütun indeksine sahip son hücreyi alır. |
| [EndCellInRow_Int_Int_Int_Int](./endcellinrow_int_int_int_int/) | Bu aralıktaki maksimum satır indeksine sahip son hücreyi alır. |
| [MoveRange](./moverange/) | Aralığı taşır. |
| [InsertCutCells](./insertcutcells/) | Kesilen aralığı ekle. |
| [InsertRange_CellArea_Int_ShiftType_Bool](./insertrange_cellarea_int_shifttype_bool/) | Bir hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [InsertRange_CellArea_ShiftType](./insertrange_cellarea_shifttype/) | Bir hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [InsertRange_CellArea_Int_ShiftType](./insertrange_cellarea_int_shifttype/) | Bir hücre aralığını ekler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [DeleteRange](./deleterange/) | Bir hücre aralığını siler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [ExportArray](./exportarray/) | Hücreler koleksiyonundaki verileri iki boyutlu dizi nesnesine dışa aktarır. |
| [RetrieveSubtotalSetting](./retrievesubtotalsetting/) | Aralığın ara toplam ayarlarını alır. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array](./subtotal_cellarea_int_consolidationfunction_int32array/) | Aralık için ara toplamlar oluşturur. |
| [Subtotal_CellArea_Int_ConsolidationFunction_int32Array_Bool_Bool_Bool](./subtotal_cellarea_int_consolidationfunction_int32array_bool_bool_bool/) | Aralık için ara toplamlar oluşturur. |
| [RemoveFormulas](./removeformulas/) | Tüm formülleri kaldırır ve formülün değeriyle değiştirir. |
| [RemoveDuplicates](./removeduplicates/) | Sayfadaki yinelenen satırları kaldırır. |
| [RemoveDuplicates_Int_Int_Int_Int](./removeduplicates_int_int_int_int/) | Aralıktaki yinelenen değerleri kaldırır. |
| [RemoveDuplicates_Int_Int_Int_Int_Bool_int32Array](./removeduplicates_int_int_int_int_bool_int32array/) | Aralığın yinelenen verilerini kaldırır. |
| [ConvertStringToNumericValue](./convertstringtonumericvalue/) | Çalışma sayfasındaki tüm metin verilerini mümkünse sayısal değere dönüştürür. |
| [GetDependents](./getdependents/) | Belirli hücreye başvuran tüm hücreleri al. |
| [GetDependentsInCalculation](./getdependentsincalculation/) | Hesaplanan sonucunun belirli hücreye bağlı olduğu tüm hücreleri alır. |
| [GetCellsWithPlaceInCellPicture](./getcellswithplaceincellpicture/) | Gömülü resim içeren tüm hücreleri alır. |
| [GetCellStyle](./getcellstyle/) | Verilen hücrenin stilini al. |
| [GetCellDisplayStyle_Int_Int](./getcelldisplaystyle_int_int/) | Verilen hücrenin görüntü stilini al. |
| [GetCellDisplayStyle_Int_Int_BorderType](./getcelldisplaystyle_int_int_bordertype/) | Verilen hücrenin görüntü stilini al. |
