---
title: "ThemeColor"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل لونًا من السمة."
type: docs
url: /ar/java/com.aspose.cells/themecolor/
---

**Inheritance:**
java.lang.Object
```
public class ThemeColor
```

يمثل لونًا من السمة.

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
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ThemeColor(int type, double tint)](#ThemeColor-int-double-) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorType()](#getColorType--) | يحصل على نوع السمة. |
| [getTint()](#getTint--) | يحصل على قيمة الصبغة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColorType(int value)](#setColorType-int-) | يضبط نوع السمة. |
| [setTint(double value)](#setTint-double-) | يضبط قيمة الصبغة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThemeColor(int type, double tint) {#ThemeColor-int-double-}
```
public ThemeColor(int type, double tint)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). نوع السمة. |
| tint | double | قيمة الصبغة. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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


يحصل على نوع السمة.

انظر [ThemeColorType](../../com.aspose.cells/themecolortype).

**Returns:**
int
### getTint() {#getTint--}
```
public double getTint()
```


يحصل على قيمة الصبغة.

**Remarks**

يتم تخزين قيمة الصبغة كعدد مزدوج من -1.0 إلى 1.0، حيث يعني -1.0 تعتيمًا بنسبة 100٪ و 1.0 يعني إضاءةً بنسبة 100٪. كما أن 0.0 يعني عدم تغيير.

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


يضبط نوع السمة.

انظر [ThemeColorType](../../com.aspose.cells/themecolortype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTint(double value) {#setTint-double-}
```
public void setTint(double value)
```


يضبط قيمة الصبغة.

**Remarks**

يتم تخزين قيمة الصبغة كعدد مزدوج من -1.0 إلى 1.0، حيث يعني -1.0 تعتيمًا بنسبة 100٪ و 1.0 يعني إضاءةً بنسبة 100٪. كما أن 0.0 يعني عدم تغيير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

