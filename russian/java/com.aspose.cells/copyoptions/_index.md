---
title: "CopyOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет параметры копирования."
type: docs
url: /ru/java/com.aspose.cells/copyoptions/
---

**Inheritance:**
java.lang.Object
```
public class CopyOptions
```

Представляет параметры копирования.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [CopyOptions()](#CopyOptions--) | Конструктор CopyOptions. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--) | Указывает, копировать ли ширину столбца в единицах символов. |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--) | Если формула недействительна для целевого назначения, копировать только значения. |
| [getCopyNames()](#getCopyNames--) | Указывает, копировать ли имена. |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--) | Указывает, расширять ли диапазоны при копировании диапазона в соседний диапазон. |
| [getKeepMacros()](#getKeepMacros--) | Указывает, сохраняются ли макросы; |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--) | При копировании диапазона в том же файле и когда диаграмма ссылается на исходный лист, False означает, что источник данных скопированной диаграммы не будет изменён. |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--) | В MS Excel при копировании формул, которые ссылаются на другие листы, во время копирования листа в другой, скопированные формулы должны ссылаться на исходную книгу. |
| [getUpdateInvalidReferencesToTargetSheet()](#getUpdateInvalidReferencesToTargetSheet--) | Указывает, следует ли ссылаться на целевой лист, если ссылка на лист не была скопирована. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColumnCharacterWidth(boolean value)](#setColumnCharacterWidth-boolean-) | Указывает, копировать ли ширину столбца в единицах символов. |
| [setCopyInvalidFormulasAsValues(boolean value)](#setCopyInvalidFormulasAsValues-boolean-) | Если формула недействительна для целевого назначения, копировать только значения. |
| [setCopyNames(boolean value)](#setCopyNames-boolean-) | Указывает, копировать ли имена. |
| [setExtendToAdjacentRange(boolean value)](#setExtendToAdjacentRange-boolean-) | Указывает, расширять ли диапазоны при копировании диапазона в соседний диапазон. |
| [setKeepMacros(boolean value)](#setKeepMacros-boolean-) | Указывает, сохраняются ли макросы; |
| [setReferToDestinationSheet(boolean value)](#setReferToDestinationSheet-boolean-) | При копировании диапазона в том же файле и когда диаграмма ссылается на исходный лист, False означает, что источник данных скопированной диаграммы не будет изменён. |
| [setReferToSheetWithSameName(boolean value)](#setReferToSheetWithSameName-boolean-) | В MS Excel при копировании формул, которые ссылаются на другие листы, во время копирования листа в другой, скопированные формулы должны ссылаться на исходную книгу. |
| [setUpdateInvalidReferencesToTargetSheet(boolean value)](#setUpdateInvalidReferencesToTargetSheet-boolean-) | Указывает, следует ли ссылаться на целевой лист, если ссылка на лист не была скопирована. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CopyOptions() {#CopyOptions--}
```
public CopyOptions()
```


Конструктор CopyOptions.

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
### getColumnCharacterWidth() {#getColumnCharacterWidth--}
```
public boolean getColumnCharacterWidth()
```


Указывает, копировать ли ширину столбца в единицах символов.

**Returns:**
boolean
### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}
```
public boolean getCopyInvalidFormulasAsValues()
```


Если формула недействительна для целевого назначения, копировать только значения.

**Returns:**
boolean
### getCopyNames() {#getCopyNames--}
```
public boolean getCopyNames()
```


Указывает, копировать ли имена.

**Returns:**
boolean
### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}
```
public boolean getExtendToAdjacentRange()
```


Указывает, расширять ли диапазоны при копировании диапазона в соседний диапазон.

**Remarks**

Если значение true, то только расширяется диапазон гиперссылки, без добавления новой гиперссылки при копировании гиперссылок в соседние строки.

**Returns:**
boolean
### getKeepMacros() {#getKeepMacros--}
```
public boolean getKeepMacros()
```


Указывает, сохраняются ли макросы;

**Remarks**

Только при копировании книги.

**Returns:**
boolean
### getReferToDestinationSheet() {#getReferToDestinationSheet--}
```
public boolean getReferToDestinationSheet()
```


При копировании диапазона в том же файле и когда диаграмма ссылается на исходный лист, False означает, что источник данных скопированной диаграммы не будет изменён. True означает, что источник данных скопированной диаграммы ссылается на лист назначения.

**Remarks**

Значение по умолчанию — false, работает как в MS Excel. Например: при копировании диаграммы с источником данных "sheet1!A1:B10" с листа "sheet1" в другой лист "sheet2", источник данных будет изменён на "sheet2!A1:B10".

**Returns:**
boolean
### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}
```
public boolean getReferToSheetWithSameName()
```


В MS Excel при копировании формул, которые ссылаются на другие листы, во время копирования листа в другой, скопированные формулы должны ссылаться на исходную книгу. Однако в некоторых ситуациях пользователю может потребоваться, чтобы скопированные формулы ссылались на листы с тем же именем в той же книге, например когда эти листы уже были скопированы до этой операции копирования; тогда это свойство должно быть установлено в true.

**Remarks**

Значение по умолчанию — true.

**Returns:**
boolean
### getUpdateInvalidReferencesToTargetSheet() {#getUpdateInvalidReferencesToTargetSheet--}
```
public boolean getUpdateInvalidReferencesToTargetSheet()
```


Указывает, следует ли ссылаться на целевой лист, если ссылка на лист не была скопирована.

**Remarks**

Работает только при копировании диапазона или листа из другой книги.

**Returns:**
boolean
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




### setColumnCharacterWidth(boolean value) {#setColumnCharacterWidth-boolean-}
```
public void setColumnCharacterWidth(boolean value)
```


Указывает, копировать ли ширину столбца в единицах символов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCopyInvalidFormulasAsValues(boolean value) {#setCopyInvalidFormulasAsValues-boolean-}
```
public void setCopyInvalidFormulasAsValues(boolean value)
```


Если формула недействительна для целевого назначения, копировать только значения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setCopyNames(boolean value) {#setCopyNames-boolean-}
```
public void setCopyNames(boolean value)
```


Указывает, копировать ли имена.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setExtendToAdjacentRange(boolean value) {#setExtendToAdjacentRange-boolean-}
```
public void setExtendToAdjacentRange(boolean value)
```


Указывает, расширять ли диапазоны при копировании диапазона в соседний диапазон.

**Remarks**

Если значение true, то только расширяется диапазон гиперссылки, без добавления новой гиперссылки при копировании гиперссылок в соседние строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setKeepMacros(boolean value) {#setKeepMacros-boolean-}
```
public void setKeepMacros(boolean value)
```


Указывает, сохраняются ли макросы;

**Remarks**

Только при копировании книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setReferToDestinationSheet(boolean value) {#setReferToDestinationSheet-boolean-}
```
public void setReferToDestinationSheet(boolean value)
```


При копировании диапазона в том же файле и когда диаграмма ссылается на исходный лист, False означает, что источник данных скопированной диаграммы не будет изменён. True означает, что источник данных скопированной диаграммы ссылается на лист назначения.

**Remarks**

Значение по умолчанию — false, работает как в MS Excel. Например: при копировании диаграммы с источником данных "sheet1!A1:B10" с листа "sheet1" в другой лист "sheet2", источник данных будет изменён на "sheet2!A1:B10".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setReferToSheetWithSameName(boolean value) {#setReferToSheetWithSameName-boolean-}
```
public void setReferToSheetWithSameName(boolean value)
```


В MS Excel при копировании формул, которые ссылаются на другие листы, во время копирования листа в другой, скопированные формулы должны ссылаться на исходную книгу. Однако в некоторых ситуациях пользователю может потребоваться, чтобы скопированные формулы ссылались на листы с тем же именем в той же книге, например когда эти листы уже были скопированы до этой операции копирования; тогда это свойство должно быть установлено в true.

**Remarks**

Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setUpdateInvalidReferencesToTargetSheet(boolean value) {#setUpdateInvalidReferencesToTargetSheet-boolean-}
```
public void setUpdateInvalidReferencesToTargetSheet(boolean value)
```


Указывает, следует ли ссылаться на целевой лист, если ссылка на лист не была скопирована.

**Remarks**

Работает только при копировании диапазона или листа из другой книги.

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

