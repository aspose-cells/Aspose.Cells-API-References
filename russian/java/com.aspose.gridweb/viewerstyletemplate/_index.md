---
title: "ViewerStyleTemplate"
second_title: "Справочник API Aspose.Cells for Java"
description: "ViewerStyleTemplate."
type: docs
url: /ru/java/com.aspose.gridweb/viewerstyletemplate/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class ViewerStyleTemplate extends Control
```

ViewerStyleTemplate.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ViewerStyleTemplate()](#ViewerStyleTemplate--) | Конструктор по умолчанию. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActiveCellBgColor()](#getActiveCellBgColor--) | Задает цвет фона активной ячейки. |
| [getActiveCellColor()](#getActiveCellColor--) | Задает цвет активной ячейки. |
| [getActiveHeaderBgColor()](#getActiveHeaderBgColor--) | Задает цвет фона активного заголовка строки/столбца. |
| [getActiveHeaderColor()](#getActiveHeaderColor--) | Задает цвет активного заголовка строки/столбца. |
| [getActiveTabStyle()](#getActiveTabStyle--) |  |
| [getBottomTableStyle()](#getBottomTableStyle--) |  |
| [getClass()](#getClass--) |  |
| [getDefaultGridLineColor()](#getDefaultGridLineColor--) |  |
| [getFrameTableStyle()](#getFrameTableStyle--) |  |
| [getHeaderBarHeight()](#getHeaderBarHeight--) |  |
| [getHeaderBarStyle()](#getHeaderBarStyle--) |  |
| [getHeaderBarTableStyle()](#getHeaderBarTableStyle--) |  |
| [getHeaderBarWidth()](#getHeaderBarWidth--) |  |
| [getScrollBarArrowColor()](#getScrollBarArrowColor--) |  |
| [getScrollBarBaseColor()](#getScrollBarBaseColor--) |  |
| [getSelectCellBgColor()](#getSelectCellBgColor--) | Указывает цвет фона выбранных ячеек в диапазоне множественного выбора. |
| [getSelectCellColor()](#getSelectCellColor--) | Указывает цвет выбранных ячеек в диапазоне множественного выбора. |
| [getStylesFromControl(MainWeb control)](#getStylesFromControl-com.aspose.gridweb.MainWeb-) |  |
| [getTabStyle()](#getTabStyle--) |  |
| [getUniqueID()](#getUniqueID--) | Получает UniqueID в элементе управления. |
| [getViewTableStyle()](#getViewTableStyle--) |  |
| [getVisible()](#getVisible--) | Получает свойство Visible в Control |
| [hashCode()](#hashCode--) |  |
| [loadPresetStyle(int presetStyle)](#loadPresetStyle-int-) | Загрузить предустановленный стиль. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parseFromFile(String fileName)](#parseFromFile-java.lang.String-) |  |
| [parseFromString(String xmlStr)](#parseFromString-java.lang.String-) |  |
| [persistToFile(String fileName)](#persistToFile-java.lang.String-) |  |
| [persistToString()](#persistToString--) |  |
| [setActiveCellBgColor(Color value)](#setActiveCellBgColor-com.aspose.gridweb.Color-) | Задает цвет фона активной ячейки. |
| [setActiveCellColor(Color value)](#setActiveCellColor-com.aspose.gridweb.Color-) | Задает цвет активной ячейки. |
| [setActiveHeaderBgColor(Color value)](#setActiveHeaderBgColor-com.aspose.gridweb.Color-) | Задает цвет фона активного заголовка строки/столбца. |
| [setActiveHeaderColor(Color value)](#setActiveHeaderColor-com.aspose.gridweb.Color-) | Задает цвет активного заголовка строки/столбца. |
| [setActiveTabStyle(GridTableItemStyle value)](#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-) |  |
| [setBottomTableStyle(GridTableStyle value)](#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-) |  |
| [setDefaultGridLineColor(Color value)](#setDefaultGridLineColor-com.aspose.gridweb.Color-) |  |
| [setFrameTableStyle(GridTableStyle value)](#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-) |  |
| [setHeaderBarHeight(Unit value)](#setHeaderBarHeight-com.aspose.gridweb.Unit-) |  |
| [setHeaderBarStyle(GridTableItemStyle value)](#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-) |  |
| [setHeaderBarTableStyle(GridTableStyle value)](#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-) |  |
| [setHeaderBarWidth(Unit value)](#setHeaderBarWidth-com.aspose.gridweb.Unit-) |  |
| [setScrollBarArrowColor(Color value)](#setScrollBarArrowColor-com.aspose.gridweb.Color-) |  |
| [setScrollBarBaseColor(Color value)](#setScrollBarBaseColor-com.aspose.gridweb.Color-) |  |
| [setSelectCellBgColor(Color value)](#setSelectCellBgColor-com.aspose.gridweb.Color-) | Указывает цвет фона выбранных ячеек в диапазоне множественного выбора. |
| [setSelectCellColor(Color value)](#setSelectCellColor-com.aspose.gridweb.Color-) | Указывает цвет выбранных ячеек в диапазоне множественного выбора. |
| [setStylesForControl(MainWeb control)](#setStylesForControl-com.aspose.gridweb.MainWeb-) |  |
| [setTabStyle(GridTableItemStyle value)](#setTabStyle-com.aspose.gridweb.GridTableItemStyle-) |  |
| [setViewTableStyle(GridTableStyle value)](#setViewTableStyle-com.aspose.gridweb.GridTableStyle-) |  |
| [setVisible(boolean value)](#setVisible-boolean-) | Устанавливает свойство Visible в Control |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ViewerStyleTemplate() {#ViewerStyleTemplate--}
```
public ViewerStyleTemplate()
```


Конструктор по умолчанию.

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
### getActiveCellBgColor() {#getActiveCellBgColor--}
```
public Color getActiveCellBgColor()
```


Задает цвет фона активной ячейки.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveCellColor() {#getActiveCellColor--}
```
public Color getActiveCellColor()
```


Задает цвет активной ячейки.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderBgColor() {#getActiveHeaderBgColor--}
```
public Color getActiveHeaderBgColor()
```


Задает цвет фона активного заголовка строки/столбца.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderColor() {#getActiveHeaderColor--}
```
public Color getActiveHeaderColor()
```


Задает цвет активного заголовка строки/столбца.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveTabStyle() {#getActiveTabStyle--}
```
public GridTableItemStyle getActiveTabStyle()
```




**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getBottomTableStyle() {#getBottomTableStyle--}
```
public GridTableStyle getBottomTableStyle()
```




**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultGridLineColor() {#getDefaultGridLineColor--}
```
public Color getDefaultGridLineColor()
```




**Returns:**
[Color](../../com.aspose.gridweb/color)
### getFrameTableStyle() {#getFrameTableStyle--}
```
public GridTableStyle getFrameTableStyle()
```




**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getHeaderBarHeight() {#getHeaderBarHeight--}
```
public Unit getHeaderBarHeight()
```




**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeaderBarStyle() {#getHeaderBarStyle--}
```
public GridTableItemStyle getHeaderBarStyle()
```




**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getHeaderBarTableStyle() {#getHeaderBarTableStyle--}
```
public GridTableStyle getHeaderBarTableStyle()
```




**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getHeaderBarWidth() {#getHeaderBarWidth--}
```
public Unit getHeaderBarWidth()
```




**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getScrollBarArrowColor() {#getScrollBarArrowColor--}
```
public Color getScrollBarArrowColor()
```




**Returns:**
[Color](../../com.aspose.gridweb/color)
### getScrollBarBaseColor() {#getScrollBarBaseColor--}
```
public Color getScrollBarBaseColor()
```




**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellBgColor() {#getSelectCellBgColor--}
```
public Color getSelectCellBgColor()
```


Указывает цвет фона выбранных ячеек в диапазоне множественного выбора.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellColor() {#getSelectCellColor--}
```
public Color getSelectCellColor()
```


Указывает цвет выбранных ячеек в диапазоне множественного выбора.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getStylesFromControl(MainWeb control) {#getStylesFromControl-com.aspose.gridweb.MainWeb-}
```
public void getStylesFromControl(MainWeb control)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| control | [MainWeb](../../com.aspose.gridweb/mainweb) |  |

