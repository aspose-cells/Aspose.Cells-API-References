---
title: "PivotField"
second_title: "Aspose.Cells for Java API Referansı"
description: "PivotTable raporunda bir alanı temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotfield/
---

**Inheritance:**
java.lang.Object
```
public class PivotField
```

PivotTable raporunda bir alanı temsil eder.

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
 
          pivot.calculateData(new PivotTableCalculateOption());
 
         //do your business
 
         book.save("out.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addCalculatedItem(String name, String formula)](#addCalculatedItem-java.lang.String-java.lang.String-) | Pivot alanına hesaplanmış bir formül öğesi ekle. |
| [clearFilter()](#clearFilter--) | Bu pivot alanındaki filtre ayarını temizler. |
| [dispose()](#dispose--) | Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterByDate(int type, DateTime dateTime1, DateTime dateTime2)](#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Satır veya sütun pivot alanının tarih değerlerine göre filtreler. |
| [filterByLabel(int type, String label1, String label2)](#filterByLabel-int-java.lang.String-java.lang.String-) | Satır veya sütun pivot alanının başlıklarına göre filtreler. |
| [filterByValue(int valueFieldIndex, int type, double value1, double value2)](#filterByValue-int-int-double-double-) | Veri pivot alanının değerlerine göre filtreler. |
| [filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)](#filterTop10-int-int-boolean-int-) | Veri pivot alanının değerlerine göre filtreler. |
| [getAllowDraggingToColumn()](#getAllowDraggingToColumn--) | Belirtilen alanın sütun bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [getAllowDraggingToData()](#getAllowDraggingToData--) | Belirtilen alanın değerler bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [getAllowDraggingToPage()](#getAllowDraggingToPage--) | Belirtilen alanın sayfa bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [getAllowDraggingToRow()](#getAllowDraggingToRow--) | Belirtilen alanın satır bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [getAllowRemovingFromView()](#getAllowRemovingFromView--) | Bu pivot alanının PivotTable görünümünden kaldırılıp kaldırılamayacağını gösterir. |
| [getAutoShowCount()](#getAutoShowCount--) | Belirtilen PivotTable alanında otomatik olarak gösterilen üst veya alt öğe sayısını temsil eder. |
| [getAutoShowField()](#getAutoShowField--) | Otomatik gösterim alanı dizinini temsil eder. -1, PivotField kendisini ifade eder. |
| [getAutoSortField()](#getAutoSortField--) | Otomatik sıralanan alanın dizinini temsil eder. |
| [getBaseIndex()](#getBaseIndex--) | Kaynak pivot alanlarındaki dizini temsil eder. |
| [getCalculatedFieldFormula()](#getCalculatedFieldFormula--) | Belirtilen hesaplanmış alanın formül dizesini al. |
| [getClass()](#getClass--) |  |
| [getCurrentPageItem()](#getCurrentPageItem--) | Bu pivot alanı için şu anda görüntülenen sayfa öğesini alır (yalnızca sayfa alanı). |
| [getCurrentPageItemText()](#getCurrentPageItemText--) | Bu pivot alanı için geçerli sayfa öğesinin görüntü metnini alır (yalnızca sayfa alanı). |
| [getDisplayName()](#getDisplayName--) | Pivot tablo görünümünde pivot alanının görüntü adını temsil eder. |
| [getDragToColumn()](#getDragToColumn--) | Belirtilen alanın sütun bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [getDragToData()](#getDragToData--) | Belirtilen alanın değerler bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [getDragToHide()](#getDragToHide--) | Bu pivot alanının PivotTable görünümünden kaldırılıp kaldırılamayacağını gösterir. |
| [getDragToPage()](#getDragToPage--) | Belirtilen alanın sayfa bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [getDragToRow()](#getDragToRow--) | Belirtilen alanın satır bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [getFilters()](#getFilters--) | Bu pivot alanına uygulanan tüm pivot filtrelerini alır. |
| [getFormula()](#getFormula--) | Hesaplanmış alanın formülünü alır. |
| [getFunction()](#getFunction--) | Bu PivotTable veri alanını özetlemek için kullanılan işlevi temsil eder. |
| [getGroupSettings()](#getGroupSettings--) | Pivot alanının grup ayarlarını alır. |
| [getInsertBlankRow()](#getInsertBlankRow--) | Her öğeden sonra boş bir satır eklenip eklenmeyeceğini gösterir. |
| [getItemCount()](#getItemCount--) | Bu pivot alanındaki temel öğelerin sayısını alır. |
| [getItems()](#getItems--) | Bu alandaki pivot öğelerinin tüm etiketlerini al. |
| [getMaxValue()](#getMaxValue--) | Bu alanın maksimum değerini alır. |
| [getMinValue()](#getMinValue--) | Bu alanın maksimum değerini alır. |
| [getName()](#getName--) | PivotField adını temsil eder. |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--) | Bu pivot alanına uygulanacak sıralama işleminin otomatik sıralama mı yoksa basit veri sıralaması mı olduğunu gösterir. |
| [getNumber()](#getNumber--) | Sayıların ve tarihlerin yerleşik görüntü biçimini temsil eder. |
| [getNumberFormat()](#getNumberFormat--) | Sayıların ve tarihlerin özel görüntü biçimini temsil eder. |
| [getOriginalItems()](#getOriginalItems--) | Orijinal temel öğeleri al; |
| [getPivotFilterByType(int type)](#getPivotFilterByType-int-) | Pivot alanının tipine göre pivot filtresini alır |
| [getPivotFilters()](#getPivotFilters--) | Pivot alanının pivot filtrelerini alır |
| [getPivotItems()](#getPivotItems--) | Pivot alanının pivot öğelerini alır |
| [getPosition()](#getPosition--) | Bölgede [PivotField](../../com.aspose.cells/pivotfield) indeksini temsil eder. |
| [getRegionType()](#getRegionType--) | Bu alanın görüntülendiği pivot tablonun bölgesini belirtir. |
| [getShowAllItems()](#getShowAllItems--) | Özet veri içermeseler bile PivotTable görünümünde tüm öğelerin gösterilip gösterilmeyeceğini belirtir. |
| [getShowCompact()](#getShowCompact--) | Pivot Tablo görünümünde aynı sütunda bir sonraki alanın etiketlerinin gösterilip gösterilmeyeceğini belirtir. |
| [getShowInCompactForm()](#getShowInCompactForm--) | Bu satır alanının sıkışık form düzeni kullanıp kullanmadığını gösteren bir değeri alır. |
| [getShowInOutlineForm()](#getShowInOutlineForm--) | Bu satır alanının anahat düzeni kullanıp kullanmadığını gösteren bir değeri alır. |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--) | Alt toplamların öğelerin üstünde mi yoksa altında mı gösterileceğini belirtir. |
| [getShowValuesSetting()](#getShowValuesSetting--) | ShowDataAs hesaplaması kullanıldığında değerlerin gösterilme ayarlarını alır. |
| [getSortSetting()](#getSortSetting--) | Otomatik sıralamanın tüm ayarlarını alır |
| [getSubtotals()](#getSubtotals--) | Alanının alt toplamlarını alır. |
| [getSubtotals(int subtotalType)](#getSubtotals-int-) | Bu pivot alanı için belirtilen alt toplamın gösterilip gösterilmeyeceğini belirtir. |
| [getTop10AutoShowSettings()](#getTop10AutoShowSettings--) | Bir pivot alanı için İlk 10 Otomatik Göster ayarlarını alır. |
| [group()](#group--) | Alanı otomatik olarak grupla. |
| [group(PivotFieldGroupOptions options)](#group-com.aspose.cells.PivotFieldGroupOptions-) | Pivot alanını seçeneklerle gruplar. |
| [groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-) | Dosyayı tarih grup türlerine göre grupla. |
| [groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)](#groupBy-boolean-double-boolean-double-double-boolean-) | Dosyayı sayıya göre grupla. |
| [groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-) | Alanı özel olarak grupla. |
| [groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)](#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-) | Dosyayı tarih grup türlerine göre grupla. |
| [groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)](#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-) | Alanı özel olarak grupla. |
| [groupBy(double interval, boolean newField)](#groupBy-double-boolean-) | Alanı aralıkla otomatik olarak grupla. |
| [groupBy(double start, double end, double interval, boolean newField)](#groupBy-double-double-double-boolean-) | Dosyayı sayıya göre grupla. |
| [groupBy(int[] groups, double interval, boolean newField)](#groupBy-int---double-boolean-) | Alanı içsel olarak otomatik grupla. |
| [hashCode()](#hashCode--) |  |
| [hideAllDetails()](#hideAllDetails--) | Her pivot öğesinin tüm ayrıntılarını gizler. |
| [hideDetail(boolean isHiddenDetail)](#hideDetail-boolean-) | Bir pivot alanındaki tüm PivotItem'ların ayrıntılarının gizlenip gizlenmeyeceğini ayarlar. |
| [hideItem(int index, boolean isHidden)](#hideItem-int-boolean-) | Veri alanındaki belirli PivotItem'ın gizlenip gizlenmeyeceğini ayarlar. |
| [hideItem(String itemValue, boolean isHidden)](#hideItem-java.lang.String-boolean-) | Veri alanındaki belirli PivotItem'ın gizlenip gizlenmeyeceğini ayarlar. |
| [hideItemDetail(int index, boolean isHiddenDetail)](#hideItemDetail-int-boolean-) | Pivot alanındaki belirli PivotItem'ın gizli ayrıntısını ayarlar. |
| [initPivotItems()](#initPivotItems--) | Pivot alanının pivot öğelerini başlat. |
| [isAscendShow()](#isAscendShow--) | Belirtilen PivotTable alanının artan şekilde otomatik gösterilip gösterilmediğini gösterir. |
| [isAscendSort()](#isAscendSort--) | Bu pivot alanının öğelerinin artan şekilde otomatik sıralanıp sıralanmadığını belirtir. |
| [isAutoShow()](#isAutoShow--) | Belirtilen PivotTable alanının otomatik olarak gösterilip gösterilmediğini belirtir. |
| [isAutoSort()](#isAutoSort--) | Bu PivotTable alanının öğelerinin otomatik olarak sıralanıp sıralanmadığını belirtir. |
| [isAutoSubtotals()](#isAutoSubtotals--) | Belirtilen alanın otomatik alt toplamları gösterip göstermediğini belirtir. |
| [isCalculatedField()](#isCalculatedField--) | Bu pivot alanının hesaplanmış bir alan olup olmadığını belirtir. |
| [isHiddenItem(int index)](#isHiddenItem-int-) | Belirli PivotItem'ın gizli olup olmadığını belirtir. |
| [isHiddenItemDetail(int index)](#isHiddenItemDetail-int-) | Belirli PivotItem'ın ayrıntısını gizleyip gizlemeyeceğini belirtir.. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--) | Manuel filtrede alana yeni öğelerin dahil edilip edilmeyeceğini belirtir. |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--) | Her öğeden sonra sayfa sonu eklenip eklenmeyeceğini gösterir. |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--) | Sayfa alanında birden çok öğenin seçilip seçilemeyeceğini gösterir. |
| [isRepeatItemLabels()](#isRepeatItemLabels--) | Alan etiketlerinin satır veya sütun bölgesinde tekrarlanıp tekrarlanmayacağını gösterir. |
| [isValueFields()](#isValueFields--) | Bu alanın değer alanlarını temsil edip etmediğini gösterir. |
| [isValuesField()](#isValuesField--) | Bu alanın değer alanını temsil edip etmediğini gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDraggingToColumn(boolean value)](#setAllowDraggingToColumn-boolean-) | Belirtilen alanın sütun bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [setAllowDraggingToData(boolean value)](#setAllowDraggingToData-boolean-) | Belirtilen alanın değerler bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [setAllowDraggingToPage(boolean value)](#setAllowDraggingToPage-boolean-) | Belirtilen alanın sayfa bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [setAllowDraggingToRow(boolean value)](#setAllowDraggingToRow-boolean-) | Belirtilen alanın satır bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [setAllowRemovingFromView(boolean value)](#setAllowRemovingFromView-boolean-) | Bu pivot alanının PivotTable görünümünden kaldırılıp kaldırılamayacağını gösterir. |
| [setAscendShow(boolean value)](#setAscendShow-boolean-) | Belirtilen PivotTable alanının artan şekilde otomatik gösterilip gösterilmediğini gösterir. |
| [setAscendSort(boolean value)](#setAscendSort-boolean-) | Bu pivot alanının öğelerinin artan şekilde otomatik sıralanıp sıralanmadığını belirtir. |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Belirtilen PivotTable alanının otomatik olarak gösterilip gösterilmediğini belirtir. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Belirtilen PivotTable alanında otomatik olarak gösterilen üst veya alt öğe sayısını temsil eder. |
| [setAutoShowField(int value)](#setAutoShowField-int-) | Otomatik gösterim alanı dizinini temsil eder. -1, PivotField kendisini ifade eder. |
| [setAutoSort(boolean value)](#setAutoSort-boolean-) | Bu PivotTable alanının öğelerinin otomatik olarak sıralanıp sıralanmadığını belirtir. |
| [setAutoSortField(int value)](#setAutoSortField-int-) | Otomatik sıralanan alanın dizinini temsil eder. |
| [setAutoSubtotals(boolean value)](#setAutoSubtotals-boolean-) | Belirtilen alanın otomatik alt toplamları gösterip göstermediğini belirtir. |
| [setBaseIndex(int value)](#setBaseIndex-int-) | Kaynak pivot alanlarındaki dizini temsil eder. |
| [setCurrentPageItem(short value)](#setCurrentPageItem-short-) | Bu pivot alanı için şu anda görüntülenen sayfa öğesini ayarlar (yalnızca sayfa alanı). |
| [setCurrentPageItemText(String value)](#setCurrentPageItemText-java.lang.String-) | Bu pivot alanı için geçerli sayfa öğesinin görüntü metnini alır (yalnızca sayfa alanı). |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Pivot tablo görünümünde pivot alanının görüntü adını temsil eder. |
| [setDragToColumn(boolean value)](#setDragToColumn-boolean-) | Belirtilen alanın sütun bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [setDragToData(boolean value)](#setDragToData-boolean-) | Belirtilen alanın değerler bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [setDragToHide(boolean value)](#setDragToHide-boolean-) | Bu pivot alanının PivotTable görünümünden kaldırılıp kaldırılamayacağını gösterir. |
| [setDragToPage(boolean value)](#setDragToPage-boolean-) | Belirtilen alanın sayfa bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [setDragToRow(boolean value)](#setDragToRow-boolean-) | Belirtilen alanın satır bölgesine sürüklenip sürüklenemeyeceğini gösterir. |
| [setFunction(int value)](#setFunction-int-) | Bu PivotTable veri alanını özetlemek için kullanılan işlevi temsil eder. |
| [setIncludeNewItemsInFilter(boolean value)](#setIncludeNewItemsInFilter-boolean-) | Manuel filtrede alana yeni öğelerin dahil edilip edilmeyeceğini belirtir. |
| [setInsertBlankRow(boolean value)](#setInsertBlankRow-boolean-) | Her öğeden sonra boş bir satır eklenip eklenmeyeceğini gösterir. |
| [setInsertPageBreaksBetweenItems(boolean value)](#setInsertPageBreaksBetweenItems-boolean-) | Her öğeden sonra sayfa sonu eklenip eklenmeyeceğini gösterir. |
| [setMultipleItemSelectionAllowed(boolean value)](#setMultipleItemSelectionAllowed-boolean-) | Sayfa alanında birden çok öğenin seçilip seçilemeyeceğini gösterir. |
| [setName(String value)](#setName-java.lang.String-) | PivotField adını temsil eder. |
| [setNonAutoSortDefault(boolean value)](#setNonAutoSortDefault-boolean-) | Bu pivot alanına uygulanacak sıralama işleminin otomatik sıralama mı yoksa basit veri sıralaması mı olduğunu gösterir. |
| [setNumber(int value)](#setNumber-int-) | Sayıların ve tarihlerin yerleşik görüntü biçimini temsil eder. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Sayıların ve tarihlerin özel görüntü biçimini temsil eder. |
| [setRepeatItemLabels(boolean value)](#setRepeatItemLabels-boolean-) | Alan etiketlerinin satır veya sütun bölgesinde tekrarlanıp tekrarlanmayacağını gösterir. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Özet veri içermeseler bile PivotTable görünümünde tüm öğelerin gösterilip gösterilmeyeceğini belirtir. |
| [setShowCompact(boolean value)](#setShowCompact-boolean-) | Pivot Tablo görünümünde aynı sütunda bir sonraki alanın etiketlerinin gösterilip gösterilmeyeceğini belirtir. |
| [setShowInCompactForm(boolean value)](#setShowInCompactForm-boolean-) | Bu satır alanının sıkışık form düzeni kullanıp kullanmadığını gösteren bir değeri ayarlar. |
| [setShowInOutlineForm(boolean value)](#setShowInOutlineForm-boolean-) | Bu satır alanının anahat düzeni kullanıp kullanmadığını gösteren bir değeri ayarlar. |
| [setShowSubtotalAtTop(boolean value)](#setShowSubtotalAtTop-boolean-) | Alt toplamların öğelerin üstünde mi yoksa altında mı gösterileceğini belirtir. |
| [setSubtotals(int value)](#setSubtotals-int-) | Alan için alt toplamları ayarlar. |
| [setSubtotals(int subtotalType, boolean shown)](#setSubtotals-int-boolean-) | Belirtilen alanın nasıl alt toplamlandırılacağını ayarlar. |
| [showAllDetails()](#showAllDetails--) | Her pivot öğesinin tüm ayrıntılarını göster. |
| [showValuesAs(int showValuesAsType, int baseField, int baseItem)](#showValuesAs-int-int-int-) | Sets the \"Show Values As\" calculation for this pivot field. |
| [showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)](#showValuesAs-int-int-int-int-) | ShowDataAs hesabı kullanıldığında veri alanının değerlerini farklı bir görüntü biçiminde gösterir. |
| [showValuesAs(int showValuesAsType, String baseField, String baseItem)](#showValuesAs-int-java.lang.String-java.lang.String-) | "Değerleri Şöyle Göster" hesabını bu veri alanı için yapılandırır. |
| [sortBy(int sortType)](#sortBy-int-) | Bu pivot alanını sıralar. |
| [sortBy(int sortType, int fieldSortedBy)](#sortBy-int-int-) | Bu pivot alanını sıralar. |
| [sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)](#sortBy-int-int-int-java.lang.String-) | Bu pivot alanını sıralar. |
| [sortBy(int sortType, int fieldSortedBy, String cellName)](#sortBy-int-int-java.lang.String-) | Bu pivot alanını sıralar. |
| [toString()](#toString--) |  |
| [top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)](#top10AutoShow-boolean-boolean-int-int-) | Bu pivot alanı için Top10 Otomatik Göster ayarlarını yapılandırır. |
| [ungroup()](#ungroup--) | Pivot alanının grubunu kaldır. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCalculatedItem(String name, String formula) {#addCalculatedItem-java.lang.String-java.lang.String-}
```
public void addCalculatedItem(String name, String formula)
```


Pivot alanına hesaplanmış bir formül öğesi ekle.

**Remarks**

Yalnızca Satır/Sütun alanına hesaplanmış öğe eklemeyi destekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Öğenin adı. |
| formula | java.lang.String | Pivot öğesinin formülü. |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Bu pivot alanındaki filtre ayarını temizler.

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
### filterByDate(int type, DateTime dateTime1, DateTime dateTime2) {#filterByDate-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter filterByDate(int type, DateTime dateTime1, DateTime dateTime2)
```


Satır veya sütun pivot alanının tarih değerlerine göre filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Veri filtreleme türü. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | Filtre koşulunun tarih etiketi |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | Aralık filtre koşulunun üst sınır tarih etiketi |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByLabel(int type, String label1, String label2) {#filterByLabel-int-java.lang.String-java.lang.String-}
```
public PivotFilter filterByLabel(int type, String label1, String label2)
```


Satır veya sütun pivot alanının başlıklarına göre filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Veri filtreleme türü. |
| label1 | java.lang.String | Filtre koşulunun etiketi |
| label2 | java.lang.String | Arasındaki filtre koşulunun üst sınır etiketi |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterByValue(int valueFieldIndex, int type, double value1, double value2) {#filterByValue-int-int-double-double-}
```
public PivotFilter filterByValue(int valueFieldIndex, int type, double value1, double value2)
```


Veri pivot alanının değerlerine göre filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| valueFieldIndex | int | Değer bölgesindeki değer alanının indeksi. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Veri filtreleme türü. |
| value1 | double | Filtre koşulunun değeri |
| value2 | double | Arasındaki filtre koşulunun üst sınır değeri |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount) {#filterTop10-int-int-boolean-int-}
```
public PivotFilter filterTop10(int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Veri pivot alanının değerlerine göre filtreler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| valueFieldIndex | int | Veri bölgesindeki veri alanının indeksi. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Veri filtreleme türü. Yalnızca Count, Sum ve Percent olabilir. |
| isTop | boolean | Filtrenin üstten mi alttan mı olduğunu gösterir |
| itemCount | int | Öğe sayısı |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getAllowDraggingToColumn() {#getAllowDraggingToColumn--}
```
public boolean getAllowDraggingToColumn()
```


Belirtilen alanın sütun bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Returns:**
boolean
### getAllowDraggingToData() {#getAllowDraggingToData--}
```
public boolean getAllowDraggingToData()
```


Belirtilen alanın değerler bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Returns:**
boolean
### getAllowDraggingToPage() {#getAllowDraggingToPage--}
```
public boolean getAllowDraggingToPage()
```


Belirtilen alanın sayfa bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Returns:**
boolean
### getAllowDraggingToRow() {#getAllowDraggingToRow--}
```
public boolean getAllowDraggingToRow()
```


Belirtilen alanın satır bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Returns:**
boolean
### getAllowRemovingFromView() {#getAllowRemovingFromView--}
```
public boolean getAllowRemovingFromView()
```


Bu pivot alanının PivotTable görünümünden kaldırılıp kaldırılamayacağını gösterir. Varsayılan değer doğrudur.

**Returns:**
boolean
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Belirtilen PivotTable alanında otomatik olarak gösterilen üst veya alt öğe sayısını temsil eder.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.Top10AutoShowSettings.AutoShowCount özelliğini veya PivotField.Top10AutoShow() yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getAutoShowField() {#getAutoShowField--}
```
public int getAutoShowField()
```


Otomatik gösterim alanı indeksini temsil eder. -1, PivotField kendisini ifade eder. Veri alanlarının indeksi olmalıdır.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.Top10AutoShowSettings.RankBy özelliğini veya PivotField.Top10AutoShow() yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getAutoSortField() {#getAutoSortField--}
```
public int getAutoSortField()
```


Otomatik sıralanan alanın indeksini temsil eder. -1, PivotField kendisini ifade eder, diğerleri veri alanlarının konumunu gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.SortSetting.SortBy özelliğini veya PivotField.SortBy() yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getBaseIndex() {#getBaseIndex--}
```
public int getBaseIndex()
```


Kaynak pivot alanlarındaki dizini temsil eder.

**Remarks**

NOT: Bu özelliğin ayarlayıcısı artık kullanımdan kaldırıldı. Bu ayarlayıcı, Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getCalculatedFieldFormula() {#getCalculatedFieldFormula--}
```
public String getCalculatedFieldFormula()
```


Belirtilen hesaplanmış alanın formül dizesini al.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.GetFormula() yöntemini kullanın. Bu yöntem, Ağustos 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentPageItem() {#getCurrentPageItem--}
```
public short getCurrentPageItem()
```


Bu pivot alanı için şu anda görüntülenen sayfa öğesini alır (yalnızca sayfa alanı).

**Remarks**

\"Select All\" göstermek için sentinel değer olarak [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) kullanın. Bu önceden tanımlanmış bir işaretçidir ve geçerli bir öğe indeksi değildir.

**Returns:**
short
### getCurrentPageItemText() {#getCurrentPageItemText--}
```
public String getCurrentPageItemText()
```


Bu pivot alanı için geçerli sayfa öğesinin görüntü metnini alır (yalnızca sayfa alanı).

**Remarks**

\"(All)\" döndürür, [getCurrentPageItem()](../../com.aspose.cells/pivotfield\\#getCurrentPageItem--) [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) eşit olduğunda. Diğer değerler için, öğe indeksinin dize temsili döndürülür.

**Returns:**
java.lang.String
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Pivot tablo görünümünde pivot alanının görüntü adını temsil eder.

**Returns:**
java.lang.String
### getDragToColumn() {#getDragToColumn--}
```
public boolean getDragToColumn()
```


Belirtilen alanın sütun bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.AllowDraggingToColumn özelliğini kullanın. Bu yöntem, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getDragToData() {#getDragToData--}
```
public boolean getDragToData()
```


Belirtilen alanın değerler bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.AllowDraggingToData özelliğini kullanın. Bu yöntem, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getDragToHide() {#getDragToHide--}
```
public boolean getDragToHide()
```


Bu pivot alanının PivotTable görünümünden kaldırılıp kaldırılamayacağını gösterir. Varsayılan değer doğrudur.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.AllowRemovingFromView özelliğini kullanın. Bu yöntem, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getDragToPage() {#getDragToPage--}
```
public boolean getDragToPage()
```


Belirtilen alanın sayfa bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.AllowDraggingToPage özelliğini kullanın. Bu yöntem, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getDragToRow() {#getDragToRow--}
```
public boolean getDragToRow()
```


Belirtilen alanın satır bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.AllowDraggingToRow özelliğini kullanın. Bu yöntem, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getFilters() {#getFilters--}
```
public PivotFilter[] getFilters()
```


Bu pivot alanına uygulanan tüm pivot filtrelerini alır.

**Returns:**
com.aspose.cells.PivotFilter[]
### getFormula() {#getFormula--}
```
public String getFormula()
```


Hesaplanmış alanın formülünü alır. Yalnızca hesaplanmış alan için çalışır.

**Returns:**
java.lang.String
### getFunction() {#getFunction--}
```
public int getFunction()
```


Bu PivotTable veri alanını özetlemek için kullanılan işlevi temsil eder.

Bakınız [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Returns:**
int
### getGroupSettings() {#getGroupSettings--}
```
public PivotFieldGroupSettings getGroupSettings()
```


Pivot alanının grup ayarlarını alır.

**Remarks**

Bu alan gruplanmamışsa, Null döndürülecektir.

**Returns:**
[PivotFieldGroupSettings](../../com.aspose.cells/pivotfieldgroupsettings)
### getInsertBlankRow() {#getInsertBlankRow--}
```
public boolean getInsertBlankRow()
```


Her öğeden sonra boş bir satır eklenip eklenmeyeceğini belirtir. Yalnızca satır alanları için.

**Returns:**
boolean
### getItemCount() {#getItemCount--}
```
public int getItemCount()
```


Bu pivot alanındaki temel öğelerin sayısını alır.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.PivotItems.Count özelliğini kullanın. Bu yöntem, Ağustos 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getItems() {#getItems--}
```
public String[] getItems()
```


Bu alandaki pivot öğelerinin tüm etiketlerini al.

**Returns:**
java.lang.String[]
### getMaxValue() {#getMaxValue--}
```
public CellValue getMaxValue()
```


Bu alanın maksimum değerini alır.

**Remarks**

Yalnızca değeri tarih saat, sayı veya boş olabilecek satır veya sütun alanları için çalışır.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getMinValue() {#getMinValue--}
```
public CellValue getMinValue()
```


Bu alanın maksimum değerini alır.

**Remarks**

Yalnızca değeri tarih saat, sayı veya boş olabilecek satır veya sütun alanları için çalışır.

**Returns:**
[CellValue](../../com.aspose.cells/cellvalue) - 
### getName() {#getName--}
```
public String getName()
```


PivotField adını temsil eder.

**Returns:**
java.lang.String
### getNonAutoSortDefault() {#getNonAutoSortDefault--}
```
public boolean getNonAutoSortDefault()
```


Bu pivot alanına uygulanacak sıralama işleminin otomatik sıralama mı yoksa basit veri sıralaması mı olduğunu gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen !PivotField.SortSetting.IsSimpleSort özelliğini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getNumber() {#getNumber--}
```
public int getNumber()
```


Sayıların ve tarihlerin yerleşik görüntü biçimini temsil eder.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Sayıların ve tarihlerin özel görüntü biçimini temsil eder.

**Returns:**
java.lang.String
### getOriginalItems() {#getOriginalItems--}
```
public String[] getOriginalItems()
```


Orijinal temel öğeleri al;

**Returns:**
java.lang.String[]
### getPivotFilterByType(int type) {#getPivotFilterByType-int-}
```
public PivotFilter getPivotFilterByType(int type)
```


Pivot alanının tipine göre pivot filtresini alır

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tip | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### getPivotFilters() {#getPivotFilters--}
```
public ArrayList getPivotFilters()
```


Pivot alanının pivot filtrelerini alır

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.GetFilters() yöntemini kullanın. Bu yöntem Kasım 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.util.ArrayList
### getPivotItems() {#getPivotItems--}
```
public PivotItemCollection getPivotItems()
```


Pivot alanının pivot öğelerini alır

**Returns:**
[PivotItemCollection](../../com.aspose.cells/pivotitemcollection)
### getPosition() {#getPosition--}
```
public int getPosition()
```


Bölgede [PivotField](../../com.aspose.cells/pivotfield) indeksini temsil eder.

**Returns:**
int
### getRegionType() {#getRegionType--}
```
public int getRegionType()
```


Bu alanın görüntülendiği pivot tablonun bölgesini belirtir.

Bkz. [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


PivotTable görünümünde özet veri içermeseler bile tüm öğelerin gösterilip gösterilmeyeceğini belirtir. Varsayılan değer false'tur.

**Returns:**
boolean
### getShowCompact() {#getShowCompact--}
```
public boolean getShowCompact()
```


Pivot Table görünümünde aynı sütunda bir sonraki alanın etiketlerinin gösterilip gösterilmeyeceğini belirtir. Yalnızca satır alanları için.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.ShowInCompactForm özelliğini kullanın. Bu yöntem Kasım 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getShowInCompactForm() {#getShowInCompactForm--}
```
public boolean getShowInCompactForm()
```


Bu satır alanının kompakt form düzeni kullanıp kullanmadığını gösteren bir değer alır. Yalnızca satır alanları için geçerlidir.

**Remarks**

Kompakt form, taslak düzenin bir alt modudur. Bu ayar yalnızca [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) true olduğunda etkili olur.

**Returns:**
boolean
### getShowInOutlineForm() {#getShowInOutlineForm--}
```
public boolean getShowInOutlineForm()
```


Bu satır alanının taslak düzeni kullanıp kullanmadığını gösteren bir değer alır. Yalnızca satır alanları için geçerlidir.

**Returns:**
boolean
### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}
```
public boolean getShowSubtotalAtTop()
```


Alt toplamların öğelerin üstünde mi yoksa altında mı gösterileceğini belirtir.

**Remarks**

ShowInOutlineForm true olduğunda yalnızca satır bölgesindeki pivot alanları için çalışır.

**Returns:**
boolean
### getShowValuesSetting() {#getShowValuesSetting--}
```
public PivotShowValuesSetting getShowValuesSetting()
```


ShowDataAs hesaplaması kullanıldığında değerlerin gösterilme ayarlarını alır.

**Returns:**
[PivotShowValuesSetting](../../com.aspose.cells/pivotshowvaluessetting)
### getSortSetting() {#getSortSetting--}
```
public PivotFieldSortSetting getSortSetting()
```


Otomatik sıralamanın tüm ayarlarını alır

**Returns:**
[PivotFieldSortSetting](../../com.aspose.cells/pivotfieldsortsetting)
### getSubtotals() {#getSubtotals--}
```
public int getSubtotals()
```


Alanının alt toplamlarını alır. Yalnızca Satır veya Sütun pivot alanı için.

[PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) adresine bakın.

**Example**

```
         //No subtotals
         rowField.setSubtotals(PivotFieldSubtotalType.NONE);
         //Automatic subtotals
         //rowField.Subtotals = PivotFieldSubtotalType.Automatic;
         //Single subtotals: Sum
         //rowField.Subtotals = PivotFieldSubtotalType.Sum;
         //Multipl subtotals: Sum and count numbers 
         //rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

**Returns:**
int
### getSubtotals(int subtotalType) {#getSubtotals-int-}
```
public boolean getSubtotals(int subtotalType)
```


Bu pivot alanı için belirtilen alt toplamın gösterilip gösterilmeyeceğini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Alt toplam türü. |

**Returns:**
boolean - Belirtilen alt toplamın gösterilip gösterilmediğini döndürür.
### getTop10AutoShowSettings() {#getTop10AutoShowSettings--}
```
public PivotFieldTop10AutoShowSettings getTop10AutoShowSettings()
```


Bir pivot alanı için İlk 10 Otomatik Göster ayarlarını alır.

**Returns:**
[PivotFieldTop10AutoShowSettings](../../com.aspose.cells/pivotfieldtop10autoshowsettings)
### group() {#group--}
```
public boolean group()
```


Alanı otomatik olarak grupla.

**Remarks**

Alan yalnızca boş ve tarih saat içeriyorsa, alan Aylar bazında gruplanır. Alan yalnızca boş ve sayı içeriyorsa, alan Sayı bazında gruplanır. Aksi takdirde herhangi bir grup olmadan sadece false döndürülür.

**Returns:**
boolean
### group(PivotFieldGroupOptions options) {#group-com.aspose.cells.PivotFieldGroupOptions-}
```
public boolean group(PivotFieldGroupOptions options)
```


Pivot alanını seçeneklerle gruplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [PivotFieldGroupOptions](../../com.aspose.cells/pivotfieldgroupoptions) | Pivot alanı gruplama ayarları için seçenekler. |

**Returns:**
boolean -
### groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-boolean-com.aspose.cells.DateTime-boolean-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(boolean isAutoStart, DateTime start, boolean isAutoEnd, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Dosyayı tarih grup türlerine göre grupla.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.Group(PivotFieldGroupOptions) yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isAutoStart | boolean | Başlangıç tarih saat değerinin otomatik olarak algılanıp algılanmayacağını belirtir. |
| start | [DateTime](../../com.aspose.cells/datetime) | Başlangıç tarih saatı |
| isAutoEnd | boolean | Bitiş tarih saat değerinin otomatik olarak algılanıp algılanmayacağını belirtir. |
| end | [DateTime](../../com.aspose.cells/datetime) | Bitiş tarih saatı |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Grup türleri |
| aralık | double | Aralık |
| firstAsNewField | boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini belirtir. Yalnızca ilk grup öğesi için. |

**Returns:**
boolean - False, bu alanın tarih saatine göre gruplanamadığını gösterir.
### groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField) {#groupBy-boolean-double-boolean-double-double-boolean-}
```
public boolean groupBy(boolean isAutoStart, double start, boolean isAutoEnd, double end, double interval, boolean newField)
```


Dosyayı sayıya göre grupla.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.Group(PivotFieldGroupOptions) yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isAutoStart | boolean | Başlangıç değerinin otomatik olarak algılanıp algılanmayacağını gösterir. |
| başlangıç | double | Başlangıç değeri |
| isAutoEnd | boolean | Bitiş değerinin otomatik olarak algılanıp algılanmayacağını gösterir. |
| bitiş | double | Değerin sonu |
| aralık | double | Aralık |
| yeniAlan | boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini gösterir |

**Returns:**
boolean - False, bu alanın tarih saatine göre gruplanamadığını gösterir.
### groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.CustomPiovtFieldGroupItem---boolean-}
```
public boolean groupBy(CustomPiovtFieldGroupItem[] customGroupItems, boolean newField)
```


Alanı özel olarak grupla.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotField.Group(PivotFieldGroupOptions options) yöntemini PivotFieldGroupOptions.DiscreteGroupItems özelliği ile kullanın. Bu yöntem Temmuz 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem\[\]](../../com.aspose.cells/custompiovtfieldgroupitem) | Özel grup öğeleri. |
| yeniAlan | boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini gösterir |

**Returns:**
boolean - False, bu alanın tarih saatine göre gruplanamadığını gösterir.
### groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField) {#groupBy-com.aspose.cells.DateTime-com.aspose.cells.DateTime-int---double-boolean-}
```
public boolean groupBy(DateTime start, DateTime end, int[] groups, double interval, boolean firstAsNewField)
```


Dosyayı tarih grup türlerine göre grupla.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.Group(PivotFieldGroupOptions) yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | Başlangıç tarih saatı |
| end | [DateTime](../../com.aspose.cells/datetime) | Bitiş tarih saatı |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Grup türleri |
| aralık | double | Aralık |
| firstAsNewField | boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini belirtir. Yalnızca ilk grup öğesi için. |

**Returns:**
boolean - False, bu alanın tarih saatine göre gruplanamadığını gösterir.
### groupBy(DiscreteGroupItem[] customGroupItems, boolean newField) {#groupBy-com.aspose.cells.DiscreteGroupItem---boolean-}
```
public boolean groupBy(DiscreteGroupItem[] customGroupItems, boolean newField)
```


Alanı özel olarak grupla.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotField.Group(PivotFieldGroupOptions options) yöntemini PivotFieldGroupOptions.DiscreteGroupItems özelliği ile kullanın. Bu yöntem Temmuz 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| customGroupItems | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) | Özel grup öğeleri. |
| yeniAlan | boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini gösterir |

**Returns:**
boolean -
### groupBy(double interval, boolean newField) {#groupBy-double-boolean-}
```
public void groupBy(double interval, boolean newField)
```


Alanı aralıkla otomatik olarak grupla.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.Group(PivotFieldGroupOptions) yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | double | Grubun içi. Değer sıfır ise otomatik değer atanır, |
| yeniAlan | boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini gösterir. Yalnızca DateTime grubu için. |

### groupBy(double start, double end, double interval, boolean newField) {#groupBy-double-double-double-boolean-}
```
public boolean groupBy(double start, double end, double interval, boolean newField)
```


Dosyayı sayıya göre grupla.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.Group(PivotFieldGroupOptions) yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | double | Başlangıç değeri |
| bitiş | double | Değerin sonu |
| aralık | double | Aralık |
| yeniAlan | boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini gösterir |

**Returns:**
boolean - False, bu alanın tarih saatine göre gruplanamadığını gösterir.
### groupBy(int[] groups, double interval, boolean newField) {#groupBy-int---double-boolean-}
```
public void groupBy(int[] groups, double interval, boolean newField)
```


Alanı içsel olarak otomatik grupla.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.Group(PivotFieldGroupOptions) yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| groups | int[] | [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype). Grup türleri |
| aralık | double | Grubun içi. Değer sıfır ise otomatik değer atanır, yalnızca Sayılar veya Günler ile gruplama için çalışır. |
| yeniAlan | boolean | Pivot tabloya yeni bir alan eklenip eklenmeyeceğini gösterir. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideAllDetails() {#hideAllDetails--}
```
public void hideAllDetails()
```


Her pivot öğesinin tüm ayrıntılarını gizler.

### hideDetail(boolean isHiddenDetail) {#hideDetail-boolean-}
```
public void hideDetail(boolean isHiddenDetail)
```


Bir pivot alanındaki tüm PivotItem'ların detayının gizli olup olmadığını ayarlar. Bu, alanı daraltıp genişletmek anlamına gelir.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotItemsCollection.HideAllDetails() ve UnhideAllDetails() yöntemlerini kullanın. Bu yöntem Kasım 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isHiddenDetail | boolean | Pivot alanının detayını gizleyip gizlemeyeceği. |

### hideItem(int index, boolean isHidden) {#hideItem-int-boolean-}
```
public void hideItem(int index, boolean isHidden)
```


Veri alanındaki belirli PivotItem'ın gizlenip gizlenmeyeceğini ayarlar.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotField.PivotItems[int].IsHidden özelliğini kullanın. Bu yöntem Ağustos 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | pivotField içindeki pivotItem'ın indeksi. |
| isHidden | boolean | belirli PivotItem'ın gizli olup olmadığı |

### hideItem(String itemValue, boolean isHidden) {#hideItem-java.lang.String-boolean-}
```
public void hideItem(String itemValue, boolean isHidden)
```


Veri alanındaki belirli PivotItem'ın gizlenip gizlenmeyeceğini ayarlar.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotField.PivotItems[string].IsHidden özelliğini kullanın. Bu yöntem Ağustos 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| itemValue | java.lang.String | pivotField içindeki pivotItem'ın adı. |
| isHidden | boolean | Belirli PivotItem'ın gizli olup olmadığı |

### hideItemDetail(int index, boolean isHiddenDetail) {#hideItemDetail-int-boolean-}
```
public void hideItemDetail(int index, boolean isHiddenDetail)
```


Pivot alanındaki belirli PivotItem'ın gizli ayrıntısını ayarlar.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotField.PivotItems[int].IsDetailHidden özelliğini kullanın. Bu yöntem Ağustos 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | pivotField içindeki pivotItem'ın indeksi. |
| isHiddenDetail | boolean | belirli PivotItem'ın gizli olup olmadığı |

### initPivotItems() {#initPivotItems--}
```
public void initPivotItems()
```


Pivot alanının pivot öğelerini başlat.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Lütfen bu yöntemin çağrısını tamamen kaldırın. Bu yöntem Ekim 2026'dan itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### isAscendShow() {#isAscendShow--}
```
public boolean isAscendShow()
```


Belirtilen PivotTable alanının artan şekilde otomatik gösterilip gösterilmediğini gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.Top10AutoShowSettings.IsTop özelliğini veya PivotField.Top10AutoShow() yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### isAscendSort() {#isAscendSort--}
```
public boolean isAscendSort()
```


Bu pivot alanının öğelerinin artan şekilde otomatik sıralanıp sıralanmadığını belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.SortSetting.SortType özelliğini veya PivotField.SortBy() yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Belirtilen PivotTable alanının otomatik olarak gösterilip gösterilmediğini belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.Top10AutoShowSettings.IsAutoShow özelliğini veya PivotField.Top10AutoShow() yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### isAutoSort() {#isAutoSort--}
```
public boolean isAutoSort()
```


Bu PivotTable alanının öğelerinin otomatik olarak sıralanıp sıralanmadığını belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.SortSetting.SortType özelliğini veya PivotField.SortBy() yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### isAutoSubtotals() {#isAutoSubtotals--}
```
public boolean isAutoSubtotals()
```


Belirtilen alanın otomatik alt toplamları gösterip göstermediğini belirtir. Varsayılan değer true'tir.

**Returns:**
boolean
### isCalculatedField() {#isCalculatedField--}
```
public boolean isCalculatedField()
```


Bu pivot alanının hesaplanmış bir alan olup olmadığını belirtir.

**Returns:**
boolean
### isHiddenItem(int index) {#isHiddenItem-int-}
```
public boolean isHiddenItem(int index)
```


Belirli PivotItem'ın gizli olup olmadığını belirtir.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotField.PivotItems[int].IsHidden özelliğini kullanın. Bu yöntem Ağustos 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | pivotField içindeki pivotItem'ın indeksi. |

**Returns:**
boolean - belirli PivotItem'ın gizli olup olmadığı
### isHiddenItemDetail(int index) {#isHiddenItemDetail-int-}
```
public boolean isHiddenItemDetail(int index)
```


Belirli PivotItem'ın ayrıntısını gizleyip gizlemeyeceğini belirtir..

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen PivotField.PivotItems[int].IsDetailHidden özelliğini kullanın. Bu yöntem Ağustos 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | pivotField içindeki pivotItem'ın indeksi. |

**Returns:**
boolean - belirli PivotItem'ın gizli detay olup olmadığı
### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}
```
public boolean isIncludeNewItemsInFilter()
```


Alana yeni öğelerin manuel filtreye dahil edilip edilmeyeceğini belirtir. Varsayılan değer false'tur.

**Returns:**
boolean
### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}
```
public boolean isInsertPageBreaksBetweenItems()
```


Her öğeden sonra sayfa sonu eklenip eklenmeyeceğini belirtir. Varsayılan değer false'tur.

**Returns:**
boolean
### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}
```
public boolean isMultipleItemSelectionAllowed()
```


Sayfa alanında birden fazla öğenin seçilip seçilemeyeceğini belirtir. Varsayılan değer false'tur.

**Remarks**

Yalnızca sayfa (filtre) alanları için.

**Returns:**
boolean
### isRepeatItemLabels() {#isRepeatItemLabels--}
```
public boolean isRepeatItemLabels()
```


Satır veya sütun bölgesinde alan etiketlerinin tekrarlanıp tekrarlanmayacağını belirtir. Varsayılan değer false'tur.

**Returns:**
boolean
### isValueFields() {#isValueFields--}
```
public boolean isValueFields()
```


Bu alanın değer alanlarını temsil edip etmediğini gösterir.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.IsValuesField özelliğini kullanın. Bu yöntem Kasım 2023'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### isValuesField() {#isValuesField--}
```
public boolean isValuesField()
```


Bu alanın değer alanını temsil edip etmediğini gösterir.

**Remarks**

Yalnızca pivot tablo görünümünde iki veya daha fazla veri alanı olduğunda çalışır.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllowDraggingToColumn(boolean value) {#setAllowDraggingToColumn-boolean-}
```
public void setAllowDraggingToColumn(boolean value)
```


Belirtilen alanın sütun bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowDraggingToData(boolean value) {#setAllowDraggingToData-boolean-}
```
public void setAllowDraggingToData(boolean value)
```


Belirtilen alanın değerler bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowDraggingToPage(boolean value) {#setAllowDraggingToPage-boolean-}
```
public void setAllowDraggingToPage(boolean value)
```


Belirtilen alanın sayfa bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowDraggingToRow(boolean value) {#setAllowDraggingToRow-boolean-}
```
public void setAllowDraggingToRow(boolean value)
```


Belirtilen alanın satır bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAllowRemovingFromView(boolean value) {#setAllowRemovingFromView-boolean-}
```
public void setAllowRemovingFromView(boolean value)
```


Bu pivot alanının PivotTable görünümünden kaldırılıp kaldırılamayacağını gösterir. Varsayılan değer doğrudur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAscendShow(boolean value) {#setAscendShow-boolean-}
```
public void setAscendShow(boolean value)
```


Belirtilen PivotTable alanının artan şekilde otomatik gösterilip gösterilmediğini gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.Top10AutoShowSettings.IsTop özelliğini veya PivotField.Top10AutoShow() yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAscendSort(boolean value) {#setAscendSort-boolean-}
```
public void setAscendSort(boolean value)
```


Bu pivot alanının öğelerinin artan şekilde otomatik sıralanıp sıralanmadığını belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.SortSetting.SortType özelliğini veya PivotField.SortBy() yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Belirtilen PivotTable alanının otomatik olarak gösterilip gösterilmediğini belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.Top10AutoShowSettings.IsAutoShow özelliğini veya PivotField.Top10AutoShow() yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Belirtilen PivotTable alanında otomatik olarak gösterilen üst veya alt öğe sayısını temsil eder.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.Top10AutoShowSettings.AutoShowCount özelliğini veya PivotField.Top10AutoShow() yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setAutoShowField(int value) {#setAutoShowField-int-}
```
public void setAutoShowField(int value)
```


Otomatik gösterim alanı indeksini temsil eder. -1, PivotField kendisini ifade eder. Veri alanlarının indeksi olmalıdır.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.Top10AutoShowSettings.RankBy özelliğini veya PivotField.Top10AutoShow() yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setAutoSort(boolean value) {#setAutoSort-boolean-}
```
public void setAutoSort(boolean value)
```


Bu PivotTable alanının öğelerinin otomatik olarak sıralanıp sıralanmadığını belirtir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.SortSetting.SortType özelliğini veya PivotField.SortBy() yöntemini kullanın. Bu yöntem Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoSortField(int value) {#setAutoSortField-int-}
```
public void setAutoSortField(int value)
```


Otomatik sıralanan alanın indeksini temsil eder. -1, PivotField kendisini ifade eder, diğerleri veri alanlarının konumunu gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.SortSetting.SortBy özelliğini veya PivotField.SortBy() yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setAutoSubtotals(boolean value) {#setAutoSubtotals-boolean-}
```
public void setAutoSubtotals(boolean value)
```


Belirtilen alanın otomatik alt toplamları gösterip göstermediğini belirtir. Varsayılan değer true'tir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBaseIndex(int value) {#setBaseIndex-int-}
```
public void setBaseIndex(int value)
```


Kaynak pivot alanlarındaki dizini temsil eder.

**Remarks**

NOT: Bu özelliğin ayarlayıcısı artık kullanımdan kaldırıldı. Bu ayarlayıcı, Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCurrentPageItem(short value) {#setCurrentPageItem-short-}
```
public void setCurrentPageItem(short value)
```


Bu pivot alanı için şu anda görüntülenen sayfa öğesini ayarlar (yalnızca sayfa alanı).

**Remarks**

\"Select All\" göstermek için sentinel değer olarak [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) (0x7FFD) kullanın. Bu önceden tanımlanmış bir işaretçidir ve geçerli bir öğe indeksi değildir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | short |  |

### setCurrentPageItemText(String value) {#setCurrentPageItemText-java.lang.String-}
```
public void setCurrentPageItemText(String value)
```


Bu pivot alanı için geçerli sayfa öğesinin görüntü metnini alır (yalnızca sayfa alanı).

**Remarks**

\"(All)\" döndürür, [getCurrentPageItem()](../../com.aspose.cells/pivotfield\\#getCurrentPageItem--) [PivotItem.ALL\\_PAGE\\_ITEMS\\_INDEX](../../com.aspose.cells/pivotitem\\#ALL-PAGE-ITEMS-INDEX) eşit olduğunda. Diğer değerler için, öğe indeksinin dize temsili döndürülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Pivot tablo görünümünde pivot alanının görüntü adını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDragToColumn(boolean value) {#setDragToColumn-boolean-}
```
public void setDragToColumn(boolean value)
```


Belirtilen alanın sütun bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.AllowDraggingToColumn özelliğini kullanın. Bu yöntem, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDragToData(boolean value) {#setDragToData-boolean-}
```
public void setDragToData(boolean value)
```


Belirtilen alanın değerler bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.AllowDraggingToData özelliğini kullanın. Bu yöntem, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDragToHide(boolean value) {#setDragToHide-boolean-}
```
public void setDragToHide(boolean value)
```


Bu pivot alanının PivotTable görünümünden kaldırılıp kaldırılamayacağını gösterir. Varsayılan değer doğrudur.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.AllowRemovingFromView özelliğini kullanın. Bu yöntem, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDragToPage(boolean value) {#setDragToPage-boolean-}
```
public void setDragToPage(boolean value)
```


Belirtilen alanın sayfa bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.AllowDraggingToPage özelliğini kullanın. Bu yöntem, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDragToRow(boolean value) {#setDragToRow-boolean-}
```
public void setDragToRow(boolean value)
```


Belirtilen alanın satır bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.AllowDraggingToRow özelliğini kullanın. Bu yöntem, Temmuz 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFunction(int value) {#setFunction-int-}
```
public void setFunction(int value)
```


Bu PivotTable veri alanını özetlemek için kullanılan işlevi temsil eder.

Bakınız [ConsolidationFunction](../../com.aspose.cells/consolidationfunction).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setIncludeNewItemsInFilter(boolean value) {#setIncludeNewItemsInFilter-boolean-}
```
public void setIncludeNewItemsInFilter(boolean value)
```


Alana yeni öğelerin manuel filtreye dahil edilip edilmeyeceğini belirtir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setInsertBlankRow(boolean value) {#setInsertBlankRow-boolean-}
```
public void setInsertBlankRow(boolean value)
```


Her öğeden sonra boş bir satır eklenip eklenmeyeceğini belirtir. Yalnızca satır alanları için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setInsertPageBreaksBetweenItems(boolean value) {#setInsertPageBreaksBetweenItems-boolean-}
```
public void setInsertPageBreaksBetweenItems(boolean value)
```


Her öğeden sonra sayfa sonu eklenip eklenmeyeceğini belirtir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMultipleItemSelectionAllowed(boolean value) {#setMultipleItemSelectionAllowed-boolean-}
```
public void setMultipleItemSelectionAllowed(boolean value)
```


Sayfa alanında birden fazla öğenin seçilip seçilemeyeceğini belirtir. Varsayılan değer false'tur.

**Remarks**

Yalnızca sayfa (filtre) alanları için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


PivotField adını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setNonAutoSortDefault(boolean value) {#setNonAutoSortDefault-boolean-}
```
public void setNonAutoSortDefault(boolean value)
```


Bu pivot alanına uygulanacak sıralama işleminin otomatik sıralama mı yoksa basit veri sıralaması mı olduğunu gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen !PivotField.SortSetting.IsSimpleSort özelliğini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Sayıların ve tarihlerin yerleşik görüntü biçimini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Sayıların ve tarihlerin özel görüntü biçimini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setRepeatItemLabels(boolean value) {#setRepeatItemLabels-boolean-}
```
public void setRepeatItemLabels(boolean value)
```


Satır veya sütun bölgesinde alan etiketlerinin tekrarlanıp tekrarlanmayacağını belirtir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


PivotTable görünümünde özet veri içermeseler bile tüm öğelerin gösterilip gösterilmeyeceğini belirtir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowCompact(boolean value) {#setShowCompact-boolean-}
```
public void setShowCompact(boolean value)
```


Pivot Table görünümünde aynı sütunda bir sonraki alanın etiketlerinin gösterilip gösterilmeyeceğini belirtir. Yalnızca satır alanları için.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.ShowInCompactForm özelliğini kullanın. Bu yöntem Kasım 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowInCompactForm(boolean value) {#setShowInCompactForm-boolean-}
```
public void setShowInCompactForm(boolean value)
```


Bu satır alanının sıkıştırılmış form düzeni kullanıp kullanmayacağını belirten bir değer ayarlar. Yalnızca satır alanlarına uygulanır.

**Remarks**

Kompakt form, taslak düzenin bir alt modudur. Bu ayar yalnızca [getShowInOutlineForm()](../../com.aspose.cells/pivotfield\#getShowInOutlineForm--) true olduğunda etkili olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowInOutlineForm(boolean value) {#setShowInOutlineForm-boolean-}
```
public void setShowInOutlineForm(boolean value)
```


Bu satır alanının anahat düzeni kullanıp kullanmayacağını belirten bir değer ayarlar. Yalnızca satır alanlarına uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowSubtotalAtTop(boolean value) {#setShowSubtotalAtTop-boolean-}
```
public void setShowSubtotalAtTop(boolean value)
```


Alt toplamların öğelerin üstünde mi yoksa altında mı gösterileceğini belirtir.

**Remarks**

ShowInOutlineForm true olduğunda yalnızca satır bölgesindeki pivot alanları için çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSubtotals(int value) {#setSubtotals-int-}
```
public void setSubtotals(int value)
```


Alan için alt toplamları ayarlar. Yalnızca Satır veya Sütun pivot alanı için.

[PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) adresine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSubtotals(int subtotalType, boolean shown) {#setSubtotals-int-boolean-}
```
public void setSubtotals(int subtotalType, boolean shown)
```


Belirtilen alanın nasıl alt toplamlandırılacağını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| subtotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| gösterildi | boolean | Belirtilen alanın bu alt toplamları gösterip göstermediği. |

### showAllDetails() {#showAllDetails--}
```
public void showAllDetails()
```


Her pivot öğesinin tüm ayrıntılarını göster.

### showValuesAs(int showValuesAsType, int baseField, int baseItem) {#showValuesAs-int-int-int-}
```
public void showValuesAs(int showValuesAsType, int baseField, int baseItem)
```


Sets the \"Show Values As\" calculation for this pivot field.

**Remarks**

Yalnızca veri alanı için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). \"Show Values As\" hesaplamasının türü. |
| baseField | int | Hesaplama için kullanılan temel alanın indeksi. |
| baseItem | int | Hesaplama için temel öğenin indeksi. Önceki öğe için [PivotShowValuesSetting.PREVIOUS\\_PIVOT\\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\\#PREVIOUS-PIVOT-ITEM) (-1), sonraki öğe için [PivotShowValuesSetting.NEXT\\_PIVOT\\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\\#NEXT-PIVOT-ITEM) (-2) kullanın; negatif olmayan değerler belirli bir pivot öğesinin sıralı indeksini gösterir. |

### showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem) {#showValuesAs-int-int-int-int-}
```
public void showValuesAs(int displayFormat, int baseField, int baseItemPositionType, int baseItem)
```


ShowDataAs hesabı kullanıldığında veri alanının değerlerini farklı bir görüntü biçiminde gösterir.

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen PivotField.ShowValuesAs(PivotShowValuesAsType,int,int) yöntemini kullanın. Bu yöntem Kasım 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| displayFormat | int | [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat). Veri görüntüleme formatı türü. |
| baseField | int | ShowDataAs hesabının dayandığı alanın indeksi. |
| baseItemPositionType | int | [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype). Temel öğenin konum türü. |
| baseItem | int | ShowDataAs hesabının dayandığı temel öğenin indeksi. Yalnızca baseItemPositionType özel olduğunda çalışır. |

### showValuesAs(int showValuesAsType, String baseField, String baseItem) {#showValuesAs-int-java.lang.String-java.lang.String-}
```
public void showValuesAs(int showValuesAsType, String baseField, String baseItem)
```


"Değerleri Şöyle Göster" hesabını bu veri alanı için yapılandırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| showValuesAsType | int | [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype). Show Values As için hesaplama türü. |
| baseField | java.lang.String | Hesaplamada kullanılan temel alanın adı. |
| baseItem | java.lang.String | Normal bir pivot öğesinin başlığı. Ayrıca ayrılmış kelime anahtarlarını kabul eder: `(previous)` önceki öğe için, `(next)` sonraki öğe için. Seçilen hesaplama türü bir temel öğe gerektirmiyorsa `null` gönderin. |

### sortBy(int sortType) {#sortBy-int-}
```
public void sortBy(int sortType)
```


Bu pivot alanını sıralar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Bu alanın sıralama türü. |

### sortBy(int sortType, int fieldSortedBy) {#sortBy-int-int-}
```
public void sortBy(int sortType, int fieldSortedBy)
```


Bu pivot alanını sıralar.

**Remarks**

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen PivotField.SortBy(SortOrder, int,string) yöntemini veya PivotField.IsAutoSort özelliğini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Bu alanın sıralama türü. |
| fieldSortedBy | int | Sıralama yapılan pivot alanının indeksi. -1, bu alanın veri etiketlerine göre sıralama anlamına gelir, diğer değerler sıralanan veri alanının indeksini ifade eder. |

### sortBy(int sortType, int fieldSortedBy, int dataType, String cellName) {#sortBy-int-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, int dataType, String cellName)
```


Bu pivot alanını sıralar.

**Remarks**

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen PivotField.SortBy(SortOrder, int,string) yöntemini kullanın. Bu yöntem, Eylül 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Bu alanın sıralama türü. |
| fieldSortedBy | int | Sıralama yapılan pivot alanının indeksi. -1, bu alanın veri etiketlerine göre sıralama anlamına gelir, diğer değerler sıralanan veri alanının indeksini ifade eder. |
| dataType | int | [PivotLineType](../../com.aspose.cells/pivotlinetype). Sıralanan veri türü. |
| cellName | java.lang.String | Satır veya sütundaki değerlere göre sırala |

### sortBy(int sortType, int fieldSortedBy, String cellName) {#sortBy-int-int-java.lang.String-}
```
public void sortBy(int sortType, int fieldSortedBy, String cellName)
```


Bu pivot alanını sıralar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sortType | int | [SortOrder](../../com.aspose.cells/sortorder). Bu alanın sıralama türü. |
| fieldSortedBy | int | Sıralama yapılan pivot alanının indeksi. -1, bu alanın veri etiketlerine göre sıralama anlamına gelir, diğer değerler sıralanan veri alanının indeksini ifade eder. |
| cellName | java.lang.String | Satır veya sütundaki değerlere göre sırala. Null ise, alanın toplamına göre grupla; aksi takdirde seçilen sütun veya satırdaki değerlere göre grupla. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy) {#top10AutoShow-boolean-boolean-int-int-}
```
public void top10AutoShow(boolean isAutoShow, boolean isTop, int count, int rankBy)
```


Bu pivot alanı için Top10 Otomatik Göster ayarlarını yapılandırır.

**Remarks**

Bu yöntem .XLS ikili formatını yapılandırır: AutoShow (Top10) yerel ve tek desteklenen seçenektir. XLSX (OpenXML): Alt dosya formatı Top10 AutoShow'u destekler, ancak Excel 2007 ve sonraki sürümlerin kullanıcı arayüzü bunu yalnızca Top10 filtresi aracılığıyla gösterir. XLS uyumluluğu gerekmezse, yerine Top10 filtresinin kullanılması önerilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isAutoShow | boolean | AutoShow'u etkinleştirmek için true; devre dışı bırakmak için false. |
| isTop | boolean | True ise üst öğeleri gösterir; false ise alt öğeleri gösterir. |
| sayı | int | Gösterilecek üst/alt öğe sayısı. |
| rankBy | int | Sıralama için kullanılan veri alanının indeksi. Pivot öğesinin kendi değerlerine göre sıralamak için -1 kullanın. |

### ungroup() {#ungroup--}
```
public void ungroup()
```


Pivot alanının grubunu kaldır.

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

