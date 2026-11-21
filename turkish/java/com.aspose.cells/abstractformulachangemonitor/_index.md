---
title: "AbstractFormulaChangeMonitor"
second_title: "Aspose.Cells for Java API Referansı"
description: "Kullanıcının belirli işlemler sırasında formüllerin değişimini izleyebilmesi için izleme."
type: docs
url: /tr/java/com.aspose.cells/abstractformulachangemonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractFormulaChangeMonitor
```

Kullanıcının belirli işlemler sırasında formüllerin değişimini izleyebilmesi için izleme.

**Remarks**

Örneğin, hücre aralığını silerken/eklerken, referansların kayması nedeniyle diğer hücrelerin formülleri değişebilir. Lütfen, monitördeki yöntemlerin formülü içeren bir nesne için birden fazla kez çağrılabileceğini unutmayın.

**Example**

```
         class MyFormulaChangeMonitor extends AbstractFormulaChangeMonitor
         {
             private final WorksheetCollection mWorksheets;
             public MyFormulaChangeMonitor(WorksheetCollection worksheets)
             {
                 mWorksheets = worksheets;
             }
             public /*override*/ void onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
             {
                 System.out.println("Cell " + mWorksheets.get(sheetIndex).getName() + "!"
                     + CellsHelper.cellIndexToName(rowIndex, columnIndex)
                     + "'s formula was changed while inserting rows.");
             }
         }
         Workbook wb = new Workbook("template.xlsx");
         InsertOptions options = new InsertOptions();
         options.setFormulaChangeMonitor(new MyFormulaChangeMonitor(wb.getWorksheets()));
         wb.getWorksheets().get(0).getCells().insertRows(0, 2, options);
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AbstractFormulaChangeMonitor()](#AbstractFormulaChangeMonitor--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)](#onCellFormulaChanged-int-int-int-) | Bir hücredeki formül değiştiğinde tetiklenecek olay. |
| [onFormatConditionFormulaChanged(FormatCondition fc)](#onFormatConditionFormulaChanged-com.aspose.cells.FormatCondition-) | FormatCondition formülü değiştiğinde tetiklenecek olay. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractFormulaChangeMonitor() {#AbstractFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor()
```


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




### onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex) {#onCellFormulaChanged-int-int-int-}
```
public void onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```


Bir hücredeki formül değiştiğinde tetiklenecek olay.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | int | Değişen hücrenin sayfa indeksi |
| rowIndex | int | Değişen hücrenin satır indeksi |
| columnIndex | int | Değişen hücrenin sütun indeksi |

### onFormatConditionFormulaChanged(FormatCondition fc) {#onFormatConditionFormulaChanged-com.aspose.cells.FormatCondition-}
```
public void onFormatConditionFormulaChanged(FormatCondition fc)
```


FormatCondition formülü değiştiğinde tetiklenecek olay.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fc | [FormatCondition](../../com.aspose.cells/formatcondition) | Formülü değişen FormatCondition nesnesi |

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