### getTabStyle() {#getTabStyle--}
```
public GridTableItemStyle getTabStyle()
```




**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Получает UniqueID в элементе управления.

**Returns:**
java.lang.String
### getViewTableStyle() {#getViewTableStyle--}
```
public GridTableStyle getViewTableStyle()
```




**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Получает свойство Visible в Control

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### loadPresetStyle(int presetStyle) {#loadPresetStyle-int-}
```
public void loadPresetStyle(int presetStyle)
```


Загрузить предустановленный стиль.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| presetStyle | int | [PresetStyle](../../com.aspose.gridweb/presetstyle). |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### parseFromFile(String fileName) {#parseFromFile-java.lang.String-}
```
public void parseFromFile(String fileName)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String |  |

### parseFromString(String xmlStr) {#parseFromString-java.lang.String-}
```
public void parseFromString(String xmlStr)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| xmlStr | java.lang.String |  |

### persistToFile(String fileName) {#persistToFile-java.lang.String-}
```
public void persistToFile(String fileName)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String |  |

### persistToString() {#persistToString--}
```
public String persistToString()
```




**Returns:**
java.lang.String -
### setActiveCellBgColor(Color value) {#setActiveCellBgColor-com.aspose.gridweb.Color-}
```
public void setActiveCellBgColor(Color value)
```


Задает цвет фона активной ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveCellColor(Color value) {#setActiveCellColor-com.aspose.gridweb.Color-}
```
public void setActiveCellColor(Color value)
```


Задает цвет активной ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderBgColor(Color value) {#setActiveHeaderBgColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderBgColor(Color value)
```


