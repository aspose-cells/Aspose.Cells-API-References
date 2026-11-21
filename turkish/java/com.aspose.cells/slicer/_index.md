---
title: "Dilimleyici"
second_title: "Aspose.Cells for Java API Referansı"
description: "Slicer View'in özet açıklaması"
type: docs
url: /tr/java/com.aspose.cells/slicer/
---

**Inheritance:**
java.lang.Object
```
public class Slicer
```

Slicer View'in özet açıklaması

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
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
 
         slicer.unselectItems(new String[] { "grape" });
         //do your business
         book.save("out.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addPivotConnection(PivotTable pivot)](#addPivotConnection-com.aspose.cells.PivotTable-) | PivotTable bağlantısı ekler. |
| [clearFilter()](#clearFilter--) | Filtreleri kaldır |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Slicer nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar. |
| [getCaption()](#getCaption--) | Belirtilen slicer'ın başlığını döndürür veya ayarlar. |
| [getCaptionVisible()](#getCaptionVisible--) | Slicer başlığını gösteren üstbilginin görünür olup olmadığını döndürür veya ayarlar. |
| [getClass()](#getClass--) |  |
| [getColumnWidth()](#getColumnWidth--) | Slicer'daki her sütunun genişliğini nokta biriminde döndürür veya ayarlar. |
| [getColumnWidthPixel()](#getColumnWidthPixel--) | Alır genişliğini\\u807dher sütun içinde\\u807dslicer, birim olarak\\u807dpiksel.\\u807d |
| [getFirstItemIndex()](#getFirstItemIndex--) | İlk slicer öğesinin sıfır tabanlı indeksini belirtir. |
| [getHeight()](#getHeight--) | Belirtilen slicer'ın yüksekliğini nokta biriminde döndürür veya ayarlar. |
| [getHeightPixel()](#getHeightPixel--) | Belirtilen dilimleyicinin yüksekliğini döndürür veya ayarlar, piksel cinsinden. |
| [getLeftPixel()](#getLeftPixel--) | Dilimleyici şeklinin sol sütunundan yatay ofsetini döndürür veya ayarlar, piksel cinsinden. |
| [getLockedAspectRatio()](#getLockedAspectRatio--) | En‑boy oranının kilitlenip kilitlenmediğini gösterir. |
| [getLockedPosition()](#getLockedPosition--) | Belirtilen dilimleyicinin kullanıcı arayüzü kullanılarak taşınıp taşınamayacağını veya yeniden boyutlandırılıp yeniden boyutlandırılamayacağını gösterir. |
| [getName()](#getName--) | Belirtilen dilimleyicinin adını döndürür veya ayarlar |
| [getNumberOfColumns()](#getNumberOfColumns--) | Dilimleyicideki sütun sayısını döndürür veya ayarlar. |
| [getParent()](#getParent--) | Bu dilimleyiciyi içeren [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) nesnesini döndürür. |
| [getPlacement()](#getPlacement--) | Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder. |
| [getRowHeight()](#getRowHeight--) | Belirtilen dilimleyicideki her satırın yüksekliğini puan biriminde döndürür veya ayarlar. |
| [getRowHeightPixel()](#getRowHeightPixel--) | Belirtilen dilimleyicideki her satırın yüksekliğini piksel biriminde döndürür veya ayarlar. |
| [getShape()](#getShape--) | Belirtilen dilimleyiciyle ilişkili Shape nesnesini döndürür. |
| [getShowAllItems()](#getShowAllItems--) | Veri olmaması veya öğelerin silinmiş olması durumunda bile tüm öğelerin gösterilip gösterilmeyeceğini belirtir. |
| [getShowCaption()](#getShowCaption--) | Dilimleyicinin başlığının görünür olup olmadığını gösterir. |
| [getShowMissing()](#getShowMissing--) | Veri kaynağından silinen öğelerin gösterilip gösterilmeyeceğini belirtir. |
| [getShowTypeOfItemsWithNoData()](#getShowTypeOfItemsWithNoData--) | Veri kaynağından silinen öğelerin gösterilip gösterilmeyeceğini belirtir. |
| [getSlicerCache()](#getSlicerCache--) | Dilimleyiciyle ilişkili SlicerCache nesnesini döndürür. |
| [getSortOrderType()](#getSortOrderType--) | Öğelerin sıralama türünü gösterir. |
| [getStyleType()](#getStyleType--) | Yerleşik dilimleyici stilinin türünü belirtin. |
| [getTitle()](#getTitle--) | Mevcut Slicer nesnesinin başlığını belirtir. |
| [getTopPixel()](#getTopPixel--) | Dilimleyici şeklinin üst satırından dikey ofsetini döndürür veya ayarlar, piksel cinsinden. |
| [getWidth()](#getWidth--) | Belirtilen dilimleyicinin genişliğini puan biriminde döndürür veya ayarlar. |
| [getWidthPixel()](#getWidthPixel--) | Belirtilen dilimleyicinin genişliğini piksel biriminde döndürür veya ayarlar. |
| [getWorksheet()](#getWorksheet--) | Bu dilimleyiciyi içeren [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) nesnesini döndürür. |
| [hashCode()](#hashCode--) |  |
| [isLocked()](#isLocked--) | Dilimleyici şeklinin kilitli olup olmadığını gösterir. |
| [isPrintable()](#isPrintable--) | Dilimleyici nesnesinin yazdırılabilir olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Dilimleyicinin öğelerini ilişkili pivot tablolarından yenileme. |
| [removePivotConnection(PivotTable pivot)](#removePivotConnection-com.aspose.cells.PivotTable-) | PivotTable bağlantısını kaldırır. |
| [selectItems(String[] labels, boolean append)](#selectItems-java.lang.String---boolean-) | **Notlar** |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Slicer nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar. |
| [setCaption(String value)](#setCaption-java.lang.String-) | Belirtilen slicer'ın başlığını döndürür veya ayarlar. |
| [setCaptionVisible(boolean value)](#setCaptionVisible-boolean-) | Slicer başlığını gösteren üstbilginin görünür olup olmadığını döndürür veya ayarlar. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Slicer'daki her sütunun genişliğini nokta biriminde döndürür veya ayarlar. |
| [setColumnWidthPixel(int value)](#setColumnWidthPixel-int-) | Genişliği ayarlar\u807ddilimleyicideki her sütun\u807d dilimleyici, birim olarak\u807dpiksel.\u807d |
| [setFirstItemIndex(int value)](#setFirstItemIndex-int-) | İlk slicer öğesinin sıfır tabanlı indeksini belirtir. |
| [setHeight(double value)](#setHeight-double-) | Belirtilen slicer'ın yüksekliğini nokta biriminde döndürür veya ayarlar. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Belirtilen dilimleyicinin yüksekliğini döndürür veya ayarlar, piksel cinsinden. |
| [setLeftPixel(int value)](#setLeftPixel-int-) | Dilimleyici şeklinin sol sütunundan yatay ofsetini döndürür veya ayarlar, piksel cinsinden. |
| [setLocked(boolean value)](#setLocked-boolean-) | Dilimleyici şeklinin kilitli olup olmadığını gösterir. |
| [setLockedAspectRatio(boolean value)](#setLockedAspectRatio-boolean-) | En‑boy oranının kilitlenip kilitlenmediğini gösterir. |
| [setLockedPosition(boolean value)](#setLockedPosition-boolean-) | Belirtilen dilimleyicinin kullanıcı arayüzü kullanılarak taşınıp taşınamayacağını veya yeniden boyutlandırılıp yeniden boyutlandırılamayacağını gösterir. |
| [setName(String value)](#setName-java.lang.String-) | Belirtilen dilimleyicinin adını döndürür veya ayarlar |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Dilimleyicideki sütun sayısını döndürür veya ayarlar. |
| [setPlacement(int value)](#setPlacement-int-) | Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Dilimleyici nesnesinin yazdırılabilir olup olmadığını gösterir. |
| [setRowHeight(double value)](#setRowHeight-double-) | Belirtilen dilimleyicideki her satırın yüksekliğini puan biriminde döndürür veya ayarlar. |
| [setRowHeightPixel(int value)](#setRowHeightPixel-int-) | Belirtilen dilimleyicideki her satırın yüksekliğini piksel biriminde döndürür veya ayarlar. |
| [setShowAllItems(boolean value)](#setShowAllItems-boolean-) | Veri olmaması veya öğelerin silinmiş olması durumunda bile tüm öğelerin gösterilip gösterilmeyeceğini belirtir. |
| [setShowCaption(boolean value)](#setShowCaption-boolean-) | Dilimleyicinin başlığının görünür olup olmadığını gösterir. |
| [setShowMissing(boolean value)](#setShowMissing-boolean-) | Veri kaynağından silinen öğelerin gösterilip gösterilmeyeceğini belirtir. |
| [setShowTypeOfItemsWithNoData(int value)](#setShowTypeOfItemsWithNoData-int-) | Veri kaynağından silinen öğelerin gösterilip gösterilmeyeceğini belirtir. |
| [setSortOrderType(int value)](#setSortOrderType-int-) | Öğelerin sıralama türünü gösterir. |
| [setStyleType(int value)](#setStyleType-int-) | Yerleşik dilimleyici stilinin türünü belirtin. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Mevcut Slicer nesnesinin başlığını belirtir. |
| [setTopPixel(int value)](#setTopPixel-int-) | Dilimleyici şeklinin üst satırından dikey ofsetini döndürür veya ayarlar, piksel cinsinden. |
| [setWidth(double value)](#setWidth-double-) | Belirtilen dilimleyicinin genişliğini puan biriminde döndürür veya ayarlar. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Belirtilen dilimleyicinin genişliğini piksel biriminde döndürür veya ayarlar. |
| [toString()](#toString--) |  |
| [unselectItems(String[] labels)](#unselectItems-java.lang.String---) | Seçili filtre etiketlerini kaldır. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addPivotConnection(PivotTable pivot) {#addPivotConnection-com.aspose.cells.PivotTable-}
```
public void addPivotConnection(PivotTable pivot)
```


PivotTable bağlantısı ekler.

**Example**

```
         slicer.addPivotConnection(pivot);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |

### clearFilter() {#clearFilter--}
```
public void clearFilter()
```


Filtreleri kaldır

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Slicer nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getCaption() {#getCaption--}
```
public String getCaption()
```


Belirtilen slicer'ın başlığını döndürür veya ayarlar.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
java.lang.String
### getCaptionVisible() {#getCaptionVisible--}
```
public boolean getCaptionVisible()
```


Slicer başlığını gösteren başlığın görünür olup olmadığını döndürür veya ayarlar. Varsayılan değer true'tir.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.setCaption("slicer caption");
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Slicer'daki her sütunun genişliğini nokta biriminde döndürür veya ayarlar.

**Example**

```
         slicer.setColumnWidth(80);
```

**Returns:**
double
### getColumnWidthPixel() {#getColumnWidthPixel--}
```
public int getColumnWidthPixel()
```


Alır genişliğini\\u807dher sütun içinde\\u807dslicer, birim olarak\\u807dpiksel.\\u807d

**Example**

```
         slicer.setColumnWidthPixel(120);
```

**Returns:**
int
### getFirstItemIndex() {#getFirstItemIndex--}
```
public int getFirstItemIndex()
```


İlk slicer öğesinin sıfır tabanlı indeksini belirtir.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Belirtilen slicer'ın yüksekliğini nokta biriminde döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen Shape.HeightPt özelliğini kullanın. Bu özellik, Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Belirtilen dilimleyicinin yüksekliğini döndürür veya ayarlar, piksel cinsinden.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Height özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


Dilimleyici şeklinin sol sütunundan yatay ofsetini döndürür veya ayarlar, piksel cinsinden.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Left özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getLockedAspectRatio() {#getLockedAspectRatio--}
```
public boolean getLockedAspectRatio()
```


En‑boy oranının kilitlenip kilitlenmediğini gösterir.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--) metodunu kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### getLockedPosition() {#getLockedPosition--}
```
public boolean getLockedPosition()
```


Belirtilen dilimleyicinin kullanıcı arayüzü kullanılarak taşınıp taşınamayacağını veya yeniden boyutlandırılıp yeniden boyutlandırılamayacağını gösterir.

**Example**

```
         slicer.setLockedPosition(false);
```

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Belirtilen dilimleyicinin adını döndürür veya ayarlar

**Example**

```
         slicer.setName("slicer name");
```

**Returns:**
java.lang.String
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


Slicer'daki sütun sayısını döndürür veya ayarlar. Varsayılan değer 1'dir.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getParent() {#getParent--}
```
public Worksheet getParent()
```


Bu slicer'ı içeren [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) nesnesini döndürür. Salt okunur.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder. Özellik, bir nesnenin çalışma sayfasındaki konumunu kontrol eder.

Bakınız [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Belirtilen dilimleyicideki her satırın yüksekliğini puan biriminde döndürür veya ayarlar.

**Example**

```
         slicer.setRowHeight(20);
```

**Returns:**
double
### getRowHeightPixel() {#getRowHeightPixel--}
```
public int getRowHeightPixel()
```


Belirtilen dilimleyicideki her satırın yüksekliğini piksel biriminde döndürür veya ayarlar.

**Example**

```
         slicer.setRowHeightPixel(30);
```

**Returns:**
int
### getShape() {#getShape--}
```
public SlicerShape getShape()
```


Belirtilen slicer ile ilişkili Shape nesnesini döndürür. Salt okunur.

**Returns:**
[SlicerShape](../../com.aspose.cells/slicershape)
### getShowAllItems() {#getShowAllItems--}
```
public boolean getShowAllItems()
```


Veri yoksa veya silinmiş olsa bile tüm öğelerin gösterilip gösterilmeyeceğini belirtir. Varsayılan değer true'tir;

**Returns:**
boolean
### getShowCaption() {#getShowCaption--}
```
public boolean getShowCaption()
```


Slicer başlığının görünür olup olmadığını belirtir. Varsayılan değer true'tir.

**Example**

```
         slicer.setShowCaption(false);
```

**Returns:**
boolean
### getShowMissing() {#getShowMissing--}
```
public boolean getShowMissing()
```


Veri kaynağından silinen öğelerin gösterilip gösterilmeyeceğini belirtir.

**Remarks**

Yalnızca [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) true olduğunda çalışır.

**Returns:**
boolean
### getShowTypeOfItemsWithNoData() {#getShowTypeOfItemsWithNoData--}
```
public int getShowTypeOfItemsWithNoData()
```


Veri kaynağından silinen öğelerin gösterilip gösterilmeyeceğini belirtir.

Bakınız [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Yalnızca [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) true olduğunda çalışır.

**Returns:**
int
### getSlicerCache() {#getSlicerCache--}
```
public SlicerCache getSlicerCache()
```


Slicer ile ilişkili SlicerCache nesnesini döndürür. Salt okunur.

**Example**

```
         SlicerCache slicerCache = slicer.getSlicerCache();
```

**Returns:**
[SlicerCache](../../com.aspose.cells/slicercache)
### getSortOrderType() {#getSortOrderType--}
```
public int getSortOrderType()
```


Öğelerin sıralama türünü gösterir.

[SortOrder](../../com.aspose.cells/sortorder) öğesine bakın.

**Returns:**
int
### getStyleType() {#getStyleType--}
```
public int getStyleType()
```


Yerleşik slicer stilinin türünü belirtin. Varsayılan tür SlicerStyleLight1'dir.

Bakınız [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Example**

```
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
```

**Returns:**
int
### getTitle() {#getTitle--}
```
public String getTitle()
```


Mevcut Slicer nesnesinin başlığını belirtir.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [Shape.getTitle()](../../com.aspose.cells/shape\#getTitle--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
java.lang.String
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


Dilimleyici şeklinin üst satırından dikey ofsetini döndürür veya ayarlar, piksel cinsinden.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Top özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Belirtilen dilimleyicinin genişliğini puan biriminde döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen Shape.WidthPt özelliğini kullanın. Bu özellik, Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
double
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Belirtilen dilimleyicinin genişliğini piksel biriminde döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Width özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.setNumberOfColumns(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Bu slicer'ı içeren [getWorksheet()](../../com.aspose.cells/slicer\#getWorksheet--) nesnesini döndürür. Salt okunur.

**Example**

```
         Worksheet currSheet = slicer.getParent();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Dilimleyici şeklinin kilitli olup olmadığını gösterir.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [Shape.isLocked()](../../com.aspose.cells/shape\#isLocked--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


Dilimleyici nesnesinin yazdırılabilir olup olmadığını gösterir.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [Shape.isPrintable()](../../com.aspose.cells/shape\#isPrintable--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Example**

```
         slicer.removePivotConnection(pivot);
```

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




### refresh() {#refresh--}
```
public void refresh()
```


Dilimleyicinin öğelerini ilişkili pivot tablolarından yenileme.

**Example**

```
         slicer.refresh();
```

### removePivotConnection(PivotTable pivot) {#removePivotConnection-com.aspose.cells.PivotTable-}
```
public void removePivotConnection(PivotTable pivot)
```


PivotTable bağlantısını kaldırır.

**Example**

```
         slicer.removePivotConnection(pivot);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |

### selectItems(String[] labels, boolean append) {#selectItems-java.lang.String---boolean-}
```
public void selectItems(String[] labels, boolean append)
```


**Remarks**

Tüm öğeleri seçmek istiyorsanız, lütfen [clearFilter()](../../com.aspose.cells/slicer\#clearFilter--) metodunu kullanın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| etiketler | java.lang.String[] | Seçilen etiketler. |
| ekle | boolean | False, yalnızca bu etiketleri seçmek ve diğerlerini seçimi kaldırmak anlamına gelir. True, eski seçili öğeleri korumak ve bu etiketleri seçmek anlamına gelir. |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Slicer nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [Shape.getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


Belirtilen slicer'ın başlığını döndürür veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCaptionVisible(boolean value) {#setCaptionVisible-boolean-}
```
public void setCaptionVisible(boolean value)
```


Slicer başlığını gösteren başlığın görünür olup olmadığını döndürür veya ayarlar. Varsayılan değer true'tir.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [getShowCaption()](../../com.aspose.cells/slicer\#getShowCaption--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Slicer'daki her sütunun genişliğini nokta biriminde döndürür veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setColumnWidthPixel(int value) {#setColumnWidthPixel-int-}
```
public void setColumnWidthPixel(int value)
```


Genişliği ayarlar\u807ddilimleyicideki her sütun\u807d dilimleyici, birim olarak\u807dpiksel.\u807d

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFirstItemIndex(int value) {#setFirstItemIndex-int-}
```
public void setFirstItemIndex(int value)
```


İlk slicer öğesinin sıfır tabanlı indeksini belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Belirtilen slicer'ın yüksekliğini nokta biriminde döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen Shape.HeightPt özelliğini kullanın. Bu özellik, Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Belirtilen dilimleyicinin yüksekliğini döndürür veya ayarlar, piksel cinsinden.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Height özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```


Dilimleyici şeklinin sol sütunundan yatay ofsetini döndürür veya ayarlar, piksel cinsinden.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Left özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Dilimleyici şeklinin kilitli olup olmadığını gösterir.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [Shape.isLocked()](../../com.aspose.cells/shape\#isLocked--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLockedAspectRatio(boolean value) {#setLockedAspectRatio-boolean-}
```
public void setLockedAspectRatio(boolean value)
```


En‑boy oranının kilitlenip kilitlenmediğini gösterir.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [Shape.isAspectRatioLocked()](../../com.aspose.cells/shape\#isAspectRatioLocked--) metodunu kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLockedPosition(boolean value) {#setLockedPosition-boolean-}
```
public void setLockedPosition(boolean value)
```


Belirtilen dilimleyicinin kullanıcı arayüzü kullanılarak taşınıp taşınamayacağını veya yeniden boyutlandırılıp yeniden boyutlandırılamayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Belirtilen dilimleyicinin adını döndürür veya ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Slicer'daki sütun sayısını döndürür veya ayarlar. Varsayılan değer 1'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Çizim nesnesinin altındaki hücrelere nasıl bağlandığını temsil eder. Özellik, bir nesnenin çalışma sayfasındaki konumunu kontrol eder.

Bakınız [PlacementType](../../com.aspose.cells/placementtype).

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [Shape.getPlacement()](../../com.aspose.cells/shape\#getPlacement--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Dilimleyici nesnesinin yazdırılabilir olup olmadığını gösterir.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [Shape.isPrintable()](../../com.aspose.cells/shape\#isPrintable--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Belirtilen dilimleyicideki her satırın yüksekliğini puan biriminde döndürür veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setRowHeightPixel(int value) {#setRowHeightPixel-int-}
```
public void setRowHeightPixel(int value)
```


Belirtilen dilimleyicideki her satırın yüksekliğini piksel biriminde döndürür veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setShowAllItems(boolean value) {#setShowAllItems-boolean-}
```
public void setShowAllItems(boolean value)
```


Veri yoksa veya silinmiş olsa bile tüm öğelerin gösterilip gösterilmeyeceğini belirtir. Varsayılan değer true'tir;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowCaption(boolean value) {#setShowCaption-boolean-}
```
public void setShowCaption(boolean value)
```


Slicer başlığının görünür olup olmadığını belirtir. Varsayılan değer true'tir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowMissing(boolean value) {#setShowMissing-boolean-}
```
public void setShowMissing(boolean value)
```


Veri kaynağından silinen öğelerin gösterilip gösterilmeyeceğini belirtir.

**Remarks**

Yalnızca [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) true olduğunda çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowTypeOfItemsWithNoData(int value) {#setShowTypeOfItemsWithNoData-int-}
```
public void setShowTypeOfItemsWithNoData(int value)
```


Veri kaynağından silinen öğelerin gösterilip gösterilmeyeceğini belirtir.

Bakınız [ItemsWithNoDataShowMode](../../com.aspose.cells/itemswithnodatashowmode).

**Remarks**

Yalnızca [getShowAllItems()](../../com.aspose.cells/slicer\#getShowAllItems--) true olduğunda çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSortOrderType(int value) {#setSortOrderType-int-}
```
public void setSortOrderType(int value)
```


Öğelerin sıralama türünü gösterir.

[SortOrder](../../com.aspose.cells/sortorder) öğesine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setStyleType(int value) {#setStyleType-int-}
```
public void setStyleType(int value)
```


Yerleşik slicer stilinin türünü belirtin. Varsayılan tür SlicerStyleLight1'dir.

Bakınız [SlicerStyleType](../../com.aspose.cells/slicerstyletype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Mevcut Slicer nesnesinin başlığını belirtir.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen [Shape.getTitle()](../../com.aspose.cells/shape\#getTitle--) özelliğini kullanın. Bu özellik, Ocak 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


Dilimleyici şeklinin üst satırından dikey ofsetini döndürür veya ayarlar, piksel cinsinden.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Top özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Belirtilen dilimleyicinin genişliğini puan biriminde döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen Shape.WidthPt özelliğini kullanın. Bu özellik, Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Belirtilen dilimleyicinin genişliğini piksel biriminde döndürür veya ayarlar.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Shape.Width özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unselectItems(String[] labels) {#unselectItems-java.lang.String---}
```
public void unselectItems(String[] labels)
```


Seçili filtre etiketlerini kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| etiketler | java.lang.String[] | Etiketler. |

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

