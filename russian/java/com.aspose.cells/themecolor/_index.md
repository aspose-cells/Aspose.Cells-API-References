---
title: "ThemeColor"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет цвет темы."
type: docs
url: /ru/java/com.aspose.cells/themecolor/
---

**Inheritance:**
java.lang.Object
```
public class ThemeColor
```

Представляет цвет темы.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").putValue("Hello World");
         Style style = cells.get("A1").getStyle();
         //Set ThemeColorType.Text2 color type with 40% lighten as the font color.
         style.getFont().setThemeColor(new ThemeColor(ThemeColorType.TEXT_2, 0.4));
         style.setPattern(BackgroundType.SOLID);
         //Set ThemeColorType.Background2 color type with 75% darken as the foreground color
         style.setForegroundThemeColor(new ThemeColor(ThemeColorType.BACKGROUND_2, -0.75));
         cells.get("A1").setStyle(style);
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ThemeColor(int type, double tint)](#ThemeColor-int-double-) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorType()](#getColorType--) | Получает тип темы. |
| [getTint()](#getTint--) | Получает значение тона. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColorType(int value)](#setColorType-int-) | Устанавливает тип темы. |
| [setTint(double value)](#setTint-double-) | Устанавливает значение тона. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThemeColor(int type, double tint) {#ThemeColor-int-double-}
```
public ThemeColor(int type, double tint)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Тип темы. |
| tint | double | Значение тона. |

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
### getColorType() {#getColorType--}
```
public int getColorType()
```


Получает тип темы.

См. [ThemeColorType](../../com.aspose.cells/themecolortype).

**Returns:**
int
### getTint() {#getTint--}
```
public double getTint()
```


Получает значение тона.

**Remarks**

Значение тона хранится как тип double от -1.0 до 1.0, где -1.0 означает 100 % затемнение, а 1.0 — 100 % осветление. Кроме того, 0.0 означает отсутствие изменений.

**Returns:**
double
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




### setColorType(int value) {#setColorType-int-}
```
public void setColorType(int value)
```


Устанавливает тип темы.

См. [ThemeColorType](../../com.aspose.cells/themecolortype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTint(double value) {#setTint-double-}
```
public void setTint(double value)
```


Устанавливает значение тона.

**Remarks**

Значение тона хранится как тип double от -1.0 до 1.0, где -1.0 означает 100 % затемнение, а 1.0 — 100 % осветление. Кроме того, 0.0 означает отсутствие изменений.

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

