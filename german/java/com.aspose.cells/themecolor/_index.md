---
title: "ThemeColor"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Designfarbe dar."
type: docs
url: /de/java/com.aspose.cells/themecolor/
---

**Inheritance:**
java.lang.Object
```
public class ThemeColor
```

Stellt eine Designfarbe dar.

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
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ThemeColor(int type, double tint)](#ThemeColor-int-double-) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorType()](#getColorType--) | Liefert den Theme-Typ. |
| [getTint()](#getTint--) | Liefert den Tönungswert. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColorType(int value)](#setColorType-int-) | Setzt den Theme-Typ. |
| [setTint(double value)](#setTint-double-) | Setzt den Tönungswert. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThemeColor(int type, double tint) {#ThemeColor-int-double-}
```
public ThemeColor(int type, double tint)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Der Theme-Typ. |
| Farbton | double | Der Farbtonwert. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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


Liefert den Theme-Typ.

Siehe [ThemeColorType](../../com.aspose.cells/themecolortype).

**Returns:**
int
### getTint() {#getTint--}
```
public double getTint()
```


Liefert den Tönungswert.

**Remarks**

Der Farbtonwert wird als double von -1.0 bis 1.0 gespeichert, wobei -1.0 100 % Abdunkeln und 1.0 100 % Aufhellen bedeutet. Außerdem bedeutet 0.0 keine Änderung.

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


Setzt den Theme-Typ.

Siehe [ThemeColorType](../../com.aspose.cells/themecolortype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTint(double value) {#setTint-double-}
```
public void setTint(double value)
```


Setzt den Tönungswert.

**Remarks**

Der Farbtonwert wird als double von -1.0 bis 1.0 gespeichert, wobei -1.0 100 % Abdunkeln und 1.0 100 % Aufhellen bedeutet. Außerdem bedeutet 0.0 keine Änderung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