Задает цвет фона активного заголовка строки/столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderColor(Color value) {#setActiveHeaderColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderColor(Color value)
```


Задает цвет активного заголовка строки/столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveTabStyle(GridTableItemStyle value) {#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setActiveTabStyle(GridTableItemStyle value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setBottomTableStyle(GridTableStyle value) {#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setBottomTableStyle(GridTableStyle value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setDefaultGridLineColor(Color value) {#setDefaultGridLineColor-com.aspose.gridweb.Color-}
```
public void setDefaultGridLineColor(Color value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setFrameTableStyle(GridTableStyle value) {#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setFrameTableStyle(GridTableStyle value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setHeaderBarHeight(Unit value) {#setHeaderBarHeight-com.aspose.gridweb.Unit-}
```
public void setHeaderBarHeight(Unit value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeaderBarStyle(GridTableItemStyle value) {#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setHeaderBarStyle(GridTableItemStyle value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setHeaderBarTableStyle(GridTableStyle value) {#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setHeaderBarTableStyle(GridTableStyle value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setHeaderBarWidth(Unit value) {#setHeaderBarWidth-com.aspose.gridweb.Unit-}
```
public void setHeaderBarWidth(Unit value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setScrollBarArrowColor(Color value) {#setScrollBarArrowColor-com.aspose.gridweb.Color-}
```
public void setScrollBarArrowColor(Color value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setScrollBarBaseColor(Color value) {#setScrollBarBaseColor-com.aspose.gridweb.Color-}
```
public void setScrollBarBaseColor(Color value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellBgColor(Color value) {#setSelectCellBgColor-com.aspose.gridweb.Color-}
```
public void setSelectCellBgColor(Color value)
```


Указывает цвет фона выбранных ячеек в диапазоне множественного выбора.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellColor(Color value) {#setSelectCellColor-com.aspose.gridweb.Color-}
```
public void setSelectCellColor(Color value)
```


Указывает цвет выбранных ячеек в диапазоне множественного выбора.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setStylesForControl(MainWeb control) {#setStylesForControl-com.aspose.gridweb.MainWeb-}
```
public void setStylesForControl(MainWeb control)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| control | [MainWeb](../../com.aspose.gridweb/mainweb) |  |

### setTabStyle(GridTableItemStyle value) {#setTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setTabStyle(GridTableItemStyle value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setViewTableStyle(GridTableStyle value) {#setViewTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setViewTableStyle(GridTableStyle value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Устанавливает свойство Visible в Control

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

