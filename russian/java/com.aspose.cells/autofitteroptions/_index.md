---
title: "AutoFitterOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет все параметры автоподгонки."
type: docs
url: /ru/java/com.aspose.cells/autofitteroptions/
---

**Inheritance:**
java.lang.Object
```
public class AutoFitterOptions
```

Представляет все параметры автоподгонки.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AutoFitterOptions()](#AutoFitterOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitMergedCells()](#getAutoFitMergedCells--) | Указывает, следует ли автоматически подгонять высоту строки, когда ячейки объединены в строке. |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--) | Получает тип автоматической подгонки высоты строки объединённых ячеек. |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--) | Получает тип автоматической подгонки перенесённого текста. |
| [getClass()](#getClass--) |  |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Получает язык редактирования по умолчанию. |
| [getForRendering()](#getForRendering--) | Указывает, следует ли подгонка для целей рендеринга. |
| [getFormatStrategy()](#getFormatStrategy--) | Получает стратегию форматирования. |
| [getIgnoreHidden()](#getIgnoreHidden--) | Игнорирует скрытые строки/столбцы. |
| [getMaxRowHeight()](#getMaxRowHeight--) | Получает максимальную высоту строки (в единицах Point) при автоматической подгонке строк. |
| [getOnlyAuto()](#getOnlyAuto--) | Указывает, следует ли подгонять только те строки, высота которых не настроена вручную. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitMergedCells(boolean value)](#setAutoFitMergedCells-boolean-) | Указывает, следует ли автоматически подгонять высоту строки, когда ячейки объединены в строке. |
| [setAutoFitMergedCellsType(int value)](#setAutoFitMergedCellsType-int-) | Устанавливает тип автоматической подгонки высоты строк объединённых ячеек. |
| [setAutoFitWrappedTextType(int value)](#setAutoFitWrappedTextType-int-) | Устанавливает тип автоматической подгонки перенесённого текста. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Устанавливает язык редактирования по умолчанию. |
| [setForRendering(boolean value)](#setForRendering-boolean-) | Указывает, следует ли подгонка для целей рендеринга. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Устанавливает стратегию форматирования. |
| [setIgnoreHidden(boolean value)](#setIgnoreHidden-boolean-) | Игнорирует скрытые строки/столбцы. |
| [setMaxRowHeight(double value)](#setMaxRowHeight-double-) | Устанавливает максимальную высоту строки (в единицах Point) при автоматической подгонке строк. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Указывает, следует ли подгонять только те строки, высота которых не настроена вручную. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AutoFitterOptions() {#AutoFitterOptions--}
```
public AutoFitterOptions()
```


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
### getAutoFitMergedCells() {#getAutoFitMergedCells--}
```
public boolean getAutoFitMergedCells()
```


Указывает, следует ли автоматически подгонять высоту строки, когда ячейки объединены в строке. Значение по умолчанию — false.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство AutoFitterOptions.AutoFitMergedCellsType. Это свойство будет удалено через 12 месяцев, начиная с декабря 2018 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}
```
public int getAutoFitMergedCellsType()
```


Получает тип автоматической подгонки высоты строки объединённых ячеек.

Смотрите [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel по умолчанию игнорирует объединённые ячейки при подгонке высоты строки, поэтому Aspose.Cells работает как стандарт Excel. Пожалуйста, установите этот тип, чтобы изменить способ автоматической подгонки высоты строки объединённых ячеек.

**Returns:**
int
### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}
```
public int getAutoFitWrappedTextType()
```


Получает тип автоматической подгонки перенесённого текста.

Смотрите [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Получает язык редактирования по умолчанию.

См. [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Это может отображать/рендерить разные макеты абзацев текста при установленном различном языке редактирования. По умолчанию — [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getForRendering() {#getForRendering--}
```
public boolean getForRendering()
```


Указывает, следует ли подгонка для целей рендеринга.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Получает стратегию форматирования.

См. [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Значение по умолчанию — CellStyle для повышения производительности.

**Returns:**
int
### getIgnoreHidden() {#getIgnoreHidden--}
```
public boolean getIgnoreHidden()
```


Игнорирует скрытые строки/столбцы.

**Returns:**
boolean
### getMaxRowHeight() {#getMaxRowHeight--}
```
public double getMaxRowHeight()
```


Получает максимальную высоту строки (в единицах Point) при автоматической подгонке строк.

**Returns:**
double
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Указывает, следует ли подгонять только те строки, высота которых не настроена вручную.

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




### setAutoFitMergedCells(boolean value) {#setAutoFitMergedCells-boolean-}
```
public void setAutoFitMergedCells(boolean value)
```


Указывает, следует ли автоматически подгонять высоту строки, когда ячейки объединены в строке. Значение по умолчанию — false.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство AutoFitterOptions.AutoFitMergedCellsType. Это свойство будет удалено через 12 месяцев, начиная с декабря 2018 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoFitMergedCellsType(int value) {#setAutoFitMergedCellsType-int-}
```
public void setAutoFitMergedCellsType(int value)
```


Устанавливает тип автоматической подгонки высоты строк объединённых ячеек.

Смотрите [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).

**Remarks**

Excel по умолчанию игнорирует объединённые ячейки при подгонке высоты строки, поэтому Aspose.Cells работает как стандарт Excel. Пожалуйста, установите этот тип, чтобы изменить способ автоматической подгонки высоты строки объединённых ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setAutoFitWrappedTextType(int value) {#setAutoFitWrappedTextType-int-}
```
public void setAutoFitWrappedTextType(int value)
```


Устанавливает тип автоматической подгонки перенесённого текста.

Смотрите [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Устанавливает язык редактирования по умолчанию.

См. [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Это может отображать/рендерить разные макеты абзацев текста при установленном различном языке редактирования. По умолчанию — [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setForRendering(boolean value) {#setForRendering-boolean-}
```
public void setForRendering(boolean value)
```


Указывает, следует ли подгонка для целей рендеринга.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Устанавливает стратегию форматирования.

См. [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).

**Remarks**

Значение по умолчанию — CellStyle для повышения производительности.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setIgnoreHidden(boolean value) {#setIgnoreHidden-boolean-}
```
public void setIgnoreHidden(boolean value)
```


Игнорирует скрытые строки/столбцы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMaxRowHeight(double value) {#setMaxRowHeight-double-}
```
public void setMaxRowHeight(double value)
```


Устанавливает максимальную высоту строки (в единицах Point) при автоматической подгонке строк.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Указывает, следует ли подгонять только те строки, высота которых не настроена вручную.

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

