---
title: "ThemeColor"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir tema rengini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/themecolor/
---

**Inheritance:**
java.lang.Object
```
public class ThemeColor
```

Bir tema rengini temsil eder.

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
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ThemeColor(int type, double tint)](#ThemeColor-int-double-) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorType()](#getColorType--) | Tema tipini alır. |
| [getTint()](#getTint--) | Renk tonu değerini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColorType(int value)](#setColorType-int-) | Tema tipini ayarlar. |
| [setTint(double value)](#setTint-double-) | Renk tonu değerini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThemeColor(int type, double tint) {#ThemeColor-int-double-}
```
public ThemeColor(int type, double tint)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Tema tipi. |
| tint | double | Renk tonu değeri. |

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
### getColorType() {#getColorType--}
```
public int getColorType()
```


Tema tipini alır.

Bakınız [ThemeColorType](../../com.aspose.cells/themecolortype).

**Returns:**
int
### getTint() {#getTint--}
```
public double getTint()
```


Renk tonu değerini alır.

**Remarks**

Renk tonu değeri -1.0 ile 1.0 arasında bir double olarak saklanır; -1.0 %100 karartma, 1.0 %100 aydınlatma anlamına gelir. Ayrıca, 0.0 değişiklik olmadığını gösterir.

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


Tema tipini ayarlar.

Bakınız [ThemeColorType](../../com.aspose.cells/themecolortype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setTint(double value) {#setTint-double-}
```
public void setTint(double value)
```


Renk tonu değerini ayarlar.

**Remarks**

Renk tonu değeri -1.0 ile 1.0 arasında bir double olarak saklanır; -1.0 %100 karartma, 1.0 %100 aydınlatma anlamına gelir. Ayrıca, 0.0 değişiklik olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

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

