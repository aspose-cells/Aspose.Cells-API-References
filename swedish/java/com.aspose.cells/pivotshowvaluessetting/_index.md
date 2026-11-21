---
title: "PivotShowValuesSetting"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar inställningarna för att visa värden som när ShowDataAs-beräkningen används."
type: docs
url: /sv/java/com.aspose.cells/pivotshowvaluessetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotShowValuesSetting
```

Representerar inställningarna för att visa värden som när ShowDataAs-beräkningen används.

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
## Fält

| Fält | Beskrivning |
| --- | --- |
| [NEXT_PIVOT_ITEM](#NEXT-PIVOT-ITEM) | Speciellt basobjektindex: använd det efterföljande pivotelementet. |
| [PREVIOUS_PIVOT_ITEM](#PREVIOUS-PIVOT-ITEM) | Speciellt basobjektindex: använd det föregående pivotelementet. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | Representerar basfältet för en ShowDataAs-beräkning när ShowDataAs-beräkningen är i bruk. |
| [getBaseFieldName()](#getBaseFieldName--) | Hämtar rubrik för pivots basfält. |
| [getBaseItemCaption()](#getBaseItemCaption--) | Hämtar rubrik för pivotelementet i basfältet. |
| [getBaseItemIndex()](#getBaseItemIndex--) | Representerar det anpassade indexet för pivotelementet i basfältet när beräkningen ShowDataAs används. |
| [getBaseItemPositionType()](#getBaseItemPositionType--) | Representerar typen av baspivotelementet i basfältet när beräkningen ShowDataAs används. |
| [getCalculationType()](#getCalculationType--) | Representerar hur värden i ett datafält visas i pivoterapporten. |
| [getClass()](#getClass--) |  |
| [getShowValuesAs()](#getShowValuesAs--) | Hämtar hur värden i ett datafält visas i pivoterapporten. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | Representerar basfältet för en ShowDataAs-beräkning när ShowDataAs-beräkningen är i bruk. |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | Representerar det anpassade indexet för pivotelementet i basfältet när beräkningen ShowDataAs används. |
| [setBaseItemPositionType(int value)](#setBaseItemPositionType-int-) | Representerar typen av baspivotelementet i basfältet när beräkningen ShowDataAs används. |
| [setCalculationType(int value)](#setCalculationType-int-) | Representerar hur värden i ett datafält visas i pivoterapporten. |
| [setShowValuesAs(int value)](#setShowValuesAs-int-) | Ställer in hur värden i ett datafält visas i pivoterapporten. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### NEXT_PIVOT_ITEM {#NEXT-PIVOT-ITEM}
```
public static final int NEXT_PIVOT_ITEM
```


Speciellt basindex: använd det efterföljande pivotelementet. Giltigt för "Show Values As"-beräkningar; gäller i Excel 2010 och senare.

### PREVIOUS_PIVOT_ITEM {#PREVIOUS-PIVOT-ITEM}
```
public static final int PREVIOUS_PIVOT_ITEM
```


Speciellt basindex: använd det föregående pivotelementet. Giltigt för "Show Values As"-beräkningar; gäller i Excel 2010 och senare.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```


Representerar basfältet för en ShowDataAs-beräkning när ShowDataAs-beräkningen är i bruk.

**Returns:**
int
### getBaseFieldName() {#getBaseFieldName--}
```
public String getBaseFieldName()
```


Hämtar rubrik för pivots basfält.

**Returns:**
java.lang.String
### getBaseItemCaption() {#getBaseItemCaption--}
```
public String getBaseItemCaption()
```


Hämtar rubrik för pivotelementet i basfältet.

**Returns:**
java.lang.String
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```


Representerar det anpassade indexet för pivotelementet i basfältet när beräkningen ShowDataAs används.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Returns:**
int
### getBaseItemPositionType() {#getBaseItemPositionType--}
```
public int getBaseItemPositionType()
```


Representerar typen av baspivotelementet i basfältet när beräkningen ShowDataAs används. Eftersom PivotItemPosition.Custom endast är för läsning, om du behöver sätta PivotItemPosition.Custom, vänligen sätt attributet PivotField.BaseItemIndex.

Se [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotShowValuesSetting.BaseItem‑egenskapen. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getCalculationType() {#getCalculationType--}
```
public int getCalculationType()
```


Representerar hur värden i ett datafält visas i pivoterapporten.

Se [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotShowValuesSetting.ShowValuesAs‑egenskapen. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


Hämtar hur värden i ett datafält visas i pivoterapporten.

Se [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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


Representerar basfältet för en ShowDataAs-beräkning när ShowDataAs-beräkningen är i bruk.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


Representerar det anpassade indexet för pivotelementet i basfältet när beräkningen ShowDataAs används.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBaseItemPositionType(int value) {#setBaseItemPositionType-int-}
```
public void setBaseItemPositionType(int value)
```


Representerar typen av baspivotelementet i basfältet när beräkningen ShowDataAs används. Eftersom PivotItemPosition.Custom endast är för läsning, om du behöver sätta PivotItemPosition.Custom, vänligen sätt attributet PivotField.BaseItemIndex.

Se [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotShowValuesSetting.BaseItem‑egenskapen. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCalculationType(int value) {#setCalculationType-int-}
```
public void setCalculationType(int value)
```


Representerar hur värden i ett datafält visas i pivoterapporten.

Se [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället PivotShowValuesSetting.ShowValuesAs‑egenskapen. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShowValuesAs(int value) {#setShowValuesAs-int-}
```
public void setShowValuesAs(int value)
```


Ställer in hur värden i ett datafält visas i pivoterapporten.

Se [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

