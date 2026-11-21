---
title: "PivotShowValuesSetting"
second_title: "Aspose.Cells for Java API Referansı"
description: "ShowDataAs hesabı kullanıldığında değerlerin nasıl gösterileceğiyle ilgili ayarları temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotshowvaluessetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotShowValuesSetting
```

ShowDataAs hesabı kullanıldığında değerlerin nasıl gösterileceğiyle ilgili ayarları temsil eder.

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
 
         PivotField dataField = pivot.getDataFields().get(0);
         // Display value as percentage of the grand total
         dataField.showValuesAs(PivotShowValuesAsType.PERCENTAGE_OF_TOTAL, 0, PivotShowValuesSetting.NEXT_PIVOT_ITEM);
         // Get the display calculation setting of data field
         PivotShowValuesSetting settings = dataField.getShowValuesSetting();
         System.out.println(settings.getShowValuesAs());
 
          pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [NEXT_PIVOT_ITEM](#NEXT-PIVOT-ITEM) | Özel temel öğe indeksi: sonraki pivot öğesini kullan. |
| [PREVIOUS_PIVOT_ITEM](#PREVIOUS-PIVOT-ITEM) | Özel temel öğe indeksi: önceki pivot öğesini kullan. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | ShowDataAs hesabı kullanıldığında ShowDataAs hesabı için temel alanı temsil eder. |
| [getBaseFieldName()](#getBaseFieldName--) | Pivot temel alanının başlığını alır. |
| [getBaseItemCaption()](#getBaseItemCaption--) | Temel alandaki pivot öğesinin başlığını alır. |
| [getBaseItemIndex()](#getBaseItemIndex--) | ShowDataAs hesabı kullanıldığında temel alandaki pivot öğesinin özel indeksini temsil eder. |
| [getBaseItemPositionType()](#getBaseItemPositionType--) | ShowDataAs hesaplaması kullanıldığında temel alan içindeki temel pivot öğesinin türünü temsil eder. |
| [getCalculationType()](#getCalculationType--) | Veri alanının değerlerinin pivot raporunda nasıl gösterileceğini temsil eder. |
| [getClass()](#getClass--) |  |
| [getShowValuesAs()](#getShowValuesAs--) | Veri alanının değerlerinin pivot raporunda nasıl gösterileceğini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | ShowDataAs hesabı kullanıldığında ShowDataAs hesabı için temel alanı temsil eder. |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | ShowDataAs hesabı kullanıldığında temel alandaki pivot öğesinin özel indeksini temsil eder. |
| [setBaseItemPositionType(int value)](#setBaseItemPositionType-int-) | ShowDataAs hesaplaması kullanıldığında temel alan içindeki temel pivot öğesinin türünü temsil eder. |
| [setCalculationType(int value)](#setCalculationType-int-) | Veri alanının değerlerinin pivot raporunda nasıl gösterileceğini temsil eder. |
| [setShowValuesAs(int value)](#setShowValuesAs-int-) | Veri alanının değerlerinin pivot raporunda nasıl gösterileceğini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### NEXT_PIVOT_ITEM {#NEXT-PIVOT-ITEM}
```
public static final int NEXT_PIVOT_ITEM
```


Özel temel öğe indeksi: sonraki pivot öğesini kullan. "Show Values As" hesaplamaları için geçerlidir; Excel 2010 ve sonraki sürümlerde etkilidir.

### PREVIOUS_PIVOT_ITEM {#PREVIOUS-PIVOT-ITEM}
```
public static final int PREVIOUS_PIVOT_ITEM
```


Özel temel öğe indeksi: önceki pivot öğesini kullan. "Show Values As" hesaplamaları için geçerlidir; Excel 2010 ve sonraki sürümlerde etkilidir.

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
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```


ShowDataAs hesabı kullanıldığında ShowDataAs hesabı için temel alanı temsil eder.

**Returns:**
int
### getBaseFieldName() {#getBaseFieldName--}
```
public String getBaseFieldName()
```


Pivot temel alanının başlığını alır.

**Returns:**
java.lang.String
### getBaseItemCaption() {#getBaseItemCaption--}
```
public String getBaseItemCaption()
```


Temel alandaki pivot öğesinin başlığını alır.

**Returns:**
java.lang.String
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```


ShowDataAs hesabı kullanıldığında temel alandaki pivot öğesinin özel indeksini temsil eder.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Returns:**
int
### getBaseItemPositionType() {#getBaseItemPositionType--}
```
public int getBaseItemPositionType()
```


ShowDataAs hesaplaması kullanıldığında temel alan içindeki temel pivot öğesinin türünü temsil eder. PivotItemPosition.Custom yalnızca okuma içindir; PivotItemPosition.Custom'ı ayarlamanız gerekiyorsa, lütfen PivotField.BaseItemIndex özniteliğini ayarlayın.

Bakınız [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotShowValuesSetting.BaseItem özelliğini kullanın. Bu yöntem Kasım 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getCalculationType() {#getCalculationType--}
```
public int getCalculationType()
```


Veri alanının değerlerinin pivot raporunda nasıl gösterileceğini temsil eder.

Bakınız [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotShowValuesSetting.ShowValuesAs özelliğini kullanın. Bu yöntem Kasım 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getShowValuesAs() {#getShowValuesAs--}
```
public int getShowValuesAs()
```


Veri alanının değerlerinin pivot raporunda nasıl gösterileceğini alır.

Bakınız [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBaseFieldIndex(int value) {#setBaseFieldIndex-int-}
```
public void setBaseFieldIndex(int value)
```


ShowDataAs hesabı kullanıldığında ShowDataAs hesabı için temel alanı temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


ShowDataAs hesabı kullanıldığında temel alandaki pivot öğesinin özel indeksini temsil eder.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setBaseItemPositionType(int value) {#setBaseItemPositionType-int-}
```
public void setBaseItemPositionType(int value)
```


ShowDataAs hesaplaması kullanıldığında temel alan içindeki temel pivot öğesinin türünü temsil eder. PivotItemPosition.Custom yalnızca okuma içindir; PivotItemPosition.Custom'ı ayarlamanız gerekiyorsa, lütfen PivotField.BaseItemIndex özniteliğini ayarlayın.

Bakınız [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotShowValuesSetting.BaseItem özelliğini kullanın. Bu yöntem Kasım 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCalculationType(int value) {#setCalculationType-int-}
```
public void setCalculationType(int value)
```


Veri alanının değerlerinin pivot raporunda nasıl gösterileceğini temsil eder.

Bakınız [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotShowValuesSetting.ShowValuesAs özelliğini kullanın. Bu yöntem Kasım 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setShowValuesAs(int value) {#setShowValuesAs-int-}
```
public void setShowValuesAs(int value)
```


Veri alanının değerlerinin pivot raporunda nasıl gösterileceğini ayarlar.

Bakınız [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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

