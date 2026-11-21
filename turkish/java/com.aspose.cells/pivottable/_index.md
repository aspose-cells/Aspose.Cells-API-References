---
title: "PivotTable"
second_title: "Aspose.Cells for Java API Referansı"
description: "PivotTable için özet açıklama."
type: docs
url: /tr/java/com.aspose.cells/pivottable/
---

**Inheritance:**
java.lang.Object
```
public class PivotTable
```

PivotTable için özet açıklama.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
          PivotTableCalculateOption calculateOption = new PivotTableCalculateOption();
          calculateOption.setRefreshData(true);
          calculateOption.setRefreshCharts(true);
          pivot.calculateData(calculateOption); 
 
         //do your business
 
         book.save("out.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addCalculatedField(String name, String formula)](#addCalculatedField-java.lang.String-java.lang.String-) | Hesaplanmış bir alanı pivot alanına ekler ve veri alanına sürükler. |
| [addCalculatedField(String name, String formula, boolean dragToDataArea)](#addCalculatedField-java.lang.String-java.lang.String-boolean-) | Hesaplanmış bir alanı pivot alanına ekler. |
| [addFieldToArea(int fieldType, PivotField pivotField)](#addFieldToArea-int-com.aspose.cells.PivotField-) | Alanı belirli alana ekler. |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Alanı belirli alana ekler. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Alanı belirli alana ekler. |
| [calculateData()](#calculateData--) | PivotTable verilerini hücrelere hesaplar. |
| [calculateData(PivotTableCalculateOption option)](#calculateData-com.aspose.cells.PivotTableCalculateOption-) | Seçeneklerle pivot tabloyu hesaplar. |
| [calculateRange()](#calculateRange--) | PivotTable aralığını hesaplar. |
| [changeDataSource(String[] source)](#changeDataSource-java.lang.String---) | Pivot tablonun veri kaynağını değiştir. |
| [clearAll()](#clearAll--) | Bölgelerden tüm alanları kaldır. |
| [clearData()](#clearData--) | PivotTable görünümünün veri ve biçimlendirmesini temizle. |
| [clearFilters()](#clearFilters--) | Bu pivot tablonun tüm filtrelerini temizler. |
| [copyStyle(PivotTable pivotTable)](#copyStyle-com.aspose.cells.PivotTable-) | Başka bir pivot tabloyündan adlandırılmış stili kopyalar. |
| [dispose()](#dispose--) | Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportViewToJson(PivotViewToJsonOptions options)](#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-) | Pivot görünümünü JSON olarak dışa aktarır. |
| [fields(int fieldType)](#fields-int-) | Alan türüne göre belirli alanları alır. |
| [format(CellArea ca, Style style)](#format-com.aspose.cells.CellArea-com.aspose.cells.Style-) | PivotTable'ın seçili alanını biçimlendirir. |
| [format(PivotArea pivotArea, Style style)](#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-) | PivotTable'ın seçili alanını biçimlendirir. |
| [format(int row, int column, Style style)](#format-int-int-com.aspose.cells.Style-) | PivotTable alanındaki hücreyi biçimlendirir |
| [formatAll(Style style)](#formatAll-com.aspose.cells.Style-) | PivotTable alanındaki tüm hücreleri biçimlendirir |
| [formatRow(int row, Style style)](#formatRow-int-com.aspose.cells.Style-) | PivotTable alanındaki satır verilerini biçimlendirir |
| [getAllowMultipleFiltersPerField()](#getAllowMultipleFiltersPerField--) | Bir PivotTable alanının birden çok filtreye sahip olup olamayacağını gösteren bir boolean değer belirler. |
| [getAltTextDescription()](#getAltTextDescription--) | Alt metnin açıklamasını alır. |
| [getAltTextTitle()](#getAltTextTitle--) | Alt metnin başlığını alır. |
| [getAutoFormatType()](#getAutoFormatType--) | PivotTable'ın otomatik biçim türünü alır. |
| [getAutofitColumnWidthOnUpdate()](#getAutofitColumnWidthOnUpdate--) | Güncelleme sırasında sütun genişliğinin otomatik ayarlanıp ayarlanmayacağını gösterir |
| [getBaseFields()](#getBaseFields--) | PivotTable'daki tüm temel pivot alanlarını döndürür. |
| [getButtonArea(int axisType)](#getButtonArea-int-) | Alan düğmesini içeren bölgeyi alır. |
| [getCellByDisplayName(String displayName)](#getCellByDisplayName-java.lang.String-) | PivotField'ın görüntüleme adıyla [Cell](../../com.aspose.cells/cell) nesnesini alır. |
| [getChildren()](#getChildren--) | Bu PivotTable verisini veri kaynağı olarak kullanan alt PivotTable'ları alır. |
| [getClass()](#getClass--) |  |
| [getColumnFields()](#getColumnFields--) | Şu anda sütun alanları olarak gösterilen bir PivotFields nesnesini döndürür. |
| [getColumnGrand()](#getColumnGrand--) | PivotTable raporunun sütunlar için genel toplamları gösterip göstermediğini belirtir. |
| [getColumnHeaderCaption()](#getColumnHeaderCaption--) | PivotTable'ın sütun başlığının özel başlığını alır. |
| [getColumnRange()](#getColumnRange--) | PivotTable raporundaki sütun alanını içeren aralığı temsil eden bir CellArea nesnesini döndürür. |
| [getConditionalFormats()](#getConditionalFormats--) | Pivot tablonun koşullu biçimlendirmelerini alır. |
| [getCustomListSort()](#getCustomListSort--) | Veri sıralanırken yerleşik özel listenin dikkate alınıp alınmayacağını gösterir |
| [getDataBodyRange()](#getDataBodyRange--) | Başlık satırı ile ek satır arasındaki listede veri alanını içeren aralığı temsil eden bir [CellArea](../../com.aspose.cells/cellarea) nesnesini döndürür. |
| [getDataField()](#getDataField--) | Bir PivotTable'daki tüm veri alanlarını temsil eden bir [PivotField](../../com.aspose.cells/pivotfield) nesnesini alır. |
| [getDataFieldHeaderName()](#getDataFieldHeaderName--) | PivotTable'daki değer alanı başlığının adını alır. |
| [getDataFields()](#getDataFields--) | PivotTable'daki tüm veri alanlarını temsil eden bir [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) alır. |
| [getDataSource()](#getDataSource--) | PivotTable'ın veri kaynağını alır. |
| [getDependentPivotTables()](#getDependentPivotTables--) | Bu PivotTable'ı veri kaynağı olarak kullanan tüm [PivotTable](../../com.aspose.cells/pivottable)s alır. |
| [getDisplayErrorString()](#getDisplayErrorString--) | PivotTable raporunun hatalı hücrelerde özel bir dize gösterip göstermediğini belirtir. |
| [getDisplayImmediateItems()](#getDisplayImmediateItems--) | PivotTable'ın veri alanı boş olduğunda satır ve sütun alanlarındaki öğelerin görünür olup olmadığını belirtir. |
| [getDisplayNullString()](#getDisplayNullString--) | PivotTable raporunun değer null olduğunda özel bir dize gösterip göstermediğini belirtir. |
| [getEnableDataValueEditing()](#getEnableDataValueEditing--) | Kullanıcının pivottable veri alanındaki hücreleri düzenleyip düzenleyemeyeceğini belirten bir boolean değer belirtir. |
| [getEnableDrilldown()](#getEnableDrilldown--) | Drilldown'un etkin olup olmadığını belirtir. |
| [getEnableFieldDialog()](#getEnableFieldDialog--) | Kullanıcı PivotTable alanına çift tıkladığında PivotTable Alanı iletişim kutusunun mevcut olup olmadığını belirtir. |
| [getEnableFieldList()](#getEnableFieldList--) | Excel görünümünde PivotTable için alan listesinin mevcut olup olmadığını belirtir. |
| [getEnableWizard()](#getEnableWizard--) | PivotTable Sihirbazının mevcut olup olmadığını belirtir. |
| [getErrorString()](#getErrorString--) | DisplayErrorString özelliği true olduğunda hatalı hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir. |
| [getExternalConnectionDataSource()](#getExternalConnectionDataSource--) | Harici bağlantı veri kaynağını alır. |
| [getFieldListSortAscending()](#getFieldListSortAscending--) | PivotTable'daki alanların alan listesinde varsayılan olmayan bir sırayla sıralanıp sıralanmadığını belirtir. |
| [getFields(int fieldType)](#getFields-int-) | Bölgeye göre belirli pivot alan listesini alır. |
| [getFilterArea()](#getFilterArea--) | Filtre bölgesi alanını alır. |
| [getGrandTotalName()](#getGrandTotalName--) | Genel toplam sütun veya satır başlığında gösterilen etiketi döndürür. |
| [getHorizontalBreaks()](#getHorizontalBreaks--) | pivot table yatay sayfa sonlarının satır indeks listesini alır. |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | Bu pivot table'ın yatay sayfa sonlarını alır. |
| [getIndent()](#getIndent--) | Kompakt eksen için girinti artışını belirtir ve Rapor Düzeni'ni Kompakt Formata ayarlamak için kullanılabilir. |
| [getItemPrintTitles()](#getItemPrintTitles--) | PivotItem adlarının her basılan sayfanın üst kısmında tekrarlanıp tekrarlanmayacağını belirtir. |
| [getManualUpdate()](#getManualUpdate--) | PivotTable raporunun yalnızca kullanıcının isteği üzerine yeniden hesaplanıp hesaplanmayacağını belirtir. |
| [getMergeLabels()](#getMergeLabels--) | Birden fazla hücreyi kapsayan satır/sütun alan etiketlerinin birleştirilip birleştirilmeyeceğini alır. |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Bir PivotTable alanının birden çok filtreye sahip olup olamayacağını gösteren bir boolean değer belirler. |
| [getName()](#getName--) | PivotTable'ın adını alır. |
| [getNamesOfSourceDataConnections()](#getNamesOfSourceDataConnections--) | Harici kaynak veri bağlantılarının adlarını alır. |
| [getNullString()](#getNullString--) | DisplayNullString özelliği true olduğunda null değer içeren hücrelerde görüntülenen dizeyi alır. Varsayılan değer boş bir dizedir. |
| [getPageFieldOrder()](#getPageFieldOrder--) | Sayfa alanlarının PivotTable raporunun düzenine eklendiği sıralamayı alır. |
| [getPageFieldWrapCount()](#getPageFieldWrapCount--) | PivotTable raporundaki her sütun veya satırdaki sayfa alanı sayısını alır. |
| [getPageFields()](#getPageFields--) | Şu anda sayfa alanı olarak gösterilen bir [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) döndürür. |
| [getPivotCache()](#getPivotCache--) | Veri kaynağını alır. |
| [getPivotFilters()](#getPivotFilters--) | Pivot tabloda bulunan tüm filtreleri döndürür. |
| [getPivotFormatConditions()](#getPivotFormatConditions--) | Pivot tablonun Biçim Koşullarını alır. |
| [getPivotFormats()](#getPivotFormats--) | Bu pivot tabloya uygulanan tüm hücre biçimlerini alır. |
| [getPivotTableStyle()](#getPivotTableStyle--) | Bu pivot tablonun [TableStyle](../../com.aspose.cells/tablestyle) ayarlarını alır. |
| [getPivotTableStyleName()](#getPivotTableStyleName--) | Pivot tablonun stil adını alır. |
| [getPivotTableStyleType()](#getPivotTableStyleType--) | Yerleşik pivot tablo stilini alır. |
| [getPivotTablesWithSamePivotCache()](#getPivotTablesWithSamePivotCache--) | Aynı pivot önbelleğine sahip tüm pivot tabloları alır. |
| [getPreserveCellFormattingOnUpdate()](#getPreserveCellFormattingOnUpdate--) | Pivot tablo yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesinin ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) korunup korunmayacağını gösterir. |
| [getPreserveFormatting()](#getPreserveFormatting--) | PivotTable yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesinin ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) korunup korunmadığını gösterir. |
| [getPrintDrill()](#getPrintDrill--) | Delme göstergelerinin yazdırılıp yazdırılmayacağını belirten bir boolean değer belirtir. |
| [getPrintTitles()](#getPrintTitles--) | Çalışma sayfası için yazdırma başlıklarının PivotTable raporuna göre ayarlanıp ayarlanmadığını gösterir. |
| [getRefreshDataOnOpeningFile()](#getRefreshDataOnOpeningFile--) | Dosya açılırken Veri Yenileme'nin yapılması gerekip gerekmediğini gösterir. |
| [getRefreshDate()](#getRefreshDate--) | PivotTable'ın en son yenilendiği tarih ve saati alır. |
| [getRefreshedByWho()](#getRefreshedByWho--) | Bu PivotTable'ı en son yenileyen kullanıcının adını alır. |
| [getRepeatItemsOnEachPrintedPage()](#getRepeatItemsOnEachPrintedPage--) | Satır alanındaki pivot öğesi başlıklarının tablo biçimindeki pivot alanları için her yazdırılan sayfada tekrarlanıp tekrarlanmadığını gösterir. |
| [getRowFields()](#getRowFields--) | Şu anda satır alanı olarak gösterilen bir [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) döndürür. |
| [getRowGrand()](#getRowGrand--) | Bu pivot tablonun satırları için genel toplamların gösterilip gösterilmeyeceğini belirtir. |
| [getRowHeaderCaption()](#getRowHeaderCaption--) | Bu PivotTable'daki Satır Başlığının özel başlığını alır. |
| [getRowRange()](#getRowRange--) | PivotTable raporundaki satır alanını içeren aralığı temsil eden bir CellArea nesnesi döndürür. |
| [getSaveData()](#getSaveData--) | PivotTable raporu için verilerin çalışma kitabıyla birlikte kaydedilip kaydedilmediğini gösterir. |
| [getShowColumnGrandTotals()](#getShowColumnGrandTotals--) | Bu pivot tablonun sütunları için genel toplamların gösterilip gösterilmeyeceğini gösterir. |
| [getShowDataTips()](#getShowDataTips--) | PivotTable veri hücreleri için araç ipuçlarının gösterilip gösterilmeyeceğini gösterir. |
| [getShowDrill()](#getShowDrill--) | Genişletme/küçültme düğmelerinin gösterilip gösterilmediğini alır. |
| [getShowEmptyCol()](#getShowEmptyCol--) | Tabloda boş sütunların dahil edilip edilmeyeceğini gösterir. |
| [getShowEmptyRow()](#getShowEmptyRow--) | Tabloda boş satırların dahil edililip edilmeyeceğini gösterir. |
| [getShowHeaders()](#getShowHeaders--) | Satır ekseninde ve sütun ekseninde PivotTable görünümünde veri alanı başlıklarını ve pivot alanı başlıklarını gösterip göstermeyeceği. |
| [getShowMemberPropertyTips()](#getShowMemberPropertyTips--) | Üye özelliği bilgilerinin PivotTable araç ipuçlarından çıkarılıp çıkarılmayacağını gösteren bir boolean değer belirtir. |
| [getShowPivotStyleColumnHeader()](#getShowPivotStyleColumnHeader--) | Pivot tabloda sütun başlığının stile uygulanıp uygulanmayacağını gösterir. |
| [getShowPivotStyleColumnStripes()](#getShowPivotStyleColumnStripes--) | Sütun için çizgili biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [getShowPivotStyleLastColumn()](#getShowPivotStyleLastColumn--) | Sütun biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [getShowPivotStyleRowHeader()](#getShowPivotStyleRowHeader--) | Pivot tabloda satır başlığının stile uygulanıp uygulanmayacağını gösterir. |
| [getShowPivotStyleRowStripes()](#getShowPivotStyleRowStripes--) | Satır çizgili biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [getShowRowGrandTotals()](#getShowRowGrandTotals--) | Pivot tablonun satırları için genel toplamların gösterilip gösterilmeyeceğini gösterir. |
| [getShowRowHeaderCaption()](#getShowRowHeaderCaption--) | PivotTable raporunda satır başlığı açıklamasının gösterilip gösterilmediğini ve alan başlıklarının ve filtre açılır menülerinin görüntülenip görüntülenmediğini gösterir. |
| [getShowValuesRow()](#getShowValuesRow--) | Değer satırının gösterilip gösterilmediğini gösterir. |
| [getSource()](#getSource--) | Bu pivot tablonun veri kaynağını alır. |
| [getSource(boolean isOriginal)](#getSource-boolean-) | Bu pivot tablonun veri kaynağını alır. |
| [getSourceDataConnections()](#getSourceDataConnections--) | Harici bağlantı veri kaynaklarını alır. |
| [getSourceType()](#getSourceType--) | Pivot tablonun veri kaynağı türünü alır. |
| [getSubtotalHiddenPageItems()](#getSubtotalHiddenPageItems--) | PivotTable raporundaki gizli sayfa alanı öğelerinin satır ve sütun alt toplamlarına, blok toplamlarına ve genel toplamlarına dahil edilip edilmediğini gösterir. |
| [getTableRange1()](#getTableRange1--) | Sayfa alanlarını içermeyen, tüm PivotTable raporunu kapsayan aralığı temsil eden bir CellArea nesnesi döndürür. |
| [getTableRange2()](#getTableRange2--) | Sayfa alanlarını içeren, tüm PivotTable raporunu kapsayan aralığı temsil eden bir CellArea nesnesi döndürür. |
| [getTag()](#getTag--) | Bu PivotTable görünümüyle ilişkili kullanıcı tanımlı bir dizeyi alır. |
| [getTopRightArea()](#getTopRightArea--) | PivotTable'ın sağ üst köşesindeki (RTL sayfalar için sol üst) boş alanı temsil eder. |
| [getValuesField()](#getValuesField--) | Bir PivotTable'daki tüm veri alanlarını temsil eden bir [PivotField](../../com.aspose.cells/pivotfield) nesnesini alır. |
| [hasBlankRows()](#hasBlankRows--) | Boş satırların eklenip eklenmeyeceğini gösterir. |
| [hashCode()](#hashCode--) |  |
| [isAutoFormat()](#isAutoFormat--) | PivotTable raporunun otomatik olarak biçimlendirilip biçimlendirilmediğini gösterir. |
| [isExcel2003Compatible()](#isExcel2003Compatible--) | PivotTable yenilenirken PivotTable'ın Excel2003 ile uyumlu olup olmadığını belirtir; doğru ise, bir dize 255 karakterden az veya eşit olmalıdır, bu nedenle dize 255 karakterden uzun olursa kesilir. Yanlış ise, bir dize yukarıda belirtilen kısıtlamaya sahip olmayacaktır. |
| [isGridDropZones()](#isGridDropZones--) | PivotTable raporunun klasik pivottable düzenini gösterip göstermediğini belirtir. |
| [isMultipleFieldFilters()](#isMultipleFieldFilters--) | Bir PivotTable alanının birden çok filtreye sahip olup olamayacağını gösteren bir boolean değer belirler. |
| [isSelected()](#isSelected--) | Bu PivotTable'ın seçili olup olmadığını gösterir. |
| [move(int row, int column)](#move-int-int-) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [move(String destCellName)](#move-java.lang.String-) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [moveItem(int region, String[] nodes, boolean absolute, int offset)](#moveItem-int-java.lang.String---boolean-int-) | Bir öğeyi yukarı veya aşağı hareket ettir. |
| [moveTo(int row, int column)](#moveTo-int-int-) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [moveTo(int sheetIndex, int row, int column)](#moveTo-int-int-int-) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [moveTo(String destCellName)](#moveTo-java.lang.String-) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Veri kaynağından [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) yenileyin ve pivot görünümü için veri ve stili hesaplayın. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Veri kaynağından [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) yenileyin ve pivot görünümü için veri ve stili hesaplayın. |
| [refreshData()](#refreshData--) | Veriyi veri kaynağından pivot önbelleğine yeniler. |
| [refreshData(PivotTableRefreshOption option)](#refreshData-com.aspose.cells.PivotTableRefreshOption-) | Seçeneklerle pivottable'ın verisini ve ayarlarını veri kaynağından yeniler. |
| [removeField(int fieldType, PivotField pivotField)](#removeField-int-com.aspose.cells.PivotField-) | Belirli alan bölgesinden alanı kaldır. |
| [removeField(int fieldType, int baseFieldIndex)](#removeField-int-int-) | Belirli pivot bölgesinden bir alanı kaldırır. |
| [removeField(int fieldType, String fieldName)](#removeField-int-java.lang.String-) | Belirli alan bölgesinden bir alanı kaldırır. |
| [selectArea(CellArea ca)](#selectArea-com.aspose.cells.CellArea-) | Pivot tablo görünümünün bir alanını seç. |
| [setAllowMultipleFiltersPerField(boolean value)](#setAllowMultipleFiltersPerField-boolean-) | Bir PivotTable alanının birden çok filtreye sahip olup olamayacağını gösteren bir boolean değer belirler. |
| [setAltTextDescription(String value)](#setAltTextDescription-java.lang.String-) | Alt metnin açıklamasını alır. |
| [setAltTextTitle(String value)](#setAltTextTitle-java.lang.String-) | Alternatif metnin başlığını ayarlar. |
| [setAutoFormat(boolean value)](#setAutoFormat-boolean-) | PivotTable raporunun otomatik olarak biçimlendirilip biçimlendirilmediğini gösterir. |
| [setAutoFormatType(int value)](#setAutoFormatType-int-) | PivotTable'ın otomatik biçim türünü ayarlar. |
| [setAutofitColumnWidthOnUpdate(boolean value)](#setAutofitColumnWidthOnUpdate-boolean-) | Güncelleme sırasında sütun genişliğinin otomatik ayarlanıp ayarlanmayacağını gösterir |
| [setColumnGrand(boolean value)](#setColumnGrand-boolean-) | PivotTable raporunun sütunlar için genel toplamları gösterip göstermediğini belirtir. |
| [setColumnHeaderCaption(String value)](#setColumnHeaderCaption-java.lang.String-) | PivotTable'ın Sütun Başlığının özel başlığını ayarlar. |
| [setCustomListSort(boolean value)](#setCustomListSort-boolean-) | Veri sıralanırken yerleşik özel listenin dikkate alınıp alınmayacağını gösterir |
| [setDataFieldHeaderName(String value)](#setDataFieldHeaderName-java.lang.String-) | PivotTable'taki değer alanı alan başlığının adını ayarlar. |
| [setDataSource(String[] value)](#setDataSource-java.lang.String---) | Pivot tablonun veri kaynağını ayarlar. |
| [setDisplayErrorString(boolean value)](#setDisplayErrorString-boolean-) | PivotTable raporunun hatalı hücrelerde özel bir dize gösterip göstermediğini belirtir. |
| [setDisplayImmediateItems(boolean value)](#setDisplayImmediateItems-boolean-) | PivotTable'ın veri alanı boş olduğunda satır ve sütun alanlarındaki öğelerin görünür olup olmadığını belirtir. |
| [setDisplayNullString(boolean value)](#setDisplayNullString-boolean-) | PivotTable raporunun değer null olduğunda özel bir dize gösterip göstermediğini belirtir. |
| [setEnableDataValueEditing(boolean value)](#setEnableDataValueEditing-boolean-) | Kullanıcının pivottable veri alanındaki hücreleri düzenleyip düzenleyemeyeceğini belirten bir boolean değer belirtir. |
| [setEnableDrilldown(boolean value)](#setEnableDrilldown-boolean-) | Drilldown'un etkin olup olmadığını belirtir. |
| [setEnableFieldDialog(boolean value)](#setEnableFieldDialog-boolean-) | Kullanıcı PivotTable alanına çift tıkladığında PivotTable Alanı iletişim kutusunun mevcut olup olmadığını belirtir. |
| [setEnableFieldList(boolean value)](#setEnableFieldList-boolean-) | Excel görünümünde PivotTable için alan listesinin mevcut olup olmadığını belirtir. |
| [setEnableWizard(boolean value)](#setEnableWizard-boolean-) | PivotTable Sihirbazının mevcut olup olmadığını belirtir. |
| [setErrorString(String value)](#setErrorString-java.lang.String-) | DisplayErrorString özelliği true olduğunda hatalı hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir. |
| [setExcel2003Compatible(boolean value)](#setExcel2003Compatible-boolean-) | PivotTable yenilenirken PivotTable'ın Excel2003 ile uyumlu olup olmadığını belirtir; doğru ise, bir dize 255 karakterden az veya eşit olmalıdır, bu nedenle dize 255 karakterden uzun olursa kesilir. Yanlış ise, bir dize yukarıda belirtilen kısıtlamaya sahip olmayacaktır. |
| [setFieldListSortAscending(boolean value)](#setFieldListSortAscending-boolean-) | PivotTable'daki alanların alan listesinde varsayılan olmayan bir sırayla sıralanıp sıralanmadığını belirtir. |
| [setGrandTotalName(String value)](#setGrandTotalName-java.lang.String-) | Genel toplam sütun veya satır başlığında gösterilen etiketi döndürür. |
| [setGridDropZones(boolean value)](#setGridDropZones-boolean-) | PivotTable raporunun klasik pivottable düzenini gösterip göstermediğini belirtir. |
| [setHasBlankRows(boolean value)](#setHasBlankRows-boolean-) | Boş satırların eklenip eklenmeyeceğini gösterir. |
| [setIndent(int value)](#setIndent-int-) | Kompakt eksen için girinti artışını belirtir ve Rapor Düzeni'ni Kompakt Formata ayarlamak için kullanılabilir. |
| [setItemPrintTitles(boolean value)](#setItemPrintTitles-boolean-) | PivotItem adlarının her basılan sayfanın üst kısmında tekrarlanıp tekrarlanmayacağını belirtir. |
| [setManualUpdate(boolean value)](#setManualUpdate-boolean-) | PivotTable raporunun yalnızca kullanıcının isteği üzerine yeniden hesaplanıp hesaplanmayacağını belirtir. |
| [setMergeLabels(boolean value)](#setMergeLabels-boolean-) | Birden fazla hücreye yayılan satır/sütun alan etiketlerini birleştirip birleştirilmeyeceğini ayarlar. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Bir PivotTable alanının birden çok filtreye sahip olup olamayacağını gösteren bir boolean değer belirler. |
| [setMultipleFieldFilters(boolean value)](#setMultipleFieldFilters-boolean-) | Bir PivotTable alanının birden çok filtreye sahip olup olamayacağını gösteren bir boolean değer belirler. |
| [setName(String value)](#setName-java.lang.String-) | PivotTable'ın adını alır. |
| [setNullString(String value)](#setNullString-java.lang.String-) | DisplayNullString özelliği true olduğunda null değer içeren hücrelerde görüntülenen dizeyi alır. Varsayılan değer boş bir dizedir. |
| [setPageFieldOrder(int value)](#setPageFieldOrder-int-) | Sayfa alanlarının PivotTable raporunun düzenine eklendiği sıralamayı ayarlar. |
| [setPageFieldWrapCount(int value)](#setPageFieldWrapCount-int-) | PivotTable raporundaki her sütun veya satırdaki sayfa alanı sayısını alır. |
| [setPivotTableStyle(TableStyle value)](#setPivotTableStyle-com.aspose.cells.TableStyle-) | Bu pivot tablonun [TableStyle](../../com.aspose.cells/tablestyle) ayarlarını alır. |
| [setPivotTableStyleName(String value)](#setPivotTableStyleName-java.lang.String-) | Pivot tablonun stil adını ayarlar. |
| [setPivotTableStyleType(int value)](#setPivotTableStyleType-int-) | Yerleşik pivot tablo stilini ayarlar. |
| [setPreserveCellFormattingOnUpdate(boolean value)](#setPreserveCellFormattingOnUpdate-boolean-) | Pivot tablo yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesinin ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) korunup korunmayacağını gösterir. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | PivotTable yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesinin ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) korunup korunmadığını gösterir. |
| [setPrintDrill(boolean value)](#setPrintDrill-boolean-) | Delme göstergelerinin yazdırılıp yazdırılmayacağını belirten bir boolean değer belirtir. |
| [setPrintTitles(boolean value)](#setPrintTitles-boolean-) | Çalışma sayfası için yazdırma başlıklarının PivotTable raporuna göre ayarlanıp ayarlanmadığını gösterir. |
| [setRefreshDataOnOpeningFile(boolean value)](#setRefreshDataOnOpeningFile-boolean-) | Dosya açılırken Veri Yenileme'nin yapılması gerekip gerekmediğini gösterir. |
| [setRepeatItemsOnEachPrintedPage(boolean value)](#setRepeatItemsOnEachPrintedPage-boolean-) | Satır alanındaki pivot öğesi başlıklarının tablo biçimindeki pivot alanları için her yazdırılan sayfada tekrarlanıp tekrarlanmadığını gösterir. |
| [setRowGrand(boolean value)](#setRowGrand-boolean-) | Bu pivot tablonun satırları için genel toplamların gösterilip gösterilmeyeceğini belirtir. |
| [setRowHeaderCaption(String value)](#setRowHeaderCaption-java.lang.String-) | Bu PivotTable'daki Satır Başlığının özel başlığını ayarlar. |
| [setSaveData(boolean value)](#setSaveData-boolean-) | PivotTable raporu için verilerin çalışma kitabıyla birlikte kaydedilip kaydedilmediğini gösterir. |
| [setSelected(boolean value)](#setSelected-boolean-) | Bu PivotTable'ın seçili olup olmadığını gösterir. |
| [setShowColumnGrandTotals(boolean value)](#setShowColumnGrandTotals-boolean-) | Bu pivot tablonun sütunları için genel toplamların gösterilip gösterilmeyeceğini gösterir. |
| [setShowDataTips(boolean value)](#setShowDataTips-boolean-) | PivotTable veri hücreleri için araç ipuçlarının gösterilip gösterilmeyeceğini gösterir. |
| [setShowDrill(boolean value)](#setShowDrill-boolean-) | Genişlet/daralt düğmelerinin gösterilip gösterilmeyeceğini ayarlar. |
| [setShowEmptyCol(boolean value)](#setShowEmptyCol-boolean-) | Tabloda boş sütunların dahil edilip edilmeyeceğini gösterir. |
| [setShowEmptyRow(boolean value)](#setShowEmptyRow-boolean-) | Tabloda boş satırların dahil edililip edilmeyeceğini gösterir. |
| [setShowHeaders(boolean value)](#setShowHeaders-boolean-) | Satır ekseninde ve sütun ekseninde PivotTable görünümünde veri alanı başlıklarını ve pivot alanı başlıklarını gösterip göstermeyeceği. |
| [setShowMemberPropertyTips(boolean value)](#setShowMemberPropertyTips-boolean-) | Üye özelliği bilgilerinin PivotTable araç ipuçlarından çıkarılıp çıkarılmayacağını gösteren bir boolean değer belirtir. |
| [setShowPivotStyleColumnHeader(boolean value)](#setShowPivotStyleColumnHeader-boolean-) | Pivot tabloda sütun başlığının stile uygulanıp uygulanmayacağını gösterir. |
| [setShowPivotStyleColumnStripes(boolean value)](#setShowPivotStyleColumnStripes-boolean-) | Sütun için çizgili biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [setShowPivotStyleLastColumn(boolean value)](#setShowPivotStyleLastColumn-boolean-) | Sütun biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [setShowPivotStyleRowHeader(boolean value)](#setShowPivotStyleRowHeader-boolean-) | Pivot tabloda satır başlığının stile uygulanıp uygulanmayacağını gösterir. |
| [setShowPivotStyleRowStripes(boolean value)](#setShowPivotStyleRowStripes-boolean-) | Satır çizgili biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [setShowRowGrandTotals(boolean value)](#setShowRowGrandTotals-boolean-) | Pivot tablonun satırları için genel toplamların gösterilip gösterilmeyeceğini gösterir. |
| [setShowRowHeaderCaption(boolean value)](#setShowRowHeaderCaption-boolean-) | PivotTable raporunda satır başlığı açıklamasının gösterilip gösterilmediğini ve alan başlıklarının ve filtre açılır menülerinin görüntülenip görüntülenmediğini gösterir. |
| [setShowValuesRow(boolean value)](#setShowValuesRow-boolean-) | Değer satırının gösterilip gösterilmediğini gösterir. |
| [setSubtotalHiddenPageItems(boolean value)](#setSubtotalHiddenPageItems-boolean-) | PivotTable raporundaki gizli sayfa alanı öğelerinin satır ve sütun alt toplamlarına, blok toplamlarına ve genel toplamlarına dahil edilip edilmediğini gösterir. |
| [setTag(String value)](#setTag-java.lang.String-) | Bu PivotTable görünümüyle ilişkili kullanıcı tanımlı bir dize ayarlar. |
| [showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)](#showDetail-int-int-boolean-int-int-) | Veri bölgesindeki bir öğenin ayrıntısını yeni bir Tablo'ya göster. |
| [showInCompactForm()](#showInCompactForm--) | PivotTable görünümünü kompakt biçimde düzenler. |
| [showInOutlineForm()](#showInOutlineForm--) | PivotTable'ı taslak biçimde düzenler. |
| [showInTabularForm()](#showInTabularForm--) | PivotTable'ı tablo biçiminde düzenler. |
| [showReportFilterPage(PivotField pageField)](#showReportFilterPage-com.aspose.cells.PivotField-) | PivotField'e göre tüm rapor filtre sayfalarını göster, PivotField PageFields içinde bulunmalıdır. |
| [showReportFilterPageByIndex(int posIndex)](#showReportFilterPageByIndex-int-) | PageFields içindeki konum indeksine göre tüm rapor filtre sayfalarını göster. |
| [showReportFilterPageByName(String fieldName)](#showReportFilterPageByName-java.lang.String-) | PivotField'in adına göre tüm rapor filtre sayfalarını göster, PivotField PageFields içinde bulunmalıdır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedField(String name, String formula) {#addCalculatedField-java.lang.String-java.lang.String-}
```
public void addCalculatedField(String name, String formula)
```


Hesaplanmış bir alanı pivot alanına ekler ve veri alanına sürükler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Hesaplanan alanın adı |
| formula | java.lang.String | Hesaplanan alanın formülü. |

### addCalculatedField(String name, String formula, boolean dragToDataArea) {#addCalculatedField-java.lang.String-java.lang.String-boolean-}
```
public void addCalculatedField(String name, String formula, boolean dragToDataArea)
```


Hesaplanmış bir alanı pivot alanına ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Hesaplanan alanın adı |
| formula | java.lang.String | Hesaplanan alanın formülü. |
| dragToDataArea | boolean | True, bu alanı hemen veri alanına sürükle |

### addFieldToArea(int fieldType, PivotField pivotField) {#addFieldToArea-int-com.aspose.cells.PivotField-}
```
public int addFieldToArea(int fieldType, PivotField pivotField)
```


Alanı belirli alana ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). alanların bölge türü. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | temel alanlardaki alan. |

**Returns:**
int - belirli alanlardaki alan konumu.
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Alanı belirli alana ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Alanların bölge türü. |
| baseFieldIndex | int | Temel alanlardaki indeks. |

**Returns:**
int - Belirli alanlardaki alan konumu.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Alanı belirli alana ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Alanların bölge türü. |
| fieldName | java.lang.String | Temel alanlardaki ad. |

**Returns:**
int - Belirli alanlardaki alan konumu. Eğer böyle bir alan yoksa, -1 döndür.
### calculateData() {#calculateData--}
```
public void calculateData()
```


PivotTable verilerini hücrelere hesaplar.

**Remarks**

Bu yöntem yalnızca [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) içindeki önbelleğe alınmış verilerle veri hesaplar. Bu nedenle en son veri kaynağıyla hesaplamak istiyorsanız, lütfen [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) yöntemini kullanın. Yalnızca pivot tablo ayarı değiştirildiyse, [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) yeterlidir.

### calculateData(PivotTableCalculateOption option) {#calculateData-com.aspose.cells.PivotTableCalculateOption-}
```
public PivotTable[] calculateData(PivotTableCalculateOption option)
```


Seçeneklerle pivot tabloyu hesaplar.

**Remarks**

Eğer [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) true ise, bu yöntem veri kaynağından pivot önbelleğini yenileyecek ve aynı pivot önbelleğine dayalı tüm pivot tabloları hesaplayacaktır. Aksi takdirde, yalnızca pivot önbelleğindeki önbelleğe alınmış verilerle hesaplama yapılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| option | [PivotTableCalculateOption](../../com.aspose.cells/pivottablecalculateoption) | Pivot tabloyu hesaplamak için seçenekler. |

**Returns:**
com.aspose.cells.PivotTable[] - Hesaplanmış tüm pivot tabloları döndürür. Eğer [PivotTableCalculateOption.getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) true ise, aynı pivot önbelleğine dayalı tüm pivot tablolar birlikte hesaplanacaktır.
### calculateRange() {#calculateRange--}
```
public void calculateRange()
```


PivotTable aralığını hesaplar.

**Remarks**

Bu yöntem çağrılmadıysa, pivot tablo aralığı düzeltilmemiş olabilir.

### changeDataSource(String[] source) {#changeDataSource-java.lang.String---}
```
public void changeDataSource(String[] source)
```


Pivot tablonun veri kaynağını değiştir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | java.lang.String[] |  |

### clearAll() {#clearAll--}
```
public void clearAll()
```


Bölgelerden tüm alanları kaldır.

### clearData() {#clearData--}
```
public void clearData()
```


PivotTable görünümünün veri ve biçimlendirmesini temizle.

**Remarks**

Bu yöntem, PivotField eklemeden veya silmeden önce çağrılmazsa, PivotTable verileri doğru olmayabilir.

### clearFilters() {#clearFilters--}
```
public void clearFilters()
```


Bu pivot tablonun tüm filtrelerini temizler.

### copyStyle(PivotTable pivotTable) {#copyStyle-com.aspose.cells.PivotTable-}
```
public void copyStyle(PivotTable pivotTable)
```


Başka bir pivot tabloyündan adlandırılmış stili kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Kaynak pivot tablo. |

### dispose() {#dispose--}
```
public void dispose()
```


Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür.

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
### exportViewToJson(PivotViewToJsonOptions options) {#exportViewToJson-com.aspose.cells.PivotViewToJsonOptions-}
```
public String exportViewToJson(PivotViewToJsonOptions options)
```


Pivot görünümünü JSON olarak dışa aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [PivotViewToJsonOptions](../../com.aspose.cells/pivotviewtojsonoptions) |  |

**Returns:**
java.lang.String -
### fields(int fieldType) {#fields-int-}
```
public PivotFieldCollection fields(int fieldType)
```


Alan türüne göre belirli alanları alır.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine lütfen PivotField.GetFields(PivotFieldType) yöntemini kullanın. Bu yöntem, Mayıs 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). alan türü. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific field collection
### format(CellArea ca, Style style) {#format-com.aspose.cells.CellArea-com.aspose.cells.Style-}
```
public void format(CellArea ca, Style style)
```


PivotTable'ın seçili alanını biçimlendirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Hücrelerin aralığı. |
| style | [Style](../../com.aspose.cells/style) | Stil |

### format(PivotArea pivotArea, Style style) {#format-com.aspose.cells.PivotArea-com.aspose.cells.Style-}
```
public void format(PivotArea pivotArea, Style style)
```


PivotTable'ın seçili alanını biçimlendirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotArea | [PivotArea](../../com.aspose.cells/pivotarea) | Seçilen pivot görünüm alanı. |
| style | [Style](../../com.aspose.cells/style) | Biçimlendirilmiş ayar. |

### format(int row, int column, Style style) {#format-int-int-com.aspose.cells.Style-}
```
public void format(int row, int column, Style style)
```


PivotTable alanındaki hücreyi biçimlendirir

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Hücrenin satır indeksi |
| sütun | int | Hücrenin sütun indeksi |
| style | [Style](../../com.aspose.cells/style) | Hücere biçim vermek için stil |

### formatAll(Style style) {#formatAll-com.aspose.cells.Style-}
```
public void formatAll(Style style)
```


PivotTable alanındaki tüm hücreleri biçimlendirir

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Biçimlendirmek için stil |

### formatRow(int row, Style style) {#formatRow-int-com.aspose.cells.Style-}
```
public void formatRow(int row, Style style)
```


PivotTable alanındaki satır verilerini biçimlendirir

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır nesnesinin satır indeksi |
| style | [Style](../../com.aspose.cells/style) | Biçimlendirmek için stil |

### getAllowMultipleFiltersPerField() {#getAllowMultipleFiltersPerField--}
```
public boolean getAllowMultipleFiltersPerField()
```


Bir PivotTable alanının birden çok filtreye sahip olup olamayacağını gösteren bir boolean değer belirler.

**Returns:**
boolean
### getAltTextDescription() {#getAltTextDescription--}
```
public String getAltTextDescription()
```


Alt metnin açıklamasını alır.

**Returns:**
java.lang.String
### getAltTextTitle() {#getAltTextTitle--}
```
public String getAltTextTitle()
```


Alt metnin başlığını alır.

**Returns:**
java.lang.String
### getAutoFormatType() {#getAutoFormatType--}
```
public int getAutoFormatType()
```


PivotTable'ın otomatik biçim türünü alır.

Bakınız [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Returns:**
int
### getAutofitColumnWidthOnUpdate() {#getAutofitColumnWidthOnUpdate--}
```
public boolean getAutofitColumnWidthOnUpdate()
```


Güncelleme sırasında sütun genişliğinin otomatik ayarlanıp ayarlanmayacağını gösterir

**Returns:**
boolean
### getBaseFields() {#getBaseFields--}
```
public PivotFieldCollection getBaseFields()
```


PivotTable'daki tüm temel pivot alanlarını döndürür.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getButtonArea(int axisType) {#getButtonArea-int-}
```
public CellArea getButtonArea(int axisType)
```


Alan düğmesini içeren bölgeyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Bölge türü. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - 
### getCellByDisplayName(String displayName) {#getCellByDisplayName-java.lang.String-}
```
public Cell getCellByDisplayName(String displayName)
```


PivotField'ın görüntüleme adıyla [Cell](../../com.aspose.cells/cell) nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| displayName | java.lang.String | PivotField'ın DisplayName'i |

**Returns:**
[Cell](../../com.aspose.cells/cell) - the Cell object
### getChildren() {#getChildren--}
```
public PivotTable[] getChildren()
```


Bu PivotTable verisini veri kaynağı olarak kullanan alt PivotTable'ları alır.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine lütfen PivotTable.GetDependentPivotTables() yöntemini kullanın. Bu yöntem, Nisan 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
com.aspose.cells.PivotTable[] - PivotTable dizi nesnesi
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnFields() {#getColumnFields--}
```
public PivotFieldCollection getColumnFields()
```


Şu anda sütun alanları olarak gösterilen bir PivotFields nesnesini döndürür.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getColumnGrand() {#getColumnGrand--}
```
public boolean getColumnGrand()
```


PivotTable raporunun sütunlar için genel toplamları gösterip göstermediğini belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine lütfen PivotTable.ShowColumnGrandTotals yöntemini kullanın. Bu yöntem, Aralık 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getColumnHeaderCaption() {#getColumnHeaderCaption--}
```
public String getColumnHeaderCaption()
```


PivotTable'ın sütun başlığının özel başlığını alır.

**Returns:**
java.lang.String
### getColumnRange() {#getColumnRange--}
```
public CellArea getColumnRange()
```


PivotTable raporundaki sütun alanını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getConditionalFormats() {#getConditionalFormats--}
```
public PivotConditionalFormatCollection getConditionalFormats()
```


Pivot tablonun koşullu biçimlendirmelerini alır.

**Returns:**
[PivotConditionalFormatCollection](../../com.aspose.cells/pivotconditionalformatcollection)
### getCustomListSort() {#getCustomListSort--}
```
public boolean getCustomListSort()
```


Veri sıralanırken yerleşik özel listenin dikkate alınıp alınmayacağını gösterir

**Returns:**
boolean
### getDataBodyRange() {#getDataBodyRange--}
```
public CellArea getDataBodyRange()
```


Başlık satırı ile ekleme satırı arasındaki listedeki veri alanını içeren aralığı temsil eden bir [CellArea](../../com.aspose.cells/cellarea) nesnesi döndürür. Salt okunur.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getDataField() {#getDataField--}
```
public PivotField getDataField()
```


Bir PivotTable'daki tüm veri alanlarını temsil eden bir [PivotField](../../com.aspose.cells/pivotfield) nesnesi alır. Salt okunur. Yalnızca Veri bölgesinde iki veya daha fazla veri alanı olduğunda oluşturulur. Varsayılan olarak satır bölgesindedir. Bunu PivotTable.AddFieldToArea() yöntemiyle satır/kolon bölgesine sürükleyebilirsiniz.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine lütfen PivotTable.ValuesField özelliğini kullanın. Bu özellik, Ekim 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### getDataFieldHeaderName() {#getDataFieldHeaderName--}
```
public String getDataFieldHeaderName()
```


PivotTable'daki değer alanı başlığının adını alır.

**Returns:**
java.lang.String
### getDataFields() {#getDataFields--}
```
public PivotFieldCollection getDataFields()
```


PivotTable'daki tüm veri alanlarını temsil eden bir [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) alır.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getDataSource() {#getDataSource--}
```
public String[] getDataSource()
```


PivotTable'ın veri kaynağını alır.

**Returns:**
java.lang.String[]
### getDependentPivotTables() {#getDependentPivotTables--}
```
public PivotTable[] getDependentPivotTables()
```


Bu PivotTable'ı veri kaynağı olarak kullanan tüm [PivotTable](../../com.aspose.cells/pivottable)s alır.

**Remarks**

Pivot tablolar birbirlerinin verilerine bağımlı olabileceği için, veri tutarlılığını sağlamak amacıyla doğru sırayla yenilenmelidir.

**Returns:**
com.aspose.cells.PivotTable[] -
### getDisplayErrorString() {#getDisplayErrorString--}
```
public boolean getDisplayErrorString()
```


PivotTable raporunun hatalı hücrelerde özel bir dize gösterip göstermediğini belirtir.

**Returns:**
boolean
### getDisplayImmediateItems() {#getDisplayImmediateItems--}
```
public boolean getDisplayImmediateItems()
```


PivotTable'ın veri alanı boş olduğunda satır ve sütun alanlarındaki öğelerin görünür olup olmadığını gösterir. Varsayılan değer true'dur.

**Returns:**
boolean
### getDisplayNullString() {#getDisplayNullString--}
```
public boolean getDisplayNullString()
```


PivotTable raporunun değer null olduğunda özel bir dize gösterip göstermediğini belirtir.

**Returns:**
boolean
### getEnableDataValueEditing() {#getEnableDataValueEditing--}
```
public boolean getEnableDataValueEditing()
```


Kullanıcının pivottable'ın veri alanındaki hücreleri düzenlemesine izin verilip verilmediğini gösteren bir Boolean değer belirler. Varsayılan değer false'tur.

**Returns:**
boolean
### getEnableDrilldown() {#getEnableDrilldown--}
```
public boolean getEnableDrilldown()
```


Drilldown'un etkin olup olmadığını belirtir.

**Returns:**
boolean
### getEnableFieldDialog() {#getEnableFieldDialog--}
```
public boolean getEnableFieldDialog()
```


Kullanıcı PivotTable alanına çift tıkladığında PivotTable Alanı iletişim kutusunun mevcut olup olmadığını belirtir.

**Returns:**
boolean
### getEnableFieldList() {#getEnableFieldList--}
```
public boolean getEnableFieldList()
```


Excel görünümünde PivotTable için alan listesinin mevcut olup olmadığını belirtir.

**Returns:**
boolean
### getEnableWizard() {#getEnableWizard--}
```
public boolean getEnableWizard()
```


PivotTable Sihirbazının mevcut olup olmadığını belirtir.

**Returns:**
boolean
### getErrorString() {#getErrorString--}
```
public String getErrorString()
```


DisplayErrorString özelliği true olduğunda hatalı hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir.

**Returns:**
java.lang.String
### getExternalConnectionDataSource() {#getExternalConnectionDataSource--}
```
public ExternalConnection getExternalConnectionDataSource()
```


Harici bağlantı veri kaynağını alır.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotTable.GetSourceDataConnections() metodunu kullanın. Bu metod, Ekim 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getFieldListSortAscending() {#getFieldListSortAscending--}
```
public boolean getFieldListSortAscending()
```


PivotTable'daki alanların alan listesinde varsayılan olmayan bir sırayla sıralanıp sıralanmadığını belirtir.

**Returns:**
boolean
### getFields(int fieldType) {#getFields-int-}
```
public PivotFieldCollection getFields(int fieldType)
```


Bölgeye göre belirli pivot alan listesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). bölge türü. |

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) - the specific pivot field collection
### getFilterArea() {#getFilterArea--}
```
public CellArea getFilterArea()
```


Filtre bölgesi alanını alır.

**Remarks**

Yalnızca filtre pivot alanları mevcutsa geçerlidir. Bu pivot tablo filtre pivot alanları içermiyorsa boş bir alan döndürülür.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getGrandTotalName() {#getGrandTotalName--}
```
public String getGrandTotalName()
```


Toplam satır veya sütun başlığında görüntülenen etiketi döndürür. Varsayılan değer "Grand Total" dizesidir.

**Returns:**
java.lang.String
### getHorizontalBreaks() {#getHorizontalBreaks--}
```
public ArrayList getHorizontalBreaks()
```


pivot table yatay sayfa sonlarının satır indeks listesini alır.

**Remarks**

NOT: Bu metod artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotTable.GetHorizontalPageBreaks() metodunu kullanın. Bu metod, Aralık 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
java.util.ArrayList -
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public int[] getHorizontalPageBreaks()
```


Bu pivot table'ın yatay sayfa sonlarını alır.

**Returns:**
int[] -
### getIndent() {#getIndent--}
```
public int getIndent()
```


Kompakt eksen için girinti artışını belirtir ve Rapor Düzeni'ni Kompakt Formata ayarlamak için kullanılabilir.

**Returns:**
int
### getItemPrintTitles() {#getItemPrintTitles--}
```
public boolean getItemPrintTitles()
```


PivotItem adlarının her basılan sayfanın üst kısmında tekrarlanıp tekrarlanmayacağını belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotTable.RepeatItemsOnEachPrintedPage özelliğini kullanın. Bu özellik, Ekim 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
boolean
### getManualUpdate() {#getManualUpdate--}
```
public boolean getManualUpdate()
```


PivotTable raporunun yalnızca kullanıcının isteği üzerine yeniden hesaplanıp hesaplanmayacağını belirtir.

**Returns:**
boolean
### getMergeLabels() {#getMergeLabels--}
```
public boolean getMergeLabels()
```


Birden fazla hücreyi kapsayan satır/sütun alan etiketlerinin birleştirilip birleştirilmeyeceğini alır.

**Returns:**
boolean
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Bir PivotTable alanının birden çok filtreye sahip olup olamayacağını gösteren bir boolean değer belirler.

Bkz. [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotCache.MissingItemsLimit özelliğini kullanın. Bu özellik, Eylül 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


PivotTable'ın adını alır.

**Returns:**
java.lang.String
### getNamesOfSourceDataConnections() {#getNamesOfSourceDataConnections--}
```
public String[] getNamesOfSourceDataConnections()
```


Harici kaynak veri bağlantılarının adlarını alır.

**Returns:**
java.lang.String[]
### getNullString() {#getNullString--}
```
public String getNullString()
```


DisplayNullString özelliği true olduğunda null değer içeren hücrelerde görüntülenen dizeyi alır. Varsayılan değer boş bir dizedir.

**Returns:**
java.lang.String
### getPageFieldOrder() {#getPageFieldOrder--}
```
public int getPageFieldOrder()
```


Sayfa alanlarının PivotTable raporunun düzenine eklendiği sıralamayı alır.

Bkz. [PrintOrderType](../../com.aspose.cells/printordertype).

**Returns:**
int
### getPageFieldWrapCount() {#getPageFieldWrapCount--}
```
public int getPageFieldWrapCount()
```


PivotTable raporundaki her sütun veya satırdaki sayfa alanı sayısını alır.

**Returns:**
int
### getPageFields() {#getPageFields--}
```
public PivotFieldCollection getPageFields()
```


Şu anda sayfa alanı olarak gösterilen bir [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) döndürür.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getPivotCache() {#getPivotCache--}
```
public PivotCache getPivotCache()
```


Veri kaynağını alır.

**Returns:**
[PivotCache](../../com.aspose.cells/pivotcache)
### getPivotFilters() {#getPivotFilters--}
```
public PivotFilterCollection getPivotFilters()
```


Pivot tabloda bulunan tüm filtreleri döndürür.

**Returns:**
[PivotFilterCollection](../../com.aspose.cells/pivotfiltercollection)
### getPivotFormatConditions() {#getPivotFormatConditions--}
```
public PivotFormatConditionCollection getPivotFormatConditions()
```


Pivot tablonun Biçim Koşullarını alır.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotTable.ConditionalFormats özelliğini kullanın. Bu özellik, Aralık 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
[PivotFormatConditionCollection](../../com.aspose.cells/pivotformatconditioncollection)
### getPivotFormats() {#getPivotFormats--}
```
public PivotTableFormatCollection getPivotFormats()
```


Bu pivot tabloya uygulanan tüm hücre biçimlerini alır.

**Returns:**
[PivotTableFormatCollection](../../com.aspose.cells/pivottableformatcollection)
### getPivotTableStyle() {#getPivotTableStyle--}
```
public TableStyle getPivotTableStyle()
```


Bu pivot tablonun [TableStyle](../../com.aspose.cells/tablestyle) ayarlarını alır.

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle)
### getPivotTableStyleName() {#getPivotTableStyleName--}
```
public String getPivotTableStyleName()
```


Pivot tablonun stil adını alır.

**Returns:**
java.lang.String
### getPivotTableStyleType() {#getPivotTableStyleType--}
```
public int getPivotTableStyleType()
```


Yerleşik pivot tablo stilini alır.

Bkz. [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Returns:**
int
### getPivotTablesWithSamePivotCache() {#getPivotTablesWithSamePivotCache--}
```
public PivotTable[] getPivotTablesWithSamePivotCache()
```


Aynı pivot önbelleğine sahip tüm pivot tabloları alır.

**Returns:**
com.aspose.cells.PivotTable[] -
### getPreserveCellFormattingOnUpdate() {#getPreserveCellFormattingOnUpdate--}
```
public boolean getPreserveCellFormattingOnUpdate()
```


Pivot tablo yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesinin ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) korunup korunmayacağını gösterir.

**Returns:**
boolean
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


PivotTable yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesinin ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) korunup korunmadığını gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotTable.PreserveCellFormattingOnUpdate özelliğini kullanın. Bu özellik, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
boolean
### getPrintDrill() {#getPrintDrill--}
```
public boolean getPrintDrill()
```


Delik göstergelerinin yazdırılıp yazdırılmayacağını gösteren bir Boolean değer belirler. Pivottable'da görüntülendiğinde genişlet/küçült düğmelerini yazdır.

**Returns:**
boolean
### getPrintTitles() {#getPrintTitles--}
```
public boolean getPrintTitles()
```


Çalışma sayfasının yazdırma başlıklarının PivotTable raporuna göre ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getRefreshDataOnOpeningFile() {#getRefreshDataOnOpeningFile--}
```
public boolean getRefreshDataOnOpeningFile()
```


Dosya açılırken Veri Yenileme'nin yapılması gerekip gerekmediğini gösterir.

**Returns:**
boolean
### getRefreshDate() {#getRefreshDate--}
```
public DateTime getRefreshDate()
```


PivotTable'ın en son yenilendiği tarih ve saati alır.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getRefreshedByWho() {#getRefreshedByWho--}
```
public String getRefreshedByWho()
```


Bu PivotTable'ı en son yenileyen kullanıcının adını alır.

**Returns:**
java.lang.String
### getRepeatItemsOnEachPrintedPage() {#getRepeatItemsOnEachPrintedPage--}
```
public boolean getRepeatItemsOnEachPrintedPage()
```


Satır alanındaki pivot öğesi başlıklarının tablo biçimindeki pivot alanları için her yazdırılan sayfada tekrarlanıp tekrarlanmadığını gösterir.

**Returns:**
boolean
### getRowFields() {#getRowFields--}
```
public PivotFieldCollection getRowFields()
```


Şu anda satır alanı olarak gösterilen bir [PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection) döndürür.

**Returns:**
[PivotFieldCollection](../../com.aspose.cells/pivotfieldcollection)
### getRowGrand() {#getRowGrand--}
```
public boolean getRowGrand()
```


Bu pivot tablonun satırları için genel toplamların gösterilip gösterilmeyeceğini belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotTable.ShowRowGrandTotals metodunu kullanın. Bu metod, Aralık 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
boolean
### getRowHeaderCaption() {#getRowHeaderCaption--}
```
public String getRowHeaderCaption()
```


Bu PivotTable'daki Satır Başlığının özel başlığını alır.

**Returns:**
java.lang.String
### getRowRange() {#getRowRange--}
```
public CellArea getRowRange()
```


PivotTable raporundaki satır alanını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSaveData() {#getSaveData--}
```
public boolean getSaveData()
```


PivotTable raporu için verilerin çalışma kitabıyla birlikte kaydedilip kaydedilmediğini gösterir.

**Returns:**
boolean
### getShowColumnGrandTotals() {#getShowColumnGrandTotals--}
```
public boolean getShowColumnGrandTotals()
```


Bu pivot tablonun sütunları için genel toplamların gösterilip gösterilmeyeceğini gösterir.

**Returns:**
boolean
### getShowDataTips() {#getShowDataTips--}
```
public boolean getShowDataTips()
```


PivotTable veri hücreleri için araç ipuçlarının gösterilip gösterilmeyeceğini gösterir.

**Returns:**
boolean
### getShowDrill() {#getShowDrill--}
```
public boolean getShowDrill()
```


Genişletme/küçültme düğmelerinin gösterilip gösterilmediğini alır.

**Returns:**
boolean
### getShowEmptyCol() {#getShowEmptyCol--}
```
public boolean getShowEmptyCol()
```


Tabloda boş sütunların dahil edilip edilmeyeceğini gösterir.

**Returns:**
boolean
### getShowEmptyRow() {#getShowEmptyRow--}
```
public boolean getShowEmptyRow()
```


Tabloda boş satırların dahil edililip edilmeyeceğini gösterir.

**Returns:**
boolean
### getShowHeaders() {#getShowHeaders--}
```
public boolean getShowHeaders()
```


Satır ekseninde ve sütun ekseninde PivotTable görünümünde veri alanı başlıklarını ve pivot alanı başlıklarını gösterip göstermeyeceği.

**Returns:**
boolean
### getShowMemberPropertyTips() {#getShowMemberPropertyTips--}
```
public boolean getShowMemberPropertyTips()
```


Üye özelliği bilgilerinin PivotTable araç ipuçlarından çıkarılıp çıkarılmayacağını gösteren bir boolean değer belirtir.

**Returns:**
boolean
### getShowPivotStyleColumnHeader() {#getShowPivotStyleColumnHeader--}
```
public boolean getShowPivotStyleColumnHeader()
```


Pivot tabloda sütun başlığının stile uygulanıp uygulanmayacağını gösterir.

**Returns:**
boolean
### getShowPivotStyleColumnStripes() {#getShowPivotStyleColumnStripes--}
```
public boolean getShowPivotStyleColumnStripes()
```


Sütun için çizgili biçimlendirmesinin uygulanıp uygulanmadığını gösterir.

**Returns:**
boolean
### getShowPivotStyleLastColumn() {#getShowPivotStyleLastColumn--}
```
public boolean getShowPivotStyleLastColumn()
```


Sütun biçimlendirmesinin uygulanıp uygulanmadığını gösterir.

**Returns:**
boolean
### getShowPivotStyleRowHeader() {#getShowPivotStyleRowHeader--}
```
public boolean getShowPivotStyleRowHeader()
```


Pivot tabloda satır başlığının stile uygulanıp uygulanmayacağını gösterir.

**Returns:**
boolean
### getShowPivotStyleRowStripes() {#getShowPivotStyleRowStripes--}
```
public boolean getShowPivotStyleRowStripes()
```


Satır çizgili biçimlendirmesinin uygulanıp uygulanmadığını gösterir.

**Returns:**
boolean
### getShowRowGrandTotals() {#getShowRowGrandTotals--}
```
public boolean getShowRowGrandTotals()
```


Pivot tablonun satırları için genel toplamların gösterilip gösterilmeyeceğini gösterir.

**Remarks**

**Returns:**
boolean
### getShowRowHeaderCaption() {#getShowRowHeaderCaption--}
```
public boolean getShowRowHeaderCaption()
```


PivotTable raporunda satır başlığı açıklamasının gösterilip gösterilmediğini ve alan başlıklarının ve filtre açılır menülerinin görüntülenip görüntülenmediğini gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotTable.ShowHeaders özelliğini kullanın. Bu özellik, Nisan 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
boolean
### getShowValuesRow() {#getShowValuesRow--}
```
public boolean getShowValuesRow()
```


Değer satırının gösterilip gösterilmediğini gösterir.

**Returns:**
boolean
### getSource() {#getSource--}
```
public String[] getSource()
```


Bu pivot tablonun veri kaynağını alır.

**Returns:**
java.lang.String[]
### getSource(boolean isOriginal) {#getSource-boolean-}
```
public String[] getSource(boolean isOriginal)
```


Bu pivot tablonun veri kaynağını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isOriginal | boolean | Orijinal mi yoksa görüntüleme veri kaynağını mı döndüreceğini gösterir. |

**Returns:**
java.lang.String[] -
### getSourceDataConnections() {#getSourceDataConnections--}
```
public ExternalConnection[] getSourceDataConnections()
```


Harici bağlantı veri kaynaklarını alır.

**Returns:**
com.aspose.cells.ExternalConnection[]
### getSourceType() {#getSourceType--}
```
public byte getSourceType()
```


Pivot tablonun veri kaynağı türünü alır.

[PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype) öğesine bakın.

**Returns:**
byte
### getSubtotalHiddenPageItems() {#getSubtotalHiddenPageItems--}
```
public boolean getSubtotalHiddenPageItems()
```


PivotTable raporundaki gizli sayfa alanı öğelerinin satır ve sütun alt toplamlarına, blok toplamlarına ve genel toplamlarına dahil edilip edilmediğini gösterir. Varsayılan değer False'tur.

**Returns:**
boolean
### getTableRange1() {#getTableRange1--}
```
public CellArea getTableRange1()
```


Tüm PivotTable raporunu içeren aralığı temsil eden bir CellArea nesnesi döndürür, ancak sayfa alanlarını içermez. Salt okunur.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTableRange2() {#getTableRange2--}
```
public CellArea getTableRange2()
```


Tüm PivotTable raporunu içeren aralığı temsil eden bir CellArea nesnesi döndürür, sayfa alanlarını içerir. Salt okunur.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getTag() {#getTag--}
```
public String getTag()
```


Bu PivotTable görünümüyle ilişkili kullanıcı tanımlı bir dizeyi alır.

**Returns:**
java.lang.String
### getTopRightArea() {#getTopRightArea--}
```
public CellArea getTopRightArea()
```


PivotTable'ın sağ üst köşesindeki (RTL sayfalar için sol üst) boş alanı temsil eder.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getValuesField() {#getValuesField--}
```
public PivotField getValuesField()
```


Bir PivotTable'daki tüm veri alanlarını temsil eden bir [PivotField](../../com.aspose.cells/pivotfield) nesnesi alır. Salt okunur. Yalnızca Veri bölgesinde iki veya daha fazla veri alanı olduğunda oluşturulur. Varsayılan olarak satır bölgesindedir. Bunu PivotTable.AddFieldToArea() yöntemiyle satır/kolon bölgesine sürükleyebilirsiniz.

**Returns:**
[PivotField](../../com.aspose.cells/pivotfield)
### hasBlankRows() {#hasBlankRows--}
```
public boolean hasBlankRows()
```


Boş satır eklenip eklenmeyeceğini gösterir. Bu özellik yalnızca boş satır eklenmesi gereken PivotTable otomatik biçim türleri için geçerlidir.

**Remarks**

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen PivotField.InsertBlankRow özelliğini kullanın. Bu yöntem, Nisan 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoFormat() {#isAutoFormat--}
```
public boolean isAutoFormat()
```


Excel 2003 için pivottable seçeneğinde bulunan "autoformat table" onay kutusu.

**Returns:**
boolean
### isExcel2003Compatible() {#isExcel2003Compatible--}
```
public boolean isExcel2003Compatible()
```


PivotTable yenilenirken PivotTable'ın Excel2003 ile uyumlu olup olmadığını belirtir; doğru ise bir dize 255 karakterden az veya eşit olmalıdır, dolayısıyla 255 karakterden uzun bir dize kırpılacaktır. Yanlış ise dize bu sınırlamaya tabi olmayacaktır. Varsayılan değer doğrudur.

**Returns:**
boolean
### isGridDropZones() {#isGridDropZones--}
```
public boolean isGridDropZones()
```


PivotTable raporunun klasik pivottable düzenini gösterip göstermediğini belirtir. (ızgarada alanları sürüklemeyi etkinleştirir)

**Returns:**
boolean
### isMultipleFieldFilters() {#isMultipleFieldFilters--}
```
public boolean isMultipleFieldFilters()
```


Bir PivotTable alanının birden çok filtreye sahip olup olamayacağını gösteren bir boolean değer belirler.

**Remarks**

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen PivotTable.AllowMultipleFiltersPerField özelliğini kullanın. Bu yöntem, Aralık 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Bu PivotTable'ın seçili olup olmadığını gösterir.

**Returns:**
boolean
### move(int row, int column) {#move-int-int-}
```
public void move(int row, int column)
```


PivotTable'ı çalışma sayfasında farklı bir konuma taşır.

**Remarks**

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen PivotTable.MoveTo() metodunu kullanın. Bu yöntem, Aralık 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | satır indeksi. |
| sütun | int | sütun indeksi. |

### move(String destCellName) {#move-java.lang.String-}
```
public void move(String destCellName)
```


PivotTable'ı çalışma sayfasında farklı bir konuma taşır.

**Remarks**

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen PivotTable.MoveTo() metodunu kullanın. Bu yöntem, Aralık 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destCellName | java.lang.String | hedef hücre adı. |

### moveItem(int region, String[] nodes, boolean absolute, int offset) {#moveItem-int-java.lang.String---boolean-int-}
```
public void moveItem(int region, String[] nodes, boolean absolute, int offset)
```


Bir öğeyi yukarı veya aşağı hareket ettir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| region | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Bölge. Yalnızca satır veya sütun için. |
| düğümler | java.lang.String[] | Öğe. |
| mutlak | boolean | Ofsetin mutlak konum olup olmadığını gösterir. |
| ofset | int | Mutlak doğru ise: 0 başlangıca, -1 sona hareket eder, diğerleri mutlak konumu ifade eder; aksi takdirde ofset göreli bir konumdur. |

### moveTo(int row, int column) {#moveTo-int-int-}
```
public void moveTo(int row, int column)
```


PivotTable'ı çalışma sayfasında farklı bir konuma taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | satır indeksi. |
| sütun | int | sütun indeksi. |

### moveTo(int sheetIndex, int row, int column) {#moveTo-int-int-int-}
```
public void moveTo(int sheetIndex, int row, int column)
```


PivotTable'ı çalışma sayfasında farklı bir konuma taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | int | hedef çalışma sayfasının indeksi |
| satır | int | satır indeksi. |
| sütun | int | sütun indeksi. |

### moveTo(String destCellName) {#moveTo-java.lang.String-}
```
public void moveTo(String destCellName)
```


PivotTable'ı çalışma sayfasında farklı bir konuma taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destCellName | java.lang.String | hedef hücre adı. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int refresh()
```


Veri kaynağından [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) yenileyin ve pivot görünümü için veri ve stili hesaplayın.

**Remarks**

Aynı PivotCache'e bağımlı tüm pivot tablolar yeniden hesaplanacaktır.

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Veri kaynağından [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) yenileyin ve pivot görünümü için veri ve stili hesaplayın.

**Remarks**

Aynı PivotCache'e bağımlı tüm pivot tablolar yeniden hesaplanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

**Returns:**
int - [PivotRefreshState](../../com.aspose.cells/pivotrefreshstate).
### refreshData() {#refreshData--}
```
public int refreshData()
```


Veriyi veri kaynağından pivot önbelleğine yeniler.

**Remarks**

Veri kaynağından bir pivot önbelleğe veri toplayacağız, ardından önbellekteki verileri hücrelere hesaplayacağız. Ve dosyadaki tüm pivot tabloları tek tek yenilemek yerine, [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) metodunu basitçe çağırmanız daha iyidir. NOT: Bu yöntem artık kullanılmamaktadır. Bunun yerine lütfen [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) metodunu kullanın ve ardından [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) metodunu kaldırın, çünkü bu pivot tablo [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) yenilenirken hesaplanacaktır. Bu yöntem, Haziran 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### refreshData(PivotTableRefreshOption option) {#refreshData-com.aspose.cells.PivotTableRefreshOption-}
```
public int refreshData(PivotTableRefreshOption option)
```


Seçeneklerle pivottable'ın verisini ve ayarlarını veri kaynağından yeniler.

**Remarks**

Veri kaynağından bir pivot önbelleğe veri toplayacağız, ardından önbellekteki verileri hücrelere hesaplayacağız. Ve dosyadaki tüm pivot tabloları tek tek yenilemek yerine, [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) metodunu basitçe çağırmanız daha iyidir. NOT: Bu yöntem artık kullanılmamaktadır. Bunun yerine lütfen [PivotCache.refresh()](../../com.aspose.cells/pivotcache\#refresh--) metodunu kullanın ve ardından [calculateData()](../../com.aspose.cells/pivottable\#calculateData--) metodunu kaldırın, çünkü bu pivot tablo [getPivotCache()](../../com.aspose.cells/pivottable\#getPivotCache--) yenilenirken hesaplanacaktır. Bu yöntem, Haziran 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Pivot tablonun veri kaynağını yenileme seçenekleri. |

**Returns:**
int
### removeField(int fieldType, PivotField pivotField) {#removeField-int-com.aspose.cells.PivotField-}
```
public void removeField(int fieldType, PivotField pivotField)
```


Belirli alan bölgesinden alanı kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). alanların bölge türü. |
| pivotField | [PivotField](../../com.aspose.cells/pivotfield) | temel alanlardaki alan. |

### removeField(int fieldType, int baseFieldIndex) {#removeField-int-int-}
```
public void removeField(int fieldType, int baseFieldIndex)
```


Belirli pivot bölgesinden bir alanı kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Alanların bölge türü. |
| baseFieldIndex | int | Temel alanlardaki alan dizini. |

### removeField(int fieldType, String fieldName) {#removeField-int-java.lang.String-}
```
public void removeField(int fieldType, String fieldName)
```


Belirli alan bölgesinden bir alanı kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Alanların bölge türü. |
| fieldName | java.lang.String | Temel alanlardaki ad. |

### selectArea(CellArea ca) {#selectArea-com.aspose.cells.CellArea-}
```
public PivotAreaCollection selectArea(CellArea ca)
```


Pivot tablo görünümünün bir alanını seç.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Hücre alanı. |

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection) - 
### setAllowMultipleFiltersPerField(boolean value) {#setAllowMultipleFiltersPerField-boolean-}
```
public void setAllowMultipleFiltersPerField(boolean value)
```


Bir PivotTable alanının birden çok filtreye sahip olup olamayacağını gösteren bir boolean değer belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAltTextDescription(String value) {#setAltTextDescription-java.lang.String-}
```
public void setAltTextDescription(String value)
```


Alt metnin açıklamasını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setAltTextTitle(String value) {#setAltTextTitle-java.lang.String-}
```
public void setAltTextTitle(String value)
```


Alternatif metnin başlığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setAutoFormat(boolean value) {#setAutoFormat-boolean-}
```
public void setAutoFormat(boolean value)
```


Excel 2003 için pivottable seçeneğinde bulunan "autoformat table" onay kutusu.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoFormatType(int value) {#setAutoFormatType-int-}
```
public void setAutoFormatType(int value)
```


PivotTable'ın otomatik biçim türünü ayarlar.

Bakınız [PivotTableAutoFormatType](../../com.aspose.cells/pivottableautoformattype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setAutofitColumnWidthOnUpdate(boolean value) {#setAutofitColumnWidthOnUpdate-boolean-}
```
public void setAutofitColumnWidthOnUpdate(boolean value)
```


Güncelleme sırasında sütun genişliğinin otomatik ayarlanıp ayarlanmayacağını gösterir

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setColumnGrand(boolean value) {#setColumnGrand-boolean-}
```
public void setColumnGrand(boolean value)
```


PivotTable raporunun sütunlar için genel toplamları gösterip göstermediğini belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine lütfen PivotTable.ShowColumnGrandTotals yöntemini kullanın. Bu yöntem, Aralık 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setColumnHeaderCaption(String value) {#setColumnHeaderCaption-java.lang.String-}
```
public void setColumnHeaderCaption(String value)
```


PivotTable'ın Sütun Başlığının özel başlığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCustomListSort(boolean value) {#setCustomListSort-boolean-}
```
public void setCustomListSort(boolean value)
```


Veri sıralanırken yerleşik özel listenin dikkate alınıp alınmayacağını gösterir

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDataFieldHeaderName(String value) {#setDataFieldHeaderName-java.lang.String-}
```
public void setDataFieldHeaderName(String value)
```


PivotTable'taki değer alanı alan başlığının adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDataSource(String[] value) {#setDataSource-java.lang.String---}
```
public void setDataSource(String[] value)
```


Pivot tablonun veri kaynağını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String[] |  |

### setDisplayErrorString(boolean value) {#setDisplayErrorString-boolean-}
```
public void setDisplayErrorString(boolean value)
```


PivotTable raporunun hatalı hücrelerde özel bir dize gösterip göstermediğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDisplayImmediateItems(boolean value) {#setDisplayImmediateItems-boolean-}
```
public void setDisplayImmediateItems(boolean value)
```


PivotTable'ın veri alanı boş olduğunda satır ve sütun alanlarındaki öğelerin görünür olup olmadığını gösterir. Varsayılan değer true'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDisplayNullString(boolean value) {#setDisplayNullString-boolean-}
```
public void setDisplayNullString(boolean value)
```


PivotTable raporunun değer null olduğunda özel bir dize gösterip göstermediğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableDataValueEditing(boolean value) {#setEnableDataValueEditing-boolean-}
```
public void setEnableDataValueEditing(boolean value)
```


Kullanıcının pivottable'ın veri alanındaki hücreleri düzenlemesine izin verilip verilmediğini gösteren bir Boolean değer belirler. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableDrilldown(boolean value) {#setEnableDrilldown-boolean-}
```
public void setEnableDrilldown(boolean value)
```


Drilldown'un etkin olup olmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableFieldDialog(boolean value) {#setEnableFieldDialog-boolean-}
```
public void setEnableFieldDialog(boolean value)
```


Kullanıcı PivotTable alanına çift tıkladığında PivotTable Alanı iletişim kutusunun mevcut olup olmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableFieldList(boolean value) {#setEnableFieldList-boolean-}
```
public void setEnableFieldList(boolean value)
```


Excel görünümünde PivotTable için alan listesinin mevcut olup olmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEnableWizard(boolean value) {#setEnableWizard-boolean-}
```
public void setEnableWizard(boolean value)
```


PivotTable Sihirbazının mevcut olup olmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setErrorString(String value) {#setErrorString-java.lang.String-}
```
public void setErrorString(String value)
```


DisplayErrorString özelliği true olduğunda hatalı hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setExcel2003Compatible(boolean value) {#setExcel2003Compatible-boolean-}
```
public void setExcel2003Compatible(boolean value)
```


PivotTable yenilenirken PivotTable'ın Excel2003 ile uyumlu olup olmadığını belirtir; doğru ise bir dize 255 karakterden az veya eşit olmalıdır, dolayısıyla 255 karakterden uzun bir dize kırpılacaktır. Yanlış ise dize bu sınırlamaya tabi olmayacaktır. Varsayılan değer doğrudur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFieldListSortAscending(boolean value) {#setFieldListSortAscending-boolean-}
```
public void setFieldListSortAscending(boolean value)
```


PivotTable'daki alanların alan listesinde varsayılan olmayan bir sırayla sıralanıp sıralanmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setGrandTotalName(String value) {#setGrandTotalName-java.lang.String-}
```
public void setGrandTotalName(String value)
```


Toplam satır veya sütun başlığında görüntülenen etiketi döndürür. Varsayılan değer "Grand Total" dizesidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setGridDropZones(boolean value) {#setGridDropZones-boolean-}
```
public void setGridDropZones(boolean value)
```


PivotTable raporunun klasik pivottable düzenini gösterip göstermediğini belirtir. (ızgarada alanları sürüklemeyi etkinleştirir)

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasBlankRows(boolean value) {#setHasBlankRows-boolean-}
```
public void setHasBlankRows(boolean value)
```


Boş satır eklenip eklenmeyeceğini gösterir. Bu özellik yalnızca boş satır eklenmesi gereken PivotTable otomatik biçim türleri için geçerlidir.

**Remarks**

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen PivotField.InsertBlankRow özelliğini kullanın. Bu yöntem, Nisan 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setIndent(int value) {#setIndent-int-}
```
public void setIndent(int value)
```


Kompakt eksen için girinti artışını belirtir ve Rapor Düzeni'ni Kompakt Formata ayarlamak için kullanılabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setItemPrintTitles(boolean value) {#setItemPrintTitles-boolean-}
```
public void setItemPrintTitles(boolean value)
```


PivotItem adlarının her basılan sayfanın üst kısmında tekrarlanıp tekrarlanmayacağını belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotTable.RepeatItemsOnEachPrintedPage özelliğini kullanın. Bu özellik, Ekim 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setManualUpdate(boolean value) {#setManualUpdate-boolean-}
```
public void setManualUpdate(boolean value)
```


PivotTable raporunun yalnızca kullanıcının isteği üzerine yeniden hesaplanıp hesaplanmayacağını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMergeLabels(boolean value) {#setMergeLabels-boolean-}
```
public void setMergeLabels(boolean value)
```


Birden fazla hücreye yayılan satır/sütun alan etiketlerini birleştirip birleştirilmeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Bir PivotTable alanının birden çok filtreye sahip olup olamayacağını gösteren bir boolean değer belirler.

Bkz. [PivotMissingItemLimitType](../../com.aspose.cells/pivotmissingitemlimittype).

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotCache.MissingItemsLimit özelliğini kullanın. Bu özellik, Eylül 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMultipleFieldFilters(boolean value) {#setMultipleFieldFilters-boolean-}
```
public void setMultipleFieldFilters(boolean value)
```


Bir PivotTable alanının birden çok filtreye sahip olup olamayacağını gösteren bir boolean değer belirler.

**Remarks**

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen PivotTable.AllowMultipleFiltersPerField özelliğini kullanın. Bu yöntem, Aralık 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


PivotTable'ın adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setNullString(String value) {#setNullString-java.lang.String-}
```
public void setNullString(String value)
```


DisplayNullString özelliği true olduğunda null değer içeren hücrelerde görüntülenen dizeyi alır. Varsayılan değer boş bir dizedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPageFieldOrder(int value) {#setPageFieldOrder-int-}
```
public void setPageFieldOrder(int value)
```


Sayfa alanlarının PivotTable raporunun düzenine eklendiği sıralamayı ayarlar.

Bkz. [PrintOrderType](../../com.aspose.cells/printordertype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPageFieldWrapCount(int value) {#setPageFieldWrapCount-int-}
```
public void setPageFieldWrapCount(int value)
```


PivotTable raporundaki her sütun veya satırdaki sayfa alanı sayısını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPivotTableStyle(TableStyle value) {#setPivotTableStyle-com.aspose.cells.TableStyle-}
```
public void setPivotTableStyle(TableStyle value)
```


Bu pivot tablonun [TableStyle](../../com.aspose.cells/tablestyle) ayarlarını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TableStyle](../../com.aspose.cells/tablestyle) |  |

### setPivotTableStyleName(String value) {#setPivotTableStyleName-java.lang.String-}
```
public void setPivotTableStyleName(String value)
```


Pivot tablonun stil adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPivotTableStyleType(int value) {#setPivotTableStyleType-int-}
```
public void setPivotTableStyleType(int value)
```


Yerleşik pivot tablo stilini ayarlar.

Bkz. [PivotTableStyleType](../../com.aspose.cells/pivottablestyletype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPreserveCellFormattingOnUpdate(boolean value) {#setPreserveCellFormattingOnUpdate-boolean-}
```
public void setPreserveCellFormattingOnUpdate(boolean value)
```


Pivot tablo yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesinin ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) korunup korunmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


PivotTable yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesinin ([PivotTableFormat](../../com.aspose.cells/pivottableformat)) korunup korunmadığını gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotTable.PreserveCellFormattingOnUpdate özelliğini kullanın. Bu özellik, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPrintDrill(boolean value) {#setPrintDrill-boolean-}
```
public void setPrintDrill(boolean value)
```


Delik göstergelerinin yazdırılıp yazdırılmayacağını gösteren bir Boolean değer belirler. Pivottable'da görüntülendiğinde genişlet/küçült düğmelerini yazdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPrintTitles(boolean value) {#setPrintTitles-boolean-}
```
public void setPrintTitles(boolean value)
```


Çalışma sayfasının yazdırma başlıklarının PivotTable raporuna göre ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRefreshDataOnOpeningFile(boolean value) {#setRefreshDataOnOpeningFile-boolean-}
```
public void setRefreshDataOnOpeningFile(boolean value)
```


Dosya açılırken Veri Yenileme'nin yapılması gerekip gerekmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRepeatItemsOnEachPrintedPage(boolean value) {#setRepeatItemsOnEachPrintedPage-boolean-}
```
public void setRepeatItemsOnEachPrintedPage(boolean value)
```


Satır alanındaki pivot öğesi başlıklarının tablo biçimindeki pivot alanları için her yazdırılan sayfada tekrarlanıp tekrarlanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRowGrand(boolean value) {#setRowGrand-boolean-}
```
public void setRowGrand(boolean value)
```


Bu pivot tablonun satırları için genel toplamların gösterilip gösterilmeyeceğini belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotTable.ShowRowGrandTotals metodunu kullanın. Bu metod, Aralık 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRowHeaderCaption(String value) {#setRowHeaderCaption-java.lang.String-}
```
public void setRowHeaderCaption(String value)
```


Bu PivotTable'daki Satır Başlığının özel başlığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSaveData(boolean value) {#setSaveData-boolean-}
```
public void setSaveData(boolean value)
```


PivotTable raporu için verilerin çalışma kitabıyla birlikte kaydedilip kaydedilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Bu PivotTable'ın seçili olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowColumnGrandTotals(boolean value) {#setShowColumnGrandTotals-boolean-}
```
public void setShowColumnGrandTotals(boolean value)
```


Bu pivot tablonun sütunları için genel toplamların gösterilip gösterilmeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowDataTips(boolean value) {#setShowDataTips-boolean-}
```
public void setShowDataTips(boolean value)
```


PivotTable veri hücreleri için araç ipuçlarının gösterilip gösterilmeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowDrill(boolean value) {#setShowDrill-boolean-}
```
public void setShowDrill(boolean value)
```


Genişlet/daralt düğmelerinin gösterilip gösterilmeyeceğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowEmptyCol(boolean value) {#setShowEmptyCol-boolean-}
```
public void setShowEmptyCol(boolean value)
```


Tabloda boş sütunların dahil edilip edilmeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowEmptyRow(boolean value) {#setShowEmptyRow-boolean-}
```
public void setShowEmptyRow(boolean value)
```


Tabloda boş satırların dahil edililip edilmeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowHeaders(boolean value) {#setShowHeaders-boolean-}
```
public void setShowHeaders(boolean value)
```


Satır ekseninde ve sütun ekseninde PivotTable görünümünde veri alanı başlıklarını ve pivot alanı başlıklarını gösterip göstermeyeceği.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowMemberPropertyTips(boolean value) {#setShowMemberPropertyTips-boolean-}
```
public void setShowMemberPropertyTips(boolean value)
```


Üye özelliği bilgilerinin PivotTable araç ipuçlarından çıkarılıp çıkarılmayacağını gösteren bir boolean değer belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowPivotStyleColumnHeader(boolean value) {#setShowPivotStyleColumnHeader-boolean-}
```
public void setShowPivotStyleColumnHeader(boolean value)
```


Pivot tabloda sütun başlığının stile uygulanıp uygulanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowPivotStyleColumnStripes(boolean value) {#setShowPivotStyleColumnStripes-boolean-}
```
public void setShowPivotStyleColumnStripes(boolean value)
```


Sütun için çizgili biçimlendirmesinin uygulanıp uygulanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowPivotStyleLastColumn(boolean value) {#setShowPivotStyleLastColumn-boolean-}
```
public void setShowPivotStyleLastColumn(boolean value)
```


Sütun biçimlendirmesinin uygulanıp uygulanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowPivotStyleRowHeader(boolean value) {#setShowPivotStyleRowHeader-boolean-}
```
public void setShowPivotStyleRowHeader(boolean value)
```


Pivot tabloda satır başlığının stile uygulanıp uygulanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowPivotStyleRowStripes(boolean value) {#setShowPivotStyleRowStripes-boolean-}
```
public void setShowPivotStyleRowStripes(boolean value)
```


Satır çizgili biçimlendirmesinin uygulanıp uygulanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowRowGrandTotals(boolean value) {#setShowRowGrandTotals-boolean-}
```
public void setShowRowGrandTotals(boolean value)
```


Pivot tablonun satırları için genel toplamların gösterilip gösterilmeyeceğini gösterir.

**Remarks**

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowRowHeaderCaption(boolean value) {#setShowRowHeaderCaption-boolean-}
```
public void setShowRowHeaderCaption(boolean value)
```


PivotTable raporunda satır başlığı açıklamasının gösterilip gösterilmediğini ve alan başlıklarının ve filtre açılır menülerinin görüntülenip görüntülenmediğini gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotTable.ShowHeaders özelliğini kullanın. Bu özellik, Nisan 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowValuesRow(boolean value) {#setShowValuesRow-boolean-}
```
public void setShowValuesRow(boolean value)
```


Değer satırının gösterilip gösterilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSubtotalHiddenPageItems(boolean value) {#setSubtotalHiddenPageItems-boolean-}
```
public void setSubtotalHiddenPageItems(boolean value)
```


PivotTable raporundaki gizli sayfa alanı öğelerinin satır ve sütun alt toplamlarına, blok toplamlarına ve genel toplamlarına dahil edilip edilmediğini gösterir. Varsayılan değer False'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTag(String value) {#setTag-java.lang.String-}
```
public void setTag(String value)
```


Bu PivotTable görünümüyle ilişkili kullanıcı tanımlı bir dize ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn) {#showDetail-int-int-boolean-int-int-}
```
public void showDetail(int rowOffset, int columnOffset, boolean newSheet, int destRow, int destColumn)
```


Veri bölgesindeki bir öğenin ayrıntısını yeni bir Tablo'ya göster.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | int | Veri bölgesindeki ilk veri satırına ofset. |
| columnOffset | int | Veri bölgesindeki ilk veri sütununa ofset. |
| newSheet | boolean | Detayı yeni bir çalışma sayfasına göster. |
| destRow | int | Hedef satır. |
| destColumn | int | Hedef sütun. |

### showInCompactForm() {#showInCompactForm--}
```
public void showInCompactForm()
```


PivotTable görünümünü kompakt biçimde düzenler.

### showInOutlineForm() {#showInOutlineForm--}
```
public void showInOutlineForm()
```


PivotTable'ı taslak biçimde düzenler.

### showInTabularForm() {#showInTabularForm--}
```
public void showInTabularForm()
```


PivotTable'ı tablo biçiminde düzenler.

### showReportFilterPage(PivotField pageField) {#showReportFilterPage-com.aspose.cells.PivotField-}
```
public void showReportFilterPage(PivotField pageField)
```


PivotField'e göre tüm rapor filtre sayfalarını göster, PivotField PageFields içinde bulunmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageField | [PivotField](../../com.aspose.cells/pivotfield) | PivotField nesnesi. |

### showReportFilterPageByIndex(int posIndex) {#showReportFilterPageByIndex-int-}
```
public void showReportFilterPageByIndex(int posIndex)
```


PageFields içindeki konum indeksine göre tüm rapor filtre sayfalarını göster.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| posIndex | int | PageFields içindeki konum dizini. |

### showReportFilterPageByName(String fieldName) {#showReportFilterPageByName-java.lang.String-}
```
public void showReportFilterPageByName(String fieldName)
```


PivotField'in adına göre tüm rapor filtre sayfalarını göster, PivotField PageFields içinde bulunmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldName | java.lang.String | PivotField adı. |

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

