---
title: "DefaultStyleSettings"
second_title: "Справочник API Aspose.Cells for Java"
description: "Настройки значений по умолчанию свойств стилей книг."
type: docs
url: /ru/java/com.aspose.cells/defaultstylesettings/
---

**Inheritance:**
java.lang.Object
```
public class DefaultStyleSettings
```

Настройки значений по умолчанию свойств стилей книги.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInPreference()](#getBuiltInPreference--) | Указывает, предпочтительно ли свойство формата числа, когда стиль определяет как встроенный номер, так и пользовательский шаблон. |
| [getClass()](#getClass--) |  |
| [getFontName()](#getFontName--) | Получает имя шрифта по умолчанию для книги |
| [getFontSize()](#getFontSize--) | Получает стандартный размер шрифта по умолчанию для книги. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Получает значение по умолчанию для горизонтального выравнивания |
| [getVerticalAlignment()](#getVerticalAlignment--) | Получает значение по умолчанию для вертикального выравнивания |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuiltInPreference(boolean value)](#setBuiltInPreference-boolean-) | Указывает, предпочтительно ли свойство формата числа, когда стиль определяет как встроенный номер, так и пользовательский шаблон. |
| [setFontName(String value)](#setFontName-java.lang.String-) | Устанавливает имя шрифта по умолчанию для рабочей книги |
| [setFontSize(double value)](#setFontSize-double-) | Устанавливает стандартный размер шрифта по умолчанию для рабочей книги. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Устанавливает значение по умолчанию для горизонтального выравнивания |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Устанавливает значение по умолчанию для вертикального выравнивания |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getBuiltInPreference() {#getBuiltInPreference--}
```
public boolean getBuiltInPreference()
```


Указывает, предпочтительно ли свойство формата числа, когда стиль определяет как встроенный числовой формат, так и пользовательский шаблон. Значение по умолчанию — false, что означает, что по умолчанию будет использоваться пользовательский шаблон для форматирования значений, если он не пуст для данного стиля.

**Remarks**

При загрузке рабочей книги из существующего шаблонного файла могут быть определены как встроенный числовой формат, так и пользовательский шаблон для одного стиля. Это свойство определяет, следует ли использовать встроенный числовой формат или пользовательский шаблон при форматировании значений с этим стилем.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontName() {#getFontName--}
```
public String getFontName()
```


Получает имя шрифта по умолчанию для книги

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Получает стандартный размер шрифта по умолчанию для книги.

**Returns:**
double
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Получает значение по умолчанию для горизонтального выравнивания

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Получает значение по умолчанию для вертикального выравнивания

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

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




### setBuiltInPreference(boolean value) {#setBuiltInPreference-boolean-}
```
public void setBuiltInPreference(boolean value)
```


Указывает, предпочтительно ли свойство формата числа, когда стиль определяет как встроенный числовой формат, так и пользовательский шаблон. Значение по умолчанию — false, что означает, что по умолчанию будет использоваться пользовательский шаблон для форматирования значений, если он не пуст для данного стиля.

**Remarks**

При загрузке рабочей книги из существующего шаблонного файла могут быть определены как встроенный числовой формат, так и пользовательский шаблон для одного стиля. Это свойство определяет, следует ли использовать встроенный числовой формат или пользовательский шаблон при форматировании значений с этим стилем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


Устанавливает имя шрифта по умолчанию для рабочей книги

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFontSize(double value) {#setFontSize-double-}
```
public void setFontSize(double value)
```


Устанавливает стандартный размер шрифта по умолчанию для рабочей книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Устанавливает значение по умолчанию для горизонтального выравнивания

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Устанавливает значение по умолчанию для вертикального выравнивания

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

