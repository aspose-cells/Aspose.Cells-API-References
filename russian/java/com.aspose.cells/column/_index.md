---
title: "Column"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет отдельный столбец в листе."
type: docs
url: /ru/java/com.aspose.cells/column/
---

**Inheritance:**
java.lang.Object
```
public class Column
```

Представляет отдельный столбец в листе.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
         //Get first Column
         Column column = worksheet.getCells().getColumns().get(0);
 
         //Apply Style to first Column
         column.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Применяет форматы ко всему столбцу. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getGroupLevel()](#getGroupLevel--) | Получает уровень группы столбца. |
| [getIndex()](#getIndex--) | Получает индекс этого столбца. |
| [getStyle()](#getStyle--) | Получает стиль этого столбца. |
| [getWidth()](#getWidth--) | Получает ширину столбца в единицах символов. |
| [hasCustomStyle()](#hasCustomStyle--) | Указывает, имеет ли этот столбец пользовательские настройки стиля (отличные от стиля по умолчанию, наследуемого из книги). |
| [hashCode()](#hashCode--) |  |
| [isCollapsed()](#isCollapsed--) | является ли столбец свернутым |
| [isHidden()](#isHidden--) | Указывает, скрыт ли столбец. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | является ли столбец свернутым |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Получает уровень группы столбца. |
| [setHidden(boolean value)](#setHidden-boolean-) | Указывает, скрыт ли столбец. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Устанавливает стиль этого столбца. |
| [setWidth(double value)](#setWidth-double-) | Устанавливает ширину столбца в единицах символов. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Применяет форматы ко всему столбцу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Объект стиля, который будет применён. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Флаги, указывающие применённые свойства форматирования. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
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
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Получает уровень группы столбца.

**Returns:**
byte
### getIndex() {#getIndex--}
```
public int getIndex()
```


Получает индекс этого столбца.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Получает стиль этого столбца.

**Remarks**

Изменение возвращаемого объекта стиля напрямую не оказывает влияния на этот столбец или любые ячейки в этом столбце. Необходимо вызвать метод [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-) или [setStyle(Style)](../../com.aspose.cells/column\#setStyle-Style-) для применения изменения к этому столбцу.

Стиль столбца — это стиль, который будет наследоваться ячейками в этом столбце (те ячейки, у которых нет пользовательских настроек стиля, такие как существующие ячейки, для которых стиль не был установлен явно, или те, которые еще не созданы).

**Returns:**
[Style](../../com.aspose.cells/style)
### getWidth() {#getWidth--}
```
public double getWidth()
```


Получает ширину столбца в единицах символов.

**Remarks**

Для электронных таблиц ширина столбца измеряется в количестве символов максимальной ширины цифр 0~9, отображаемых шрифтом обычного стиля.

**Returns:**
double
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Указывает, имеет ли этот столбец пользовательские настройки стиля (отличные от стиля по умолчанию, наследуемого из книги).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


является ли столбец свернутым

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Указывает, скрыт ли столбец.

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




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


является ли столбец свернутым

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Получает уровень группы столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Указывает, скрыт ли столбец.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Устанавливает стиль этого столбца.

**Remarks**

Этот метод только задает указанный стиль в качестве стиля по умолчанию для этого столбца, не изменяя настройки стиля для существующих ячеек в этом столбце. Чтобы одновременно обновить настройки стиля существующих ячеек до указанного стиля, пожалуйста, используйте [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\\#applyStyle-Style-StyleFlag-)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | стиль, который будет использоваться в качестве стиля по умолчанию для ячеек в этом столбце. |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Устанавливает ширину столбца в единицах символов.

**Remarks**

Для электронных таблиц ширина столбца измеряется в количестве символов максимальной ширины цифр 0~9, отображаемых шрифтом обычного стиля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

