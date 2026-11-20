---
title: "FontSettingCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет список ."
type: docs
url: /ru/java/com.aspose.cells/fontsettingcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class FontSettingCollection extends CollectionBase
```

Представляет список [FontSetting](../../com.aspose.cells/fontsetting).
## Методы

| Метод | Описание |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [appendText(String text)](#appendText-java.lang.String-) | Добавляет текст. |
| [clear()](#clear--) | Очистить все настройки. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [deleteText(int index, int count)](#deleteText-int-int-) | Удалить некоторые символы. |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [format(int startIndex, int length, Font font, StyleFlag flag)](#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Форматировать текст с настройкой шрифта. |
| [get(int index)](#get-int-) | Получает [FontSetting](../../com.aspose.cells/fontsetting) по индексу. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [getHtmlString()](#getHtmlString--) | Получает строку html, содержащую данные и некоторые форматы в этой фигуре. |
| [getParagraphEnumerator()](#getParagraphEnumerator--) | Получает перечислитель абзацев. |
| [getText()](#getText--) | Получает текст фигуры. |
| [getTextAlignment()](#getTextAlignment--) | Представляет настройку выравнивания тела текста. |
| [getTextParagraphs()](#getTextParagraphs--) | Получает все абзацы. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | Вставить индекс в позицию. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Удаляет элемент по указанному индексу. |
| [replace(int index, int count, String text)](#replace-int-int-java.lang.String-) | Заменить текст. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Заменить текст. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Устанавливает строку html, содержащую данные и некоторые форматы в этой фигуре. |
| [setText(String value)](#setText-java.lang.String-) | Устанавливает текст фигуры. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Устанавливает предустановленный стиль WordArt. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Добавляет элемент в экземпляр CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Объект, который нужно добавить в экземпляр CollectionBase. |

**Returns:**
int — позиция, в которую был вставлен новый элемент.
### appendText(String text) {#appendText-java.lang.String-}
```
public void appendText(String text)
```


Добавляет текст.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | java.lang.String | Текст. |

### clear() {#clear--}
```
public void clear()
```


Очистить все настройки.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Возвращает, содержит ли экземпляр этот объект

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | тестовый объект |

**Returns:**
boolean — содержит ли экземпляр этот объект
### deleteText(int index, int count) {#deleteText-int-int-}
```
public void deleteText(int index, int count)
```


Удалить некоторые символы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Начальный индекс. |
| количество | int | Количество символов. |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### format(int startIndex, int length, Font font, StyleFlag flag) {#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void format(int startIndex, int length, Font font, StyleFlag flag)
```


Форматировать текст с настройкой шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | int | Начальный индекс. |
| length | int | Длина. |
| font | [Font](../../com.aspose.cells/font) | Шрифт. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Флаги шрифта. |

### get(int index) {#get-int-}
```
public FontSetting get(int index)
```


Получает [FontSetting](../../com.aspose.cells/fontsetting) по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Получает количество элементов, содержащихся в экземпляре CollectionBase.

**Returns:**
int — количество элементов, содержащихся в экземпляре CollectionBase.
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Получает строку html, содержащую данные и некоторые форматы в этой фигуре.

**Returns:**
java.lang.String
### getParagraphEnumerator() {#getParagraphEnumerator--}
```
public Iterator getParagraphEnumerator()
```


Получает перечислитель абзацев.

**Returns:**
java.util.Iterator -
### getText() {#getText--}
```
public String getText()
```


Получает текст фигуры.

**Returns:**
java.lang.String
### getTextAlignment() {#getTextAlignment--}
```
public ShapeTextAlignment getTextAlignment()
```


Представляет настройку выравнивания тела текста.

**Returns:**
[ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)
### getTextParagraphs() {#getTextParagraphs--}
```
public TextParagraphCollection getTextParagraphs()
```


Получает все абзацы.

**Returns:**
[TextParagraphCollection](../../com.aspose.cells/textparagraphcollection)
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int -
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Определяет индекс конкретного элемента в экземпляре CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Определяет индекс конкретного элемента в экземпляре CollectionBase. |

**Returns:**
int — индекс значения, если оно найдено в списке; иначе -1.
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


Вставить индекс в позицию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Начальный индекс. |
| текст | java.lang.String | Текст. |

### iterator() {#iterator--}
```
public Iterator iterator()
```


Возвращает перечислитель, который проходит по экземпляру CollectionBase.

**Returns:**
java.util.Iterator — итератор для экземпляра CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удаляет элемент по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс элемента, который нужно удалить. |

### replace(int index, int count, String text) {#replace-int-int-java.lang.String-}
```
public void replace(int index, int count, String text)
```


Заменить текст.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Начальный индекс. |
| количество | int | Количество символов. |
| текст | java.lang.String | Текст. |

### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public void replace(String oldValue, String newValue)
```


Заменить текст.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| oldValue | java.lang.String | Старый текст. |
| newValue | java.lang.String | Новый текст. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Устанавливает строку html, содержащую данные и некоторые форматы в этой фигуре.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Устанавливает текст фигуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Устанавливает предустановленный стиль WordArt.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Предустановленный стиль WordArt. |

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

