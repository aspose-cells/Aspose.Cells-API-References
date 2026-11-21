---
title: "Worksheet"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tek bir çalışma sayfasını temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/worksheet/
---

**Inheritance:**
java.lang.Object
```
public class Worksheet
```

Tek bir çalışma sayfasını temsil eden nesneyi kapsüller.

**Example**

Aşağıdaki örnek, .Net veya VB ile çalışma sayfasında bölmeleri dondurmayı ve bir bağlantı eklemeyi gösterir.

```
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Freeze panes at "AS40" with 10 rows and 10 columns
         sheet.freezePanes("AS40", 10, 10);
 
         //Add a hyperlink in Cell A1
         sheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addPageBreaks(String cellName)](#addPageBreaks-java.lang.String-) | Sayfa sonu ekler. |
| [advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)](#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-) | Verileri karmaşık ölçütlerle filtreler. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Sütun genişliğini otomatik olarak ayarlar. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Sütun genişliğini otomatik olarak ayarlar. |
| [autoFitColumns()](#autoFitColumns--) | Bu çalışma sayfasındaki tüm sütunları otomatik olarak ayarlar. |
| [autoFitColumns(AutoFitterOptions options)](#autoFitColumns-com.aspose.cells.AutoFitterOptions-) | Bu çalışma sayfasındaki tüm sütunları otomatik olarak ayarlar. |
| [autoFitColumns(int firstColumn, int lastColumn)](#autoFitColumns-int-int-) | Sütunların genişliğini otomatik olarak ayarlar. |
| [autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-) | Sütunların genişliğini otomatik olarak ayarlar. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)](#autoFitColumns-int-int-int-int-) | Sütunların genişliğini otomatik olarak ayarlar. |
| [autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)](#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-) | Sütunların genişliğini otomatik olarak ayarlar. |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Satır yüksekliğini otomatik olarak ayarlar. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Satır yüksekliğini otomatik olarak ayarlar. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)](#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-) | Satır yüksekliğini otomatik olarak ayarlar. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Dikdörtgen bir aralıktaki satır yüksekliğini otomatik olarak ayarlar. |
| [autoFitRows()](#autoFitRows--) | Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar. |
| [autoFitRows(AutoFitterOptions options)](#autoFitRows-com.aspose.cells.AutoFitterOptions-) | Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Bir aralıktaki satır yüksekliğini otomatik olarak ayarlar. |
| [autoFitRows(int startRow, int endRow, AutoFitterOptions options)](#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-) | Bir aralıktaki satır yüksekliğini otomatik olarak ayarlar. |
| [calculateArrayFormula(String formula, CalculationOptions opts)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Bir formülü dizi formülü olarak hesaplar. |
| [calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)](#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-) | Bir formülü dizi formülü olarak hesaplar. |
| [calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)](#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-) | Bir formülü dizi formülü olarak hesaplar. |
| [calculateFormula(CalculationOptions options, boolean recursive)](#calculateFormula-com.aspose.cells.CalculationOptions-boolean-) | Bu çalışma sayfasındaki tüm formülleri hesaplar. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Bir formülü hesaplar. |
| [calculateFormula(String formula, CalculationOptions opts)](#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-) | Bir formül ifadesini doğrudan hesaplar. |
| [calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)](#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-) | Bir formül ifadesini doğrudan hesaplar. |
| [clearComments()](#clearComments--) | Tasarımcı elektronik tablosundaki tüm yorumları temizler. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Bu çalışma sayfasındaki verilere erişmek için önbellek kullanan oturumu kapatır. |
| [convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)](#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-) | Formül referans stilini dönüştürür. |
| [copy(Worksheet sourceSheet)](#copy-com.aspose.cells.Worksheet-) | Başka bir çalışma sayfasından içerikleri ve biçimleri kopyalar. |
| [copy(Worksheet sourceSheet, CopyOptions copyOptions)](#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-) | Başka bir çalışma sayfasından içerikleri ve biçimleri kopyalar. |
| [dispose()](#dispose--) | Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(CellArea ca)](#filter-com.aspose.cells.CellArea-) | Aralığı filtreler. |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur. |
| [getActiveCell()](#getActiveCell--) | Çalışma sayfasındaki etkin hücreyi alır. |
| [getAdvancedFilter()](#getAdvancedFilter--) | Gelişmiş filtrenin ayarlarını alır. |
| [getAllPictures()](#getAllPictures--) | Hücreye gömülü ve hücrelerin üzerindeki tüm resimleri alır. |
| [getAllowEditRanges()](#getAllowEditRanges--) | Çalışma sayfasındaki düzenleme izinli aralık koleksiyonunu alır. |
| [getAreasOfXmlMapQuery(String path, XmlMap xmlMap)](#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | XML haritasının belirli yoluna eşlenen/bağlanan hücre alanlarını sorgular. |
| [getAutoFilter()](#getAutoFilter--) | Belirtilen çalışma sayfası için otomatik filtreyi temsil eder. |
| [getBackgroundImage()](#getBackgroundImage--) | Çalışma sayfasının arka plan resmini alır. |
| [getCellWatches()](#getCellWatches--) | Bu çalışma sayfasında 'watch window' içinde izlenen hücrelerin koleksiyonunu alır. |
| [getCells()](#getCells--) | [Cells](../../com.aspose.cells/cells) koleksiyonunu alır. |
| [getCharts()](#getCharts--) | [Chart](../../com.aspose.cells/chart) koleksiyonunu alır |
| [getCheckBoxes()](#getCheckBoxes--) | [CheckBox](../../com.aspose.cells/checkbox) koleksiyonunu alır. |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Çalışma sayfasının kod adını alır. |
| [getComments()](#getComments--) | [Comment](../../com.aspose.cells/comment) koleksiyonunu alır. |
| [getConditionalFormattings()](#getConditionalFormattings--) | Çalışma sayfasındaki ConditionalFormattings öğelerini alır. |
| [getCustomProperties()](#getCustomProperties--) | Bir çalışma sayfasıyla ilişkili tanımlayıcı bilgilerini temsil eden nesneyi alır. |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Belirtilen çalışma sayfasının soldan sağa yerine sağdan sola görüntülenip görüntülenmediğini gösterir. |
| [getDisplayZeros()](#getDisplayZeros--) | Sıfır değerler gösteriliyorsa doğru. |
| [getErrorCheckOptions()](#getErrorCheckOptions--) | Belirli aralıklara uygulanan hata kontrol ayarını alır. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | İlk görünen sütun indeksini temsil eder. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | İlk görünen satır indeksini temsil eder. |
| [getFreezedPanes()](#getFreezedPanes--) | Dondurulmuş bölmeleri alır. |
| [getGridlineColor()](#getGridlineColor--) | Izgara çizgisi rengini alır |
| [getHorizontalPageBreaks()](#getHorizontalPageBreaks--) | [HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection) koleksiyonunu alır. |
| [getHyperlinks()](#getHyperlinks--) | [HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection) koleksiyonunu alır. |
| [getIndex()](#getIndex--) | Çalışma sayfası koleksiyonundaki sayfanın indeksini alır. |
| [getListObjects()](#getListObjects--) | Bu çalışma sayfasındaki tüm ListObjects öğelerini alır. |
| [getName()](#getName--) | Çalışma sayfasının adını alır. |
| [getOleObjects()](#getOleObjects--) | Bir çalışma sayfasındaki [OleObject](../../com.aspose.cells/oleobject) koleksiyonunu temsil eder. |
| [getOutline()](#getOutline--) | Bu çalışma sayfasındaki anahatı alır. |
| [getPageSetup()](#getPageSetup--) | Bu sayfadaki sayfa ayarı açıklamasını temsil eder. |
| [getPaneState()](#getPaneState--) | Bölmenin yatay mı yoksa dikey mi bölünmüş olduğunu ve bu bölünmelerin dondurulup dondurulmadığını gösterir. |
| [getPanes()](#getPanes--) | Pencere bölmelerini alır. |
| [getPictures()](#getPictures--) | Bir [Picture](../../com.aspose.cells/picture) koleksiyonu alır. |
| [getPivotTables()](#getPivotTables--) | Bu çalışma sayfasındaki tüm pivot tabloları alır. |
| [getPrintingPageBreaks(ImageOrPrintOptions options)](#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-) | Otomatik sayfa sonlarını alır. |
| [getProtection()](#getProtection--) | Bir çalışma sayfası için mevcut çeşitli koruma seçenekleri tiplerini temsil eder. |
| [getQueryTables()](#getQueryTables--) | Çalışma sayfasındaki [QueryTableCollection](../../com.aspose.cells/querytablecollection) alır. |
| [getScenarios()](#getScenarios--) | [Scenario](../../com.aspose.cells/scenario) koleksiyonunu alır. |
| [getSelectedAreas()](#getSelectedAreas--) | Tasarımcı elektronik tablosundaki seçili hücre aralıklarını alır. |
| [getSelectedRanges()](#getSelectedRanges--) | Tasarımcı elektronik tablosundaki seçili hücre aralıklarını alır. |
| [getShapes()](#getShapes--) | Bu çalışma sayfasındaki tüm çizim şekillerini döndürür. |
| [getShowDataTypeIcons()](#getShowDataTypeIcons--) | Veri tipi simgelerinin gösterilip gösterilmeyeceğini belirtir. |
| [getShowFormulas()](#getShowFormulas--) | Formüllerin mi yoksa sonuçlarının mı gösterileceğini belirtir. |
| [getSlicers()](#getSlicers--) | Çalışma sayfasındaki Slicer koleksiyonunu al. |
| [getSmartTagSetting()](#getSmartTagSetting--) | Çalışma sayfasının tüm [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnelerini alır. |
| [getSparklineGroups()](#getSparklineGroups--) | Çalışma sayfasındaki sparkline gruplarını alır. |
| [getTabColor()](#getTabColor--) | Çalışma sayfası sekme rengini temsil eder. |
| [getTabId()](#getTabId--) | Sayfa için dahili tanımlayıcıyı belirtir. |
| [getTextBoxes()](#getTextBoxes--) | Bir [TextBox](../../com.aspose.cells/textbox) koleksiyonu alır. |
| [getTimelines()](#getTimelines--) | Çalışma sayfasındaki Timeline koleksiyonunu al. |
| [getTransitionEntry()](#getTransitionEntry--) | Geçiş Formülü Girişi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını belirtir. |
| [getTransitionEvaluation()](#getTransitionEvaluation--) | Geçiş Formülü Değerlendirmesi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını belirtir. |
| [getType()](#getType--) | Çalışma sayfası türünü temsil eder. |
| [getUniqueId()](#getUniqueId--) | Benzersiz kimliği alır, \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\} ile aynıdır. |
| [getValidations()](#getValidations--) | Çalışma sayfasındaki veri doğrulama ayarları koleksiyonunu alır. |
| [getVerticalPageBreaks()](#getVerticalPageBreaks--) | [VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection) koleksiyonunu alır. |
| [getViewType()](#getViewType--) | Görünüm tipini alır. |
| [getVisibilityType()](#getVisibilityType--) | Bu sayfanın görünür durumunu belirtir. |
| [getWorkbook()](#getWorkbook--) | Bu sayfayı içeren çalışma kitabı nesnesini alır. |
| [getZoom()](#getZoom--) | Yüzde olarak ölçekleme faktörünü temsil eder. |
| [hasAutofilter()](#hasAutofilter--) | Bu çalışma sayfasının otomatik filtreye sahip olup olmadığını gösterir. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Izgara çizgilerinin görünür olup olmadığını gösteren bir değeri alır. Varsayılan değer true'tır. |
| [isOutlineShown()](#isOutlineShown--) | Anahatın gösterilip gösterilmeyeceğini belirtir. |
| [isPageBreakPreview()](#isPageBreakPreview--) | Belirtilen çalışma sayfasının normal görünümde mi yoksa sayfa kırılımı önizlemesinde mi gösterileceğini belirtir. |
| [isProtected()](#isProtected--) | Çalışma sayfasının korumalı olup olmadığını belirtir. |
| [isRowColumnHeadersVisible()](#isRowColumnHeadersVisible--) | Çalışma sayfasının satır ve sütun başlıklarını gösterip göstermeyeceğini belirten bir değeri alır. |
| [isRulerVisible()](#isRulerVisible--) | Cetvelin görünür olup olmadığını belirtir. |
| [isSelected()](#isSelected--) | Bu çalışma sayfasının, çalışma kitabı açıldığında seçili olup olmadığını belirtir. |
| [isVisible()](#isVisible--) | Çalışma sayfasının görünür olup olmadığını temsil eder. |
| [moveTo(int index)](#moveTo-int-) | Sayfayı elektronik tabloda başka bir konuma taşır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [protect(int type)](#protect-int-) | Çalışma sayfasını korur. |
| [protect(int type, String password, String oldPassword)](#protect-int-java.lang.String-java.lang.String-) | Çalışma sayfasını korur. |
| [refreshPivotTables()](#refreshPivotTables--) | Bu çalışma sayfasındaki tüm PivotTable'ları yeniler. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Bu çalışma sayfasındaki tüm PivotTable'ları yeniler. |
| [removeAllDrawingObjects()](#removeAllDrawingObjects--) | Bu çalışma sayfasındaki tüm çizim nesnelerini kaldırır. |
| [removeAutoFilter()](#removeAutoFilter--) | Çalışma sayfasının otomatik filtresini kaldırır. |
| [removeSplit()](#removeSplit--) | Bölünmüş pencereyi kaldırır. |
| [replace(String oldString, String newString)](#replace-java.lang.String-java.lang.String-) | Tüm hücrelerin metnini yeni bir dizeyle değiştirir. |
| [selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)](#selectRange-int-int-int-int-boolean-) | Bir aralığı seçer. |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Çalışma sayfasındaki etkin hücreyi ayarlar. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Çalışma sayfasının arka plan resmini ayarlar. |
| [setCodeName(String value)](#setCodeName-java.lang.String-) | Çalışma sayfasının kod adını alır. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Belirtilen çalışma sayfasının soldan sağa yerine sağdan sola görüntülenip görüntülenmediğini gösterir. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | Sıfır değerler gösteriliyorsa doğru. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | İlk görünen sütun indeksini temsil eder. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | İlk görünen satır indeksini temsil eder. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Izgara çizgisinin rengini ayarlar |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Izgara çizgilerinin görünür olup olmadığını gösteren bir değeri ayarlar. Varsayılan değer true'tır. |
| [setName(String value)](#setName-java.lang.String-) | Çalışma sayfasının adını ayarlar. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Anahatın gösterilip gösterilmeyeceğini belirtir. |
| [setPageBreakPreview(boolean value)](#setPageBreakPreview-boolean-) | Belirtilen çalışma sayfasının normal görünümde mi yoksa sayfa kırılımı önizlemesinde mi gösterileceğini belirtir. |
| [setRowColumnHeadersVisible(boolean value)](#setRowColumnHeadersVisible-boolean-) | Çalışma sayfasının satır ve sütun başlıklarını gösterip göstermeyeceğini belirten bir değeri ayarlar. |
| [setRulerVisible(boolean value)](#setRulerVisible-boolean-) | Cetvelin görünür olup olmadığını belirtir. |
| [setSelected(boolean value)](#setSelected-boolean-) | Bu çalışma sayfasının, çalışma kitabı açıldığında seçili olup olmadığını belirtir. |
| [setShowDataTypeIcons(boolean value)](#setShowDataTypeIcons-boolean-) | Veri tipi simgelerinin gösterilip gösterilmeyeceğini belirtir. |
| [setShowFormulas(boolean value)](#setShowFormulas-boolean-) | Formüllerin mi yoksa sonuçlarının mı gösterileceğini belirtir. |
| [setTabColor(Color value)](#setTabColor-com.aspose.cells.Color-) | Çalışma sayfası sekme rengini temsil eder. |
| [setTabId(int value)](#setTabId-int-) | Sayfa için dahili tanımlayıcıyı belirtir. |
| [setTransitionEntry(boolean value)](#setTransitionEntry-boolean-) | Geçiş Formülü Girişi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını belirtir. |
| [setTransitionEvaluation(boolean value)](#setTransitionEvaluation-boolean-) | Geçiş Formülü Değerlendirmesi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını belirtir. |
| [setType(int value)](#setType-int-) | Çalışma sayfası türünü temsil eder. |
| [setUniqueId(String value)](#setUniqueId-java.lang.String-) | Benzersiz kimliği ayarlar, bu \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\} ile aynı. |
| [setViewType(int value)](#setViewType-int-) | Görünüm türünü ayarlar. |
| [setVisibilityType(int value)](#setVisibilityType-int-) | Bu sayfanın görünür durumunu belirtir. |
| [setVisible(boolean value)](#setVisible-boolean-) | Çalışma sayfasının görünür olup olmadığını temsil eder. |
| [setVisible(boolean isVisible, boolean ignoreError)](#setVisible-boolean-boolean-) | Görünür seçenekleri ayarlar. |
| [setZoom(int value)](#setZoom-int-) | Yüzde olarak ölçekleme faktörünü temsil eder. |
| [split()](#split--) | Pencereyi böler. |
| [startAccessCache(int opts)](#startAccessCache-int-) | Bu çalışma sayfasındaki verilere erişmek için önbellekleri kullanan oturumu başlatır. |
| [toString()](#toString--) | Geçerli Worksheet nesnesini temsil eden bir dize döndürür. |
| [unFreezePanes()](#unFreezePanes--) | Çalışma sayfasındaki bölmeleri dondurmayı kaldırır. |
| [unprotect()](#unprotect--) | Çalışma sayfasının korumasını kaldırır. |
| [unprotect(String password)](#unprotect-java.lang.String-) | Çalışma sayfasının korumasını kaldırır. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [xmlMapQuery(String path, XmlMap xmlMap)](#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-) | XML haritasının belirli yoluna eşlenen/bağlanan hücre alanlarını sorgular. |
### addPageBreaks(String cellName) {#addPageBreaks-java.lang.String-}
```
public void addPageBreaks(String cellName)
```


Sayfa sonu ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String |  |

### advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly) {#advancedFilter-boolean-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public void advancedFilter(boolean isFilter, String listRange, String criteriaRange, String copyTo, boolean uniqueRecordOnly)
```


