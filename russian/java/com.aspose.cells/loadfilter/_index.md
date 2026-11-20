---
title: "LoadFilter"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет фильтр, предоставляющий параметры загрузки данных при загрузке книги из шаблона."
type: docs
url: /ru/java/com.aspose.cells/loadfilter/
---

**Inheritance:**
java.lang.Object
```
public class LoadFilter
```

Представляет фильтр, предоставляющий параметры загрузки данных при загрузке книги из шаблона.

**Remarks**

Пользователь может указать параметры фильтра или реализовать собственный LoadFilter, чтобы задать, как загружать данные.

**Example**

В следующем примере показано, как определить параметры фильтра в соответствии со свойствами листа.

```
         class LoadFilterSheet extends LoadFilter
         {
             public /*override*/ void startSheet(Worksheet sheet) 
             {
                 if ("Sheet1".equals(sheet.getName()))
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.ALL);
                 }
                 else
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.STRUCTURE);
                 }
             }
         }
         LoadOptions opts = new LoadOptions();
         opts.setLoadFilter(new LoadFilterSheet());
         Workbook wb = new Workbook("template.xlsx", opts);
         //Custom LoadFilter implementation
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [LoadFilter()](#LoadFilter--) | Создаёт один LoadFilter с параметрами фильтра по умолчанию LoadDataFilterOptions.All. |
| [LoadFilter(int opts)](#LoadFilter-int-) | Создаёт один LoadFilter с заданными параметрами фильтра. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getLoadDataFilterOptions()](#getLoadDataFilterOptions--) | Параметры фильтра, указывающие, какие данные следует загрузить. |
| [getSheetsInLoadingOrder()](#getSheetsInLoadingOrder--) | Указывает листы (индексы) и порядок их загрузки. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setLoadDataFilterOptions(int value)](#setLoadDataFilterOptions-int-) | Параметры фильтра, указывающие, какие данные следует загрузить. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Подготавливает параметры фильтра перед загрузкой указанного листа. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LoadFilter() {#LoadFilter--}
```
public LoadFilter()
```


Создаёт один LoadFilter с параметрами фильтра по умолчанию LoadDataFilterOptions.All.

### LoadFilter(int opts) {#LoadFilter-int-}
```
public LoadFilter(int opts)
```


Создаёт один LoadFilter с заданными параметрами фильтра.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| opts | int | [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions). параметры фильтра по умолчанию |

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
### getLoadDataFilterOptions() {#getLoadDataFilterOptions--}
```
public int getLoadDataFilterOptions()
```


Параметры фильтра, указывающие, какие данные следует загрузить.

См. [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Returns:**
int
### getSheetsInLoadingOrder() {#getSheetsInLoadingOrder--}
```
public int[] getSheetsInLoadingOrder()
```


Указывает листы (индексы) и порядок их загрузки. По умолчанию значение null, что означает загрузку всех листов в порядке по умолчанию из шаблонного файла. Если значение не null и индекс некоторого листа отсутствует в возвращённом массиве, то этот лист не будет загружен.

**Returns:**
int[]
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




### setLoadDataFilterOptions(int value) {#setLoadDataFilterOptions-int-}
```
public void setLoadDataFilterOptions(int value)
```


Параметры фильтра, указывающие, какие данные следует загрузить.

См. [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public void startSheet(Worksheet sheet)
```


Подготавливает параметры фильтра перед загрузкой указанного листа. Реализация LoadFilter пользователем может изменить LoadDataFilterOptions здесь, чтобы указать, как загружать данные для этого листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Лист, который будет загружен. Здесь можно использовать только несколько свойств объекта листа, поскольку большинство данных и свойств ещё не загружены. Доступные свойства: Name, Index, VisibilityType. |

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

