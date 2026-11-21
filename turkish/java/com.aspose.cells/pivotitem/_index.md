---
title: "PivotItem"
second_title: "Aspose.Cells for Java API Referansı"
description: "PivotField raporunda bir öğeyi temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotitem/
---

**Inheritance:**
java.lang.Object
```
public class PivotItem
```

PivotField raporunda bir öğeyi temsil eder.

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
 
         //Hide the first item
         PivotItem item = rowField.getPivotItems().get(0);          
         item.setHidden(true);
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [ALL_PAGE_ITEMS_INDEX](#ALL-PAGE-ITEMS-INDEX) | Tümünü seç sentinel dizini sayfa öğeleri için (0x7FFD, geçerli bir dizin değil) |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDateTimeValue()](#getDateTimeValue--) | Pivot öğesinin tarih saat değerini alır. Değer null ise DateTime.MinValue döndürülür. |
| [getDoubleValue()](#getDoubleValue--) | Pivot öğesinin double değerini alır. Değer null ya da sayı değilse 0 döndürülür. |
| [getFormula()](#getFormula--) | Bu hesaplanan öğenin formülünü alır. |
| [getIndex()](#getIndex--) | Pivot öğesinin önbellek alanındaki dizinini alır. |
| [getName()](#getName--) | Pivot öğesinin adını alır. |
| [getPosition()](#getPosition--) | Bu öğenin dizinini alanın tüm PivotItem'larında belirtme. |
| [getPositionInSameParentNode()](#getPositionInSameParentNode--) | Aynı üst düğüm altında bulunan PivotItem'larda konum dizinini belirtme. |
| [getStringValue()](#getStringValue--) | Pivot öğesinin dize değerini alır. Değer null ise, "" döndürür. |
| [getValue()](#getValue--) | Pivot öğesinin değerini alır. |
| [hashCode()](#hashCode--) |  |
| [hide(boolean value)](#hide-boolean-) | Pivot öğesinin gizli olup olmadığını ayarlar. |
| [isCalculatedItem()](#isCalculatedItem--) | Bu pivot öğesinin hesaplanmış formül öğesi olup olmadığını gösterir. |
| [isDetailHidden()](#isDetailHidden--) | Bu pivot öğesinin detayının gizli olup olmadığını alır. |
| [isFormula()](#isFormula--) | Bu pivot öğesinin hesaplanmış formül öğesi olup olmadığını gösterir. |
| [isHidden()](#isHidden--) | Pivot öğesinin gizli olup olmadığını alır. |
| [isHideDetail()](#isHideDetail--) | Pivot öğesinin detayı gizleyip gizlemediğini alır. |
| [isMissing()](#isMissing--) | Öğenin veri kaynağından kaldırılıp kaldırılmadığını gösterir. |
| [move(int offset)](#move-int-) | Öğeyi pivot alanında yukarı veya aşağı hareket ettirir |
| [move(int offset, boolean isSameParent)](#move-int-boolean-) | Öğeyi yukarı veya aşağı hareket ettirir |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDetailHidden(boolean value)](#setDetailHidden-boolean-) | Bu pivot öğesinin detayının gizli olup olmadığını ayarlar. |
| [setFormula(boolean value)](#setFormula-boolean-) | Bu pivot öğesinin hesaplanmış formül öğesi olup olmadığını gösterir. |
| [setHidden(boolean value)](#setHidden-boolean-) | Pivot öğesinin gizli olup olmadığını ayarlar. |
| [setHideDetail(boolean value)](#setHideDetail-boolean-) | Pivot öğesinin detayı gizleyip gizlemeyeceğini ayarlar. |
| [setIndex(int value)](#setIndex-int-) | Pivot öğesinin önbellek alanındaki dizinini alır. |
| [setName(String value)](#setName-java.lang.String-) | Pivot öğesinin adını alır. |
| [setPosition(int value)](#setPosition-int-) | Bu öğenin dizinini alanın tüm PivotItem'larında belirtme. |
| [setPositionInSameParentNode(int value)](#setPositionInSameParentNode-int-) | Aynı üst düğüm altında bulunan PivotItem'larda konum dizinini belirtme. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL_PAGE_ITEMS_INDEX {#ALL-PAGE-ITEMS-INDEX}
```
public static final short ALL_PAGE_ITEMS_INDEX
```


Tümünü seç sentinel dizini sayfa öğeleri için (0x7FFD, geçerli bir dizin değil)

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Pivot öğesinin tarih saat değerini alır. Değer null ise DateTime.MinValue döndürülür.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Pivot öğesinin double değerini alır. Değer null ya da sayı değilse 0 döndürülür.

**Returns:**
double
### getFormula() {#getFormula--}
```
public String getFormula()
```


Bu hesaplanmış öğenin formülünü alır. Yalnızca öğe hesaplanmış bir öğe olduğunda çalışır.

**Returns:**
java.lang.String -
### getIndex() {#getIndex--}
```
public int getIndex()
```


Pivot öğesinin önbellek alanındaki dizinini alır.

**Remarks**

NOT: Bu özellik artık kullanılmıyor. Bunun yerine lütfen PivotItem.Position property özelliğini kullanın. Bu yöntem Ağustos 2026'dan itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Pivot öğesinin adını alır.

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


Bu öğenin dizinini alanın tüm PivotItem'larında belirtme.

**Returns:**
int
### getPositionInSameParentNode() {#getPositionInSameParentNode--}
```
public int getPositionInSameParentNode()
```


Aynı üst düğüm altında bulunan PivotItem'larda konum dizinini belirtme.

**Remarks**

NOT: Bu yöntem artık kullanılmıyor. Bunun yerine lütfen PivotTable.MoveItem(PivotFieldType, string[],bool,int) yöntemini kullanın. Bu yöntem Kasım 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Pivot öğesinin dize değerini alır. Değer null ise, "" döndürür.

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Pivot öğesinin değerini alır.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hide(boolean value) {#hide-boolean-}
```
public void hide(boolean value)
```


Pivot öğesinin gizli olup olmadığını ayarlar.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen Aspose.Cells.Pivot.PivotItem.IsHidden özelliğini kullanın. Bu özellik OCAK 2012'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### isCalculatedItem() {#isCalculatedItem--}
```
public boolean isCalculatedItem()
```


Bu pivot öğesinin hesaplanmış formül öğesi olup olmadığını gösterir.

**Returns:**
boolean
### isDetailHidden() {#isDetailHidden--}
```
public boolean isDetailHidden()
```


Bu pivot öğesinin detayının gizli olup olmadığını alır.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Bu pivot öğesinin hesaplanmış formül öğesi olup olmadığını gösterir.

**Remarks**

NOT: Bu özellik artık kullanılmıyor. Bunun yerine lütfen PivotItem.IsCalculatedItem özelliğini kullanın. Bu özellik Kasım 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Pivot öğesinin gizli olup olmadığını alır.

**Returns:**
boolean
### isHideDetail() {#isHideDetail--}
```
public boolean isHideDetail()
```


Pivot öğesinin detayı gizleyip gizlemediğini alır.

**Remarks**

NOT: Bu özellik artık kullanılmıyor. Bunun yerine lütfen PivotItem.IsDetailHidden özelliğini kullanın. Bu özellik Kasım 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### isMissing() {#isMissing--}
```
public boolean isMissing()
```


Öğenin veri kaynağından kaldırılıp kaldırılmadığını gösterir.

**Remarks**

True, bu değerin veri kaynağından kaldırıldığını ifade eder.

**Returns:**
boolean
### move(int offset) {#move-int-}
```
public void move(int offset)
```


Öğeyi pivot alanında yukarı veya aşağı hareket ettirir

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ofset | int | Yukarı veya aşağı hareket sayısı. Değer sıfırdan küçükse öğeyi yukarı, sıfırdan büyükse öğeyi aşağı hareket ettirin. |

### move(int offset, boolean isSameParent) {#move-int-boolean-}
```
public void move(int offset, boolean isSameParent)
```


Öğeyi yukarı veya aşağı hareket ettirir

**Remarks**

NOT: Bu yöntem artık kullanılmıyor. Bunun yerine lütfen PivotTable.MoveItem(PivotFieldType, string[],bool,int) veya PivotItem.Move(int) yöntemini kullanın. Bu yöntem Kasım 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ofset | int | Yukarı veya aşağı hareket sayısı. Değer sıfırdan küçükse öğeyi yukarı, sıfırdan büyükse öğeyi aşağı hareket ettirin. |
| isSameParent | boolean | Hareket işleminin aynı üst düğümde olup olmadığını belirtme |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDetailHidden(boolean value) {#setDetailHidden-boolean-}
```
public void setDetailHidden(boolean value)
```


Bu pivot öğesinin detayının gizli olup olmadığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFormula(boolean value) {#setFormula-boolean-}
```
public void setFormula(boolean value)
```


Bu pivot öğesinin hesaplanmış formül öğesi olup olmadığını gösterir.

**Remarks**

NOT: Bu özellik artık kullanılmıyor. Bunun yerine lütfen PivotItem.IsCalculatedItem özelliğini kullanın. Bu özellik Kasım 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Pivot öğesinin gizli olup olmadığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHideDetail(boolean value) {#setHideDetail-boolean-}
```
public void setHideDetail(boolean value)
```


Pivot öğesinin detayı gizleyip gizlemeyeceğini ayarlar.

**Remarks**

NOT: Bu özellik artık kullanılmıyor. Bunun yerine lütfen PivotItem.IsDetailHidden özelliğini kullanın. Bu özellik Kasım 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setIndex(int value) {#setIndex-int-}
```
public void setIndex(int value)
```


Pivot öğesinin önbellek alanındaki dizinini alır.

**Remarks**

NOT: Bu özellik artık kullanılmıyor. Bunun yerine lütfen PivotItem.Position property özelliğini kullanın. Bu yöntem Ağustos 2026'dan itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Pivot öğesinin adını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Bu öğenin dizinini alanın tüm PivotItem'larında belirtme.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPositionInSameParentNode(int value) {#setPositionInSameParentNode-int-}
```
public void setPositionInSameParentNode(int value)
```


Aynı üst düğüm altında bulunan PivotItem'larda konum dizinini belirtme.

**Remarks**

NOT: Bu yöntem artık kullanılmıyor. Bunun yerine lütfen PivotTable.MoveItem(PivotFieldType, string[],bool,int) yöntemini kullanın. Bu yöntem Kasım 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

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