Verileri karmaşık ölçütlerle filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isFilter | boolean | Listenin yerinde filtrelenip filtrelenmediğini gösterir. |
| listRange | java.lang.String | Liste aralığı. |
| criteriaRange | java.lang.String | Kriter aralığı. |
| copyTo | java.lang.String | Verilerin kopyalanacağı aralık. |
| uniqueRecordOnly | boolean | Yalnızca benzersiz satırları görüntüleme veya kopyalama. |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Sütun genişliğini otomatik olarak ayarlar.

**Remarks**

AutoFitColumn, kesin olmayan bir işlevdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Sütun genişliğini otomatik olarak ayarlar.

**Remarks**

Bu yöntem, satır içindeki hücre aralığındaki içeriğe göre satırı otomatik olarak sığdırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | int | Sütun indeksi. |
| firstRow | int | İlk satır indeksi. |
| lastRow | int | Son satır indeksi. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```


Bu çalışma sayfasındaki tüm sütunları otomatik olarak ayarlar.

### autoFitColumns(AutoFitterOptions options) {#autoFitColumns-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(AutoFitterOptions options)
```


Bu çalışma sayfasındaki tüm sütunları otomatik olarak ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Otomatik sığdırma seçenekleri |

### autoFitColumns(int firstColumn, int lastColumn) {#autoFitColumns-int-int-}
```
public void autoFitColumns(int firstColumn, int lastColumn)
```


Sütunların genişliğini otomatik olarak ayarlar.

**Remarks**

AutoFitColumn, kesin olmayan bir işlevdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstColumn | int | İlk sütun indeksi. |
| lastColumn | int | Son sütun indeksi. |

### autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```


Sütunların genişliğini otomatik olarak ayarlar.

**Remarks**

AutoFitColumn, kesin olmayan bir işlevdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstColumn | int | İlk sütun indeksi. |
| lastColumn | int | Son sütun indeksi. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Otomatik sığdırma seçenekleri |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn) {#autoFitColumns-int-int-int-int-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```


Sütunların genişliğini otomatik olarak ayarlar.

**Remarks**

AutoFitColumn, kesin olmayan bir işlevdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | İlk satır indeksi. |
| firstColumn | int | İlk sütun indeksi. |
| lastRow | int | Son satır indeksi. |
| lastColumn | int | Son sütun indeksi. |

### autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options) {#autoFitColumns-int-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, AutoFitterOptions options)
```


Sütunların genişliğini otomatik olarak ayarlar.

**Remarks**

AutoFitColumn, kesin olmayan bir işlevdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | İlk satır indeksi. |
| firstColumn | int | İlk sütun indeksi. |
| lastRow | int | Son satır indeksi. |
| lastColumn | int | Son sütun indeksi. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Otomatik sığdırma seçenekleri |

### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Satır yüksekliğini otomatik olarak ayarlar.

**Remarks**

AutoFitRow, kesin olmayan bir işlevdir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Satır yüksekliğini otomatik olarak ayarlar.

**Remarks**

Bu yöntem, satır içindeki hücre aralığındaki içeriğe göre satırı otomatik olarak sığdırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |
| firstColumn | int | İlk sütun indeksi. |
| lastColumn | int | Son sütun indeksi. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options) {#autoFitRow-int-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```


Satır yüksekliğini otomatik olarak ayarlar.

**Remarks**

Bu yöntem, satır içindeki hücre aralığındaki içeriğe göre satırı otomatik olarak sığdırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int | Satır indeksi. |
| firstColumn | int | İlk sütun indeksi. |
| lastColumn | int | Son sütun indeksi. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Otomatik sığdırıcı seçenekleri |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Dikdörtgen bir aralıktaki satır yüksekliğini otomatik olarak ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi. |
| endRow | int | Bitiş satır indeksi. |
| startColumn | int | Başlangıç sütun indeksi. |
| endColumn | int | Bitiş sütun indeksi. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| onlyAuto | boolean | Doğru, yalnızca satır yüksekliği özelleştirilmediğinde satır yüksekliğini otomatik olarak sığdırır. |

### autoFitRows(AutoFitterOptions options) {#autoFitRows-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(AutoFitterOptions options)
```


Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Otomatik sığdırıcı seçenekleri |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Bir aralıktaki satır yüksekliğini otomatik olarak ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi. |
| endRow | int | Bitiş satır indeksi. |

### autoFitRows(int startRow, int endRow, AutoFitterOptions options) {#autoFitRows-int-int-com.aspose.cells.AutoFitterOptions-}
```
public void autoFitRows(int startRow, int endRow, AutoFitterOptions options)
```


Bir aralıktaki satır yüksekliğini otomatik olarak ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi. |
| endRow | int | Bitiş satır indeksi. |
| options | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) | Otomatik sığdırıcının seçenekleri. |

### calculateArrayFormula(String formula, CalculationOptions opts) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts)
```


Bir formülü dizi formülü olarak hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Hesaplanacak formül. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Formül hesaplama seçenekleri |

**Returns:**
java.lang.Object[][]
### calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount) {#calculateArrayFormula-java.lang.String-com.aspose.cells.CalculationOptions-int-int-}
```
public Object[][] calculateArrayFormula(String formula, CalculationOptions opts, int maxRowCount, int maxColumnCount)
```


Bir formülü dizi formülü olarak hesaplar.

**Remarks**

Formül, boyutu ve sonucu hesaplamak için dinamik dizi formülü olarak alınacaktır. Kullanıcı tarafından belirtilen maksimum boyut, hesaplanan sonucun büyük bir veri kümesi olduğu durumlarda (örneğin, hesaplanan sonuç bir bütün satır veya sütun verisine karşılık gelebilir) ancak iş gereksinimi veya performans düşüncesi nedeniyle kullanıcı bu kadar büyük bir diziye ihtiyaç duymadığında kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Hesaplanacak formül. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Formül hesaplama seçenekleri |
| maxRowCount | int | sonuç verisinin maksimum satır sayısı. Eğer pozitif olmayan bir değer ya da gerçek satır sayısından büyükse, gerçek satır sayısı kullanılacaktır. |
| maxColumnCount | int | sonuç verisinin maksimum sütun sayısı. Eğer pozitif olmayan bir değer ya da gerçek sütun sayısından büyükse, gerçek sütun sayısı kullanılacaktır. |

**Returns:**
java.lang.Object[][] - Hesaplanmış formül sonucu.
### calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData) {#calculateArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-int-int-com.aspose.cells.CalculationData-}
```
public Object[][] calculateArrayFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, int maxColumnCount, CalculationData calculationData)
```


Bir formülü dizi formülü olarak hesaplar.

**Remarks**

Formül, boyutu ve sonucu hesaplamak için dinamik dizi formülü olarak alınacaktır. Kullanıcı tarafından belirtilen maksimum boyut, hesaplanan sonucun büyük bir veri kümesi olduğu durumlarda (örneğin, hesaplanan sonuç bir bütün satır veya sütun verisine karşılık gelebilir) ancak iş gereksinimi veya performans düşüncesi nedeniyle kullanıcı bu kadar büyük bir diziye ihtiyaç duymadığında kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Hesaplanacak formül. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Formül ayrıştırma seçenekleri |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Formül hesaplama seçenekleri |
| baseCellRow | int | Temel hücrenin satır indeksi. |
| baseCellColumn | int | Temel hücrenin sütun indeksi. |
| maxRowCount | int | Sonuç verisinin maksimum satır sayısı. Eğer pozitif olmayan bir değer ya da gerçek satır sayısından büyükse, gerçek satır sayısı kullanılacaktır. |
| maxColumnCount | int | Sonuç verisinin maksimum sütun sayısı. Eğer sıfır veya negatif ise ya da gerçek satır sayısından büyükse, gerçek sütun sayısı kullanılacaktır. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | Hesaplama verileri. Kullanıcı özel bir hesaplama motoru uygularken bazı statik formülleri hesaplaması gerektiğinde bu durum için kullanılır. Bu tür bir durumda, kullanıcı bunu [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) için sağlanan hesaplama verileriyle belirtmelidir. |

**Returns:**
java.lang.Object[][] - Hesaplanmış formül sonucu.
### calculateFormula(CalculationOptions options, boolean recursive) {#calculateFormula-com.aspose.cells.CalculationOptions-boolean-}
```
public void calculateFormula(CalculationOptions options, boolean recursive)
```


Bu çalışma sayfasındaki tüm formülleri hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Hesaplama seçenekleri |
| recursive | boolean | True, çalışma sayfasının hücreleri diğer çalışma sayfalarının hücrelerine bağımlıysa, bağımlı hücrelerin de diğer çalışma sayfalarında hesaplanacağını ifade eder. False ise çalışma sayfasındaki tüm formüllerin hesaplandığını ve değerlerin doğru olduğunu gösterir. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Bir formülü hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Hesaplanacak formül. |

**Returns:**
java.lang.Object - Hesaplanmış formül sonucu.
### calculateFormula(String formula, CalculationOptions opts) {#calculateFormula-java.lang.String-com.aspose.cells.CalculationOptions-}
```
public Object calculateFormula(String formula, CalculationOptions opts)
```


Bir formül ifadesini doğrudan hesaplar.

**Remarks**

Formül, A1 hücresine ayarlanmış gibi hesaplanacaktır. Ve formül normal bir formül olarak alınacaktır. Formülün bir dizi formülü olarak hesaplanması ve hesaplanmış sonuç için bir dizi alınması gerekiyorsa, lütfen [calculateArrayFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-CalculationOptions-) kullanın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Hesaplanacak formül. |
| opts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Formül hesaplama seçenekleri |

**Returns:**
java.lang.Object - Verilen formülün hesaplanmış sonucu. Döndürülen nesne, [Cell.getValue()](../../com.aspose.cells/cell\#getValue--) gibi olası tiplerden biri ya da ReferredArea olabilir.
### calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData) {#calculateFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-com.aspose.cells.CalculationOptions-int-int-com.aspose.cells.CalculationData-}
```
public Object calculateFormula(String formula, FormulaParseOptions pOpts, CalculationOptions cOpts, int baseCellRow, int baseCellColumn, CalculationData calculationData)
```


Bir formül ifadesini doğrudan hesaplar.

**Remarks**

Formül, belirtilen temel hücreye ayarlanmış gibi hesaplanacaktır. Ve formül normal bir formül olarak alınacaktır. Formülün bir dizi formülü olarak hesaplanması ve hesaplanmış sonuç için bir dizi alınması gerekiyorsa, lütfen [calculateArrayFormula(String,FormulaParseOptions,CalculationOptions,int,int,int,int,CalculationData)](../../com.aspose.cells/worksheet\#calculateArrayFormula-String-FormulaParseOptions-CalculationOptions-int-int-int-int-CalculationData-) kullanın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Hesaplanacak formül. |
| pOpts | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Formül ayrıştırma seçenekleri. |
| cOpts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Formül hesaplama seçenekleri. |
| baseCellRow | int | Temel hücrenin satır indeksi. |
| baseCellColumn | int | Temel hücrenin sütun indeksi. |
| calculationData | [CalculationData](../../com.aspose.cells/calculationdata) | Hesaplama verileri. Kullanıcı özel bir hesaplama motoru uygularken bazı statik formülleri hesaplaması gerektiğinde bu durum için kullanılır. Bu tür bir durumda, kullanıcı bunu [AbstractCalculationEngine.calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) için sağlanan hesaplama verileriyle belirtmelidir. |

**Returns:**
java.lang.Object - Verilen formülün hesaplanmış sonucu. Döndürülen nesne, [Cell.getValue()](../../com.aspose.cells/cell\#getValue--) gibi olası tiplerden biri ya da ReferredArea olabilir.
### clearComments() {#clearComments--}
```
public void clearComments()
```


Tasarımcı elektronik tablosundaki tüm yorumları temizler.

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Bu çalışma sayfasındaki verilere erişmek için önbellek kullanan oturumu kapatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). veri erişim seçenekleri |

### convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn) {#convertFormulaReferenceStyle-java.lang.String-boolean-int-int-}
```
public String convertFormulaReferenceStyle(String formula, boolean toR1C1, int baseCellRow, int baseCellColumn)
```


Formül referans stilini dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Dönüştürülecek formül. |
| toR1C1 | boolean | Formülün hangi referans stiline dönüştürüleceği. Orijinal formül A1 referans stilindeyse, bu değer true olmalı, böylece formül A1'den R1C1 referans stiline dönüştürülür; Orijinal formül R1C1 referans stilindeyse, bu değer false olmalı, böylece formül R1C1'den A1 referans stiline dönüştürülür; |
| baseCellRow | int | Temel hücrenin satır indeksi. |
| baseCellColumn | int | Temel hücrenin sütun indeksi. |

**Returns:**
java.lang.String - Dönüştürülmüş formül.
### copy(Worksheet sourceSheet) {#copy-com.aspose.cells.Worksheet-}
```
public void copy(Worksheet sourceSheet)
```


Başka bir çalışma sayfasından içerikleri ve biçimleri kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Kaynak çalışma sayfası. |

### copy(Worksheet sourceSheet, CopyOptions copyOptions) {#copy-com.aspose.cells.Worksheet-com.aspose.cells.CopyOptions-}
```
public void copy(Worksheet sourceSheet, CopyOptions copyOptions)
```


Başka bir çalışma sayfasından içerikleri ve biçimleri kopyalar.

**Remarks**

Aynı dosyadaki ya da başka bir dosyadaki başka bir çalışma sayfasından veri kopyalayabilirsiniz. Ancak bu yöntem, yorumlar, resimler ve grafikler gibi çizim nesnelerinin kopyalanmasını desteklemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceSheet | [Worksheet](../../com.aspose.cells/worksheet) | Kaynak çalışma sayfası. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) |  |

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
### filter(CellArea ca) {#filter-com.aspose.cells.CellArea-}
```
public void filter(CellArea ca)
```


Aralığı filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Aralık |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur.

**Remarks**

Satır indeksi ve sütun indeksi aynı anda sıfır olamaz. Satır sayısı ve sütun sayısı da aynı anda sıfır olamaz.

İlk iki parametre dondurulmuş konumu, son iki parametre ise sol üst bölmede dondurulmuş alanı belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |
| freezedRows | int | Üst bölmede görünen satır sayısı, satır indeksinden fazla olamaz. |
| freezedColumns | int | Sol bölmede görünen sütun sayısı, sütun indeksinden fazla olamaz. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur.

**Remarks**

Satır indeksi ve sütun indeksi aynı anda sıfır olamaz. Satır sayısı ve sütun sayısı da aynı anda sıfır olamaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı. |
| freezedRows | int | Üst bölmede görünen satır sayısı, satır indeksinden fazla olamaz. |
| freezedColumns | int | Sol bölmede görünen sütun sayısı, sütun indeksinden fazla olamaz. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


Çalışma sayfasındaki etkin hücreyi alır.

**Returns:**
java.lang.String
### getAdvancedFilter() {#getAdvancedFilter--}
```
public AdvancedFilter getAdvancedFilter()
```


Gelişmiş filtrenin ayarlarını alır.

**Returns:**
[AdvancedFilter](../../com.aspose.cells/advancedfilter) - 
### getAllPictures() {#getAllPictures--}
```
public Picture[] getAllPictures()
```


Hücreye gömülü ve hücrelerin üzerindeki tüm resimleri alır.

**Returns:**
com.aspose.cells.Picture[] -
### getAllowEditRanges() {#getAllowEditRanges--}
```
public ProtectedRangeCollection getAllowEditRanges()
```


Çalışma sayfasındaki düzenleme izinli aralık koleksiyonunu alır.

**Returns:**
[ProtectedRangeCollection](../../com.aspose.cells/protectedrangecollection)
### getAreasOfXmlMapQuery(String path, XmlMap xmlMap) {#getAreasOfXmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public CellArea[] getAreasOfXmlMapQuery(String path, XmlMap xmlMap)
```


XML haritasının belirli yoluna eşlenen/bağlanan hücre alanlarını sorgular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | java.lang.String | xml öğe yolu |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Belirli bir harita içinde belirli bir yolu sorgulamak istiyorsanız bir xml haritası belirtin |

**Returns:**
com.aspose.cells.CellArea[] - [CellArea](../../com.aspose.cells/cellarea) listesi, xml haritasının belirli yoluna eşlenen/bağlanan, hiçbir şey eşlenmez/bağlanmazsa boş bir liste döndürülür.
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Belirtilen çalışma sayfası için otomatik filtreyi temsil eder.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Çalışma sayfasının arka plan resmini alır.

**Returns:**
byte[]
### getCellWatches() {#getCellWatches--}
```
public CellWatchCollection getCellWatches()
```


Bu çalışma sayfasında 'watch window' içinde izlenen hücrelerin koleksiyonunu alır.

**Returns:**
[CellWatchCollection](../../com.aspose.cells/cellwatchcollection)
### getCells() {#getCells--}
```
public Cells getCells()
```


[Cells](../../com.aspose.cells/cells) koleksiyonunu alır.

**Returns:**
[Cells](../../com.aspose.cells/cells)
### getCharts() {#getCharts--}
```
public ChartCollection getCharts()
```


[Chart](../../com.aspose.cells/chart) koleksiyonunu alır

**Returns:**
[ChartCollection](../../com.aspose.cells/chartcollection)
### getCheckBoxes() {#getCheckBoxes--}
```
public CheckBoxCollection getCheckBoxes()
```


[CheckBox](../../com.aspose.cells/checkbox) koleksiyonunu alır.

**Returns:**
[CheckBoxCollection](../../com.aspose.cells/checkboxcollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Çalışma sayfasının kod adını alır.

**Returns:**
java.lang.String
### getComments() {#getComments--}
```
public CommentCollection getComments()
```


[Comment](../../com.aspose.cells/comment) koleksiyonunu alır.

**Returns:**
[CommentCollection](../../com.aspose.cells/commentcollection)
### getConditionalFormattings() {#getConditionalFormattings--}
```
public ConditionalFormattingCollection getConditionalFormattings()
```


Çalışma sayfasındaki ConditionalFormattings öğelerini alır.

**Returns:**
[ConditionalFormattingCollection](../../com.aspose.cells/conditionalformattingcollection)
### getCustomProperties() {#getCustomProperties--}
```
public CustomPropertyCollection getCustomProperties()
```


Bir çalışma sayfasıyla ilişkili tanımlayıcı bilgilerini temsil eden nesneyi alır.

**Remarks**

Worksheet.CustomProperties, rastgele veri depolamak için tercih edilen bir mekanizma sağlar. Eski üçüncü taraf belge bileşenlerini ve ikili parçalara sıkı bir ihtiyaç duyan durumları da destekler.

**Returns:**
[CustomPropertyCollection](../../com.aspose.cells/custompropertycollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


Belirtilen çalışma sayfasının soldan sağa yerine sağdan sola görüntülenip görüntülenmediğini gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


Sıfır değerler gösteriliyorsa doğru.

**Returns:**
boolean
### getErrorCheckOptions() {#getErrorCheckOptions--}
```
public ErrorCheckOptionCollection getErrorCheckOptions()
```


Belirli aralıklara uygulanan hata kontrol ayarını alır.

**Returns:**
[ErrorCheckOptionCollection](../../com.aspose.cells/errorcheckoptioncollection)
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


İlk görünen sütun indeksini temsil eder.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


İlk görünen satır indeksini temsil eder.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Dondurulmuş bölmeleri alır.

**Returns:**
int[] - null döndürmek, çalışma sayfasının dondurulmadığını gösterir 0:Satır indeksi;1:sütun;2:dondurulmuşSatırlar;3:dondurulmuşSatırlar
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Izgara çizgisi rengini alır

**Returns:**
[Color](../../com.aspose.cells/color)
### getHorizontalPageBreaks() {#getHorizontalPageBreaks--}
```
public HorizontalPageBreakCollection getHorizontalPageBreaks()
```


[HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection) koleksiyonunu alır.

**Returns:**
[HorizontalPageBreakCollection](../../com.aspose.cells/horizontalpagebreakcollection)
### getHyperlinks() {#getHyperlinks--}
```
public HyperlinkCollection getHyperlinks()
```


[HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection) koleksiyonunu alır.

**Returns:**
[HyperlinkCollection](../../com.aspose.cells/hyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Çalışma sayfası koleksiyonundaki sayfanın indeksini alır.

**Returns:**
int
### getListObjects() {#getListObjects--}
```
public ListObjectCollection getListObjects()
```


Bu çalışma sayfasındaki tüm ListObjects öğelerini alır.

**Returns:**
[ListObjectCollection](../../com.aspose.cells/listobjectcollection)
### getName() {#getName--}
```
public String getName()
```


Çalışma sayfasının adını alır.

**Remarks**

Çalışma sayfası adının maksimum uzunluğu 31'dir. Aynı adı (büyük/küçük harf duyarsız) iki çalışma sayfasına atayamazsınız. Örneğin, \"SheetName1\" değerini ilk çalışma sayfasına, \"SHEETNAME1\" değerini ikinci çalışma sayfasına atayamazsınız.

**Returns:**
java.lang.String
### getOleObjects() {#getOleObjects--}
```
public OleObjectCollection getOleObjects()
```


Bir çalışma sayfasındaki [OleObject](../../com.aspose.cells/oleobject) koleksiyonunu temsil eder.

**Returns:**
[OleObjectCollection](../../com.aspose.cells/oleobjectcollection)
### getOutline() {#getOutline--}
```
public Outline getOutline()
```


Bu çalışma sayfasındaki anahatı alır.

**Returns:**
[Outline](../../com.aspose.cells/outline)
### getPageSetup() {#getPageSetup--}
```
public PageSetup getPageSetup()
```


Bu sayfadaki sayfa ayarı açıklamasını temsil eder.

**Returns:**
[PageSetup](../../com.aspose.cells/pagesetup)
### getPaneState() {#getPaneState--}
```
public int getPaneState()
```


Bölmenin yatay mı yoksa dikey mi bölünmüş olduğunu ve bu bölünmelerin dondurulup dondurulmadığını gösterir.

Bakınız [PaneStateType](../../com.aspose.cells/panestatetype).

**Returns:**
int
### getPanes() {#getPanes--}
```
public PaneCollection getPanes()
```


Pencere bölmelerini alır.

**Remarks**

Pencere bölünmemiş veya dondurulmamışsa.

**Returns:**
[PaneCollection](../../com.aspose.cells/panecollection)
### getPictures() {#getPictures--}
```
public PictureCollection getPictures()
```


Bir [Picture](../../com.aspose.cells/picture) koleksiyonu alır.

**Returns:**
[PictureCollection](../../com.aspose.cells/picturecollection)
### getPivotTables() {#getPivotTables--}
```
public PivotTableCollection getPivotTables()
```


Bu çalışma sayfasındaki tüm pivot tabloları alır.

**Returns:**
[PivotTableCollection](../../com.aspose.cells/pivottablecollection)
### getPrintingPageBreaks(ImageOrPrintOptions options) {#getPrintingPageBreaks-com.aspose.cells.ImageOrPrintOptions-}
```
public CellArea[] getPrintingPageBreaks(ImageOrPrintOptions options)
```


Otomatik sayfa sonlarını alır.

**Remarks**

Her hücre alanı bir kağıdı temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Yazdırma seçenekleri |

**Returns:**
com.aspose.cells.CellArea[] - Otomatik sayfa sonu alanları.
### getProtection() {#getProtection--}
```
public Protection getProtection()
```


Bir çalışma sayfası için mevcut olan çeşitli koruma seçeneklerini temsil eder. ExcelXP ve üzeri sürümlerde gelişmiş koruma seçeneklerini destekler.

**Remarks**

Bu özellik, Excel dosyasının tüm sürümlerinde çalışma sayfasını koruyabilir ve ExcelXP ve üzeri sürümlerde gelişmiş koruma seçeneklerini destekler.

**Returns:**
[Protection](../../com.aspose.cells/protection)
### getQueryTables() {#getQueryTables--}
```
public QueryTableCollection getQueryTables()
```


Çalışma sayfasındaki [QueryTableCollection](../../com.aspose.cells/querytablecollection) alır.

**Returns:**
[QueryTableCollection](../../com.aspose.cells/querytablecollection)
### getScenarios() {#getScenarios--}
```
public ScenarioCollection getScenarios()
```


[Scenario](../../com.aspose.cells/scenario) koleksiyonunu alır.

**Returns:**
[ScenarioCollection](../../com.aspose.cells/scenariocollection)
### getSelectedAreas() {#getSelectedAreas--}
```
public Range[] getSelectedAreas()
```


Tasarımcı elektronik tablosundaki seçili hücre aralıklarını alır.

**Returns:**
com.aspose.cells.Range[] - Tüm seçili aralıkları döndürür.
### getSelectedRanges() {#getSelectedRanges--}
```
public ArrayList getSelectedRanges()
```


Tasarımcı elektronik tablosundaki seçili hücre aralıklarını alır.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Worksheet.GetSelectedAreas() yöntemini kullanın. Bu özellik, Mart 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.util.ArrayList - Seçili aralıkları içeren bir ArrayList.
### getShapes() {#getShapes--}
```
public ShapeCollection getShapes()
```


Bu çalışma sayfasındaki tüm çizim şekillerini döndürür.

**Returns:**
[ShapeCollection](../../com.aspose.cells/shapecollection)
### getShowDataTypeIcons() {#getShowDataTypeIcons--}
```
public boolean getShowDataTypeIcons()
```


Veri tipi simgelerinin gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### getShowFormulas() {#getShowFormulas--}
```
public boolean getShowFormulas()
```


Formüllerin mi yoksa sonuçlarının mı gösterileceğini belirtir.

**Returns:**
boolean
### getSlicers() {#getSlicers--}
```
public SlicerCollection getSlicers()
```


Çalışma sayfasındaki Slicer koleksiyonunu al.

**Returns:**
[SlicerCollection](../../com.aspose.cells/slicercollection)
### getSmartTagSetting() {#getSmartTagSetting--}
```
public SmartTagSetting getSmartTagSetting()
```


Çalışma sayfasının tüm [SmartTagCollection](../../com.aspose.cells/smarttagcollection) nesnelerini alır.

**Returns:**
[SmartTagSetting](../../com.aspose.cells/smarttagsetting)
### getSparklineGroups() {#getSparklineGroups--}
```
public SparklineGroupCollection getSparklineGroups()
```


Çalışma sayfasındaki sparkline gruplarını alır.

**Returns:**
[SparklineGroupCollection](../../com.aspose.cells/sparklinegroupcollection)
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Çalışma sayfası sekme rengini temsil eder.

**Remarks**

Bu özellik yalnızca ExcelXP (Excel2002) ve sonraki sürümlerde desteklenir. Dosyayı Excel97 veya Excel2000 formatında kaydederseniz, bu özellik atlanır.

**Returns:**
[Color](../../com.aspose.cells/color)
### getTabId() {#getTabId--}
```
public int getTabId()
```


Sayfa için dahili tanımlayıcıyı belirtir.

**Returns:**
int
### getTextBoxes() {#getTextBoxes--}
```
public TextBoxCollection getTextBoxes()
```


Bir [TextBox](../../com.aspose.cells/textbox) koleksiyonu alır.

**Returns:**
[TextBoxCollection](../../com.aspose.cells/textboxcollection)
### getTimelines() {#getTimelines--}
```
public TimelineCollection getTimelines()
```


Çalışma sayfasındaki Timeline koleksiyonunu al.

**Returns:**
[TimelineCollection](../../com.aspose.cells/timelinecollection)
### getTransitionEntry() {#getTransitionEntry--}
```
public boolean getTransitionEntry()
```


Geçiş Formülü Girişi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını belirtir.

**Returns:**
boolean
### getTransitionEvaluation() {#getTransitionEvaluation--}
```
public boolean getTransitionEvaluation()
```


Geçiş Formülü Değerlendirmesi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını belirtir.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Çalışma sayfası türünü temsil eder.

Bakınız [SheetType](../../com.aspose.cells/sheettype).

**Returns:**
int
### getUniqueId() {#getUniqueId--}
```
public String getUniqueId()
```


Benzersiz kimliği alır, \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\} ile aynıdır.

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public ValidationCollection getValidations()
```


Çalışma sayfasındaki veri doğrulama ayarları koleksiyonunu alır.

**Returns:**
[ValidationCollection](../../com.aspose.cells/validationcollection)
### getVerticalPageBreaks() {#getVerticalPageBreaks--}
```
public VerticalPageBreakCollection getVerticalPageBreaks()
```


[VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection) koleksiyonunu alır.

**Returns:**
[VerticalPageBreakCollection](../../com.aspose.cells/verticalpagebreakcollection)
### getViewType() {#getViewType--}
```
public int getViewType()
```


Görünüm tipini alır.

Bakınız [ViewType](../../com.aspose.cells/viewtype).

**Returns:**
int
### getVisibilityType() {#getVisibilityType--}
```
public int getVisibilityType()
```


Bu sayfanın görünür durumunu belirtir.

Bakınız [VisibilityType](../../com.aspose.cells/visibilitytype).

**Returns:**
int
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Bu sayfayı içeren çalışma kitabı nesnesini alır.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Yüzde olarak ölçekleme faktörünü temsil eder. 10 ile 400 arasında olmalıdır.

**Remarks**

Lütfen önce görünüm tipini ayarlayın.

**Returns:**
int
### hasAutofilter() {#hasAutofilter--}
```
public boolean hasAutofilter()
```


Bu çalışma sayfasının otomatik filtreye sahip olup olmadığını gösterir.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


Izgara çizgilerinin görünür olup olmadığını gösteren bir değeri alır. Varsayılan değer true'tır.

**Returns:**
boolean
### isOutlineShown() {#isOutlineShown--}
```
public boolean isOutlineShown()
```


Anahatın gösterilip gösterilmeyeceğini belirtir.

**Returns:**
boolean
### isPageBreakPreview() {#isPageBreakPreview--}
```
public boolean isPageBreakPreview()
```


Belirtilen çalışma sayfasının normal görünümde mi yoksa sayfa kırılımı önizlemesinde mi gösterileceğini belirtir.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Çalışma sayfasının korumalı olup olmadığını belirtir.

**Returns:**
boolean
### isRowColumnHeadersVisible() {#isRowColumnHeadersVisible--}
```
public boolean isRowColumnHeadersVisible()
```


Çalışma sayfasının satır ve sütun başlıklarını gösterip göstermeyeceğini belirten bir değer alır. Varsayılan değer true'tur.

**Returns:**
boolean
### isRulerVisible() {#isRulerVisible--}
```
public boolean isRulerVisible()
```


Cetvelin görünür olup olmadığını gösterir. Bu özellik yalnızca sayfa sonu önizlemesi için uygulanır.

**Returns:**
boolean
### isSelected() {#isSelected--}
```
public boolean isSelected()
```


Bu çalışma sayfasının, çalışma kitabı açıldığında seçili olup olmadığını belirtir.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Çalışma sayfasının görünür olup olmadığını temsil eder.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Sayfayı elektronik tabloda başka bir konuma taşır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Hedef sayfa indeksi. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### protect(int type) {#protect-int-}
```
public void protect(int type)
```


Çalışma sayfasını korur.

**Remarks**

Bu yöntem, çalışma sayfasını şifre olmadan korur. Excel dosyasının tüm sürümlerinde çalışma sayfasını koruyabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Koruma türü. |

### protect(int type, String password, String oldPassword) {#protect-int-java.lang.String-java.lang.String-}
```
public void protect(int type, String password, String oldPassword)
```


Çalışma sayfasını korur.

**Remarks**

Bu yöntem, Excel dosyasının tüm sürümlerinde çalışma sayfasını koruyabilir.

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = excel.getWorksheets().get(0);
         //Protecting the worksheet with a password
         worksheet.protect(ProtectionType.ALL, "aspose", null);
         //Saving the modified Excel file in default (that is Excel 20003) format
         excel.save("output.xls");
         //Closing the file stream to free all resources
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ProtectionType](../../com.aspose.cells/protectiontype). Koruma türü. |
| password | java.lang.String | Şifre. |
| oldPassword | java.lang.String | Eğer çalışma sayfası zaten bir şifreyle korunuyorsa, lütfen eski şifreyi sağlayın. Aksi takdirde, bu parametreye null değer veya boş bir dize ayarlayabilirsiniz. |

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Bu çalışma sayfasındaki tüm PivotTable'ları yeniler.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Bu çalışma sayfasındaki tüm PivotTable'ları yeniler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Özet tablo veri kaynağını yenileme seçeneği. |

**Returns:**
boolean
### removeAllDrawingObjects() {#removeAllDrawingObjects--}
```
public void removeAllDrawingObjects()
```


Bu çalışma sayfasındaki tüm çizim nesnelerini kaldırır.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Çalışma sayfasının otomatik filtresini kaldırır.

### removeSplit() {#removeSplit--}
```
public void removeSplit()
```


Bölünmüş pencereyi kaldırır.

### replace(String oldString, String newString) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String oldString, String newString)
```


Tüm hücrelerin metnini yeni bir dizeyle değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| oldString | java.lang.String | Eski dize değeri. |
| newString | java.lang.String | Yeni dize değeri. |

**Returns:**
int
### selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers) {#selectRange-int-int-int-int-boolean-}
```
public void selectRange(int startRow, int startColumn, int totalRows, int totalColumns, boolean removeOthers)
```


Bir aralığı seçer.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satırı. |
| startColumn | int | Başlangıç sütunu |
| totalRows | int | Satır sayısı. |
| totalColumns | int | Sütun sayısı |
| removeOthers | boolean | True, diğer seçili aralığı kaldırıp yalnızca bu aralığı seçmek anlamına gelir. |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Çalışma sayfasındaki etkin hücreyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Çalışma sayfasının arka plan resmini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte[] |  |

### setCodeName(String value) {#setCodeName-java.lang.String-}
```
public void setCodeName(String value)
```


Çalışma sayfasının kod adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


Belirtilen çalışma sayfasının soldan sağa yerine sağdan sola görüntülenip görüntülenmediğini gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


Sıfır değerler gösteriliyorsa doğru.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


İlk görünen sütun indeksini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


İlk görünen satır indeksini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Izgara çizgisinin rengini ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Izgara çizgilerinin görünür olup olmadığını gösteren bir değeri ayarlar. Varsayılan değer true'tır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Çalışma sayfasının adını ayarlar.

**Remarks**

Çalışma sayfası adının maksimum uzunluğu 31'dir. Aynı adı (büyük/küçük harf duyarsız) iki çalışma sayfasına atayamazsınız. Örneğin, \"SheetName1\" değerini ilk çalışma sayfasına, \"SHEETNAME1\" değerini ikinci çalışma sayfasına atayamazsınız.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


Anahatın gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPageBreakPreview(boolean value) {#setPageBreakPreview-boolean-}
```
public void setPageBreakPreview(boolean value)
```


Belirtilen çalışma sayfasının normal görünümde mi yoksa sayfa kırılımı önizlemesinde mi gösterileceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRowColumnHeadersVisible(boolean value) {#setRowColumnHeadersVisible-boolean-}
```
public void setRowColumnHeadersVisible(boolean value)
```


Çalışma sayfasının satır ve sütun başlıklarını gösterip göstermeyeceğini belirten bir değer ayarlar. Varsayılan true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRulerVisible(boolean value) {#setRulerVisible-boolean-}
```
public void setRulerVisible(boolean value)
```


Cetvelin görünür olup olmadığını gösterir. Bu özellik yalnızca sayfa sonu önizlemesi için uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Bu çalışma sayfasının, çalışma kitabı açıldığında seçili olup olmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowDataTypeIcons(boolean value) {#setShowDataTypeIcons-boolean-}
```
public void setShowDataTypeIcons(boolean value)
```


Veri tipi simgelerinin gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowFormulas(boolean value) {#setShowFormulas-boolean-}
```
public void setShowFormulas(boolean value)
```


Formüllerin mi yoksa sonuçlarının mı gösterileceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.cells.Color-}
```
public void setTabColor(Color value)
```


Çalışma sayfası sekme rengini temsil eder.

**Remarks**

Bu özellik yalnızca ExcelXP (Excel2002) ve sonraki sürümlerde desteklenir. Dosyayı Excel97 veya Excel2000 formatında kaydederseniz, bu özellik atlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setTabId(int value) {#setTabId-int-}
```
public void setTabId(int value)
```


Sayfa için dahili tanımlayıcıyı belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTransitionEntry(boolean value) {#setTransitionEntry-boolean-}
```
public void setTransitionEntry(boolean value)
```


Geçiş Formülü Girişi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTransitionEvaluation(boolean value) {#setTransitionEvaluation-boolean-}
```
public void setTransitionEvaluation(boolean value)
```


Geçiş Formülü Değerlendirmesi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Çalışma sayfası türünü temsil eder.

Bakınız [SheetType](../../com.aspose.cells/sheettype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setUniqueId(String value) {#setUniqueId-java.lang.String-}
```
public void setUniqueId(String value)
```


Benzersiz kimliği ayarlar, bu \{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F\} ile aynı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setViewType(int value) {#setViewType-int-}
```
public void setViewType(int value)
```


Görünüm türünü ayarlar.

Bakınız [ViewType](../../com.aspose.cells/viewtype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setVisibilityType(int value) {#setVisibilityType-int-}
```
public void setVisibilityType(int value)
```


Bu sayfanın görünür durumunu belirtir.

Bakınız [VisibilityType](../../com.aspose.cells/visibilitytype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Çalışma sayfasının görünür olup olmadığını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setVisible(boolean isVisible, boolean ignoreError) {#setVisible-boolean-boolean-}
```
public void setVisible(boolean isVisible, boolean ignoreError)
```


Görünür seçenekleri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isVisible | boolean | Çalışma sayfasının görünür olup olmadığı |
| ignoreError | boolean | Bu seçenek geçerli değilse hatayı görmezden gelip gelmeyeceği. |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Yüzde olarak ölçekleme faktörünü temsil eder. 10 ile 400 arasında olmalıdır.

**Remarks**

Lütfen önce görünüm tipini ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### split() {#split--}
```
public void split()
```


Pencereyi böler.

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Bu çalışma sayfasındaki verilere erişmek için önbellekleri kullanan oturumu başlatır.

**Remarks**

Veriye erişim tamamlandıktan sonra, tüm önbellekleri temizlemek ve normal erişim modunu geri kazanmak için aynı seçeneklerle [closeAccessCache(int)](../../com.aspose.cells/worksheet\#closeAccessCache-int-) çağrılmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). veri erişim seçenekleri |

### toString() {#toString--}
```
public String toString()
```


Geçerli Worksheet nesnesini temsil eden bir dize döndürür.

**Returns:**
java.lang.String -
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Çalışma sayfasındaki bölmeleri dondurmayı kaldırır.

### unprotect() {#unprotect--}
```
public void unprotect()
```


Çalışma sayfasının korumasını kaldırır.

**Remarks**

Bu yöntem, şifresiz korunan çalışma sayfasının korumasını kaldırır.

### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Çalışma sayfasının korumasını kaldırır.

**Remarks**

Çalışma sayfası şifre olmadan korunduysa, şifre parametresine null değer veya boş dize atayabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| password | java.lang.String | Parola |

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

### xmlMapQuery(String path, XmlMap xmlMap) {#xmlMapQuery-java.lang.String-com.aspose.cells.XmlMap-}
```
public ArrayList xmlMapQuery(String path, XmlMap xmlMap)
```


XML haritasının belirli yoluna eşlenen/bağlanan hücre alanlarını sorgular.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Worksheet.GetAreasOfXmlMapQuery() yöntemini kullanın. Bu özellik, Ağustos 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | java.lang.String | xml öğe yolu |
| xmlMap | [XmlMap](../../com.aspose.cells/xmlmap) | Belirli bir harita içinde belirli bir yolu sorgulamak istiyorsanız bir xml haritası belirtin |

**Returns:**
java.util.ArrayList - [CellArea](../../com.aspose.cells/cellarea) listesi, xml haritasının belirli yoluna eşlenen/bağlanan öğeleri içerir; hiçbir şey eşlenmez/bağlanmazsa boş bir liste döndürülür.
