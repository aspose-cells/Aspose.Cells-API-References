---
title: "BuiltInDocumentPropertyCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Коллекция встроенных свойств документа."
type: docs
url: /ru/java/com.aspose.cells/builtindocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class BuiltInDocumentPropertyCollection extends DocumentPropertyCollection
```

Коллекция встроенных свойств документа.

**Remarks**

Обеспечивает доступ к объектам по их именам (используя индексатор) и через набор типизированных свойств, которые возвращают значения соответствующих типов.
## Методы

| Метод | Описание |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [clear()](#clear--) | Удаляет все объекты из экземпляра CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [contains(String name)](#contains-java.lang.String-) | Возвращает true, если свойство с указанным именем существует в коллекции. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Возвращает объект [DocumentProperty](../../com.aspose.cells/documentproperty) по индексу. |
| [get(String name)](#get-java.lang.String-) | Возвращает объект [DocumentProperty](../../com.aspose.cells/documentproperty) по имени свойства. |
| [getAuthor()](#getAuthor--) | Получает имя автора документа. |
| [getBytes()](#getBytes--) | Представляет оценку количества байтов в документе. |
| [getCategory()](#getCategory--) | Получает категорию документа. |
| [getCharacters()](#getCharacters--) | Представляет оценку количества символов в документе. |
| [getCharactersWithSpaces()](#getCharactersWithSpaces--) | Представляет оценку количества символов (включая пробелы) в документе. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Получает комментарии к документу. |
| [getCompany()](#getCompany--) | Получает свойство компании. |
| [getContentStatus()](#getContentStatus--) | Получает статус содержимого документа. |
| [getContentType()](#getContentType--) | Получает тип содержимого документа. |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [getCreatedTime()](#getCreatedTime--) | Получает дату создания документа в локальном часовом поясе. |
| [getCreatedUniversalTime()](#getCreatedUniversalTime--) | Получает универсальное время создания документа. |
| [getDocumentVersion()](#getDocumentVersion--) | Представляет версию файла. |
| [getHyperlinkBase()](#getHyperlinkBase--) | Получает свойство hyperlinkbase. |
| [getKeywords()](#getKeywords--) | Получает ключевые слова документа. |
| [getLanguage()](#getLanguage--) | Получает язык документа. |
| [getLastPrinted()](#getLastPrinted--) | Получает дату последней печати документа в локальном часовом поясе. |
| [getLastPrintedUniversalTime()](#getLastPrintedUniversalTime--) | Получает универсальное время последней печати документа. |
| [getLastSavedBy()](#getLastSavedBy--) | Получает имя последнего автора. |
| [getLastSavedTime()](#getLastSavedTime--) | Получает время последнего сохранения в локальном часовом поясе. |
| [getLastSavedUniversalTime()](#getLastSavedUniversalTime--) | Получает универсальное время последнего сохранения. |
| [getLines()](#getLines--) | Представляет оценку количества строк в документе. |
| [getLinksUpToDate()](#getLinksUpToDate--) | Указывает, актуальны ли гиперссылки в документе. |
| [getManager()](#getManager--) | Получает свойство manager. |
| [getNameOfApplication()](#getNameOfApplication--) | Получает имя приложения. |
| [getPages()](#getPages--) | Представляет оценку количества страниц в документе. |
| [getParagraphs()](#getParagraphs--) | Представляет оценку количества абзацев в документе. |
| [getRevisionNumber()](#getRevisionNumber--) | Получает номер ревизии документа. |
| [getScaleCrop()](#getScaleCrop--) | Указывает режим отображения миниатюры документа. |
| [getSubject()](#getSubject--) | Получает тему документа. |
| [getTemplate()](#getTemplate--) | Получает информационное имя шаблона документа. |
| [getTitle()](#getTitle--) | Получает заголовок документа. |
| [getTotalEditingTime()](#getTotalEditingTime--) | Получает общее время редактирования в минутах. |
| [getVersion()](#getVersion--) | Представляет номер версии приложения, создавшего документ. |
| [getWords()](#getWords--) | Представляет оценку количества слов в документе. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Получает индекс свойства по имени. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Удаляет свойство с указанным именем из коллекции. |
| [removeAt(int index)](#removeAt-int-) | Удаляет свойство по указанному индексу. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Устанавливает имя автора документа. |
| [setBytes(int value)](#setBytes-int-) | Представляет оценку количества байтов в документе. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Устанавливает категорию документа. |
| [setCharacters(int value)](#setCharacters-int-) | Представляет оценку количества символов в документе. |
| [setCharactersWithSpaces(int value)](#setCharactersWithSpaces-int-) | Представляет оценку количества символов (включая пробелы) в документе. |
| [setComments(String value)](#setComments-java.lang.String-) | Устанавливает комментарии к документу. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Устанавливает свойство company. |
| [setContentStatus(String value)](#setContentStatus-java.lang.String-) | Устанавливает статус содержимого документа. |
| [setContentType(String value)](#setContentType-java.lang.String-) | Устанавливает тип содержимого документа. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Устанавливает дату создания документа в локальном часовом поясе. |
| [setCreatedUniversalTime(DateTime value)](#setCreatedUniversalTime-com.aspose.cells.DateTime-) | Устанавливает универсальное время создания документа. |
| [setDocumentVersion(String value)](#setDocumentVersion-java.lang.String-) | Представляет версию файла. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Устанавливает свойство hyperlinkbase. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Устанавливает ключевые слова документа. |
| [setLanguage(String value)](#setLanguage-java.lang.String-) | Устанавливает язык документа. |
| [setLastPrinted(DateTime value)](#setLastPrinted-com.aspose.cells.DateTime-) | Устанавливает дату последней печати документа в локальном часовом поясе. |
| [setLastPrintedUniversalTime(DateTime value)](#setLastPrintedUniversalTime-com.aspose.cells.DateTime-) | Устанавливает универсальное время последней печати документа. |
| [setLastSavedBy(String value)](#setLastSavedBy-java.lang.String-) | Устанавливает имя последнего автора. |
| [setLastSavedTime(DateTime value)](#setLastSavedTime-com.aspose.cells.DateTime-) | Устанавливает время последнего сохранения в локальном часовом поясе. |
| [setLastSavedUniversalTime(DateTime value)](#setLastSavedUniversalTime-com.aspose.cells.DateTime-) | Устанавливает универсальное время последнего сохранения. |
| [setLines(int value)](#setLines-int-) | Представляет оценку количества строк в документе. |
| [setLinksUpToDate(boolean value)](#setLinksUpToDate-boolean-) | Указывает, актуальны ли гиперссылки в документе. |
| [setManager(String value)](#setManager-java.lang.String-) | Устанавливает свойство manager. |
| [setNameOfApplication(String value)](#setNameOfApplication-java.lang.String-) | Устанавливает имя приложения. |
| [setPages(int value)](#setPages-int-) | Представляет оценку количества страниц в документе. |
| [setParagraphs(int value)](#setParagraphs-int-) | Представляет оценку количества абзацев в документе. |
| [setRevisionNumber(String value)](#setRevisionNumber-java.lang.String-) | Устанавливает номер ревизии документа. |
| [setScaleCrop(boolean value)](#setScaleCrop-boolean-) | Указывает режим отображения миниатюры документа. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Устанавливает тему документа. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Устанавливает информационное имя шаблона документа. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Устанавливает заголовок документа. |
| [setTotalEditingTime(double value)](#setTotalEditingTime-double-) | Устанавливает общее время редактирования в минутах. |
| [setVersion(String value)](#setVersion-java.lang.String-) | Представляет номер версии приложения, создавшего документ. |
| [setWords(int value)](#setWords-int-) | Представляет оценку количества слов в документе. |
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
### clear() {#clear--}
```
public void clear()
```


Удаляет все объекты из экземпляра CollectionBase.

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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Возвращает true, если свойство с указанным именем существует в коллекции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя свойства без учёта регистра. |

**Returns:**
boolean - True, если свойство существует в коллекции; false в противном случае.
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
### get(int index) {#get-int-}
```
public DocumentProperty get(int index)
```


Возвращает объект [DocumentProperty](../../com.aspose.cells/documentproperty) по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| index | int | Нулевой индекс [DocumentProperty](../../com.aspose.cells/documentproperty) для получения. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Возвращает объект [DocumentProperty](../../com.aspose.cells/documentproperty) по имени свойства.

**Remarks**

Строковые имена свойств соответствуют именам типизированных свойств, доступных из .

Если вы запрашиваете свойство, которое отсутствует в документе, но имя свойства распознаётся как допустимое встроенное имя, создаётся новое  , добавляется в коллекцию и возвращается. Новое созданное свойство получает значение по умолчанию (пустая строка, ноль, false или DateTime.MinValue в зависимости от типа встроенного свойства).

Если вы запрашиваете свойство, которое отсутствует в документе, и имя не распознаётся как встроенное, возвращается null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя свойства без учёта регистра для получения. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Получает имя автора документа.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public int getBytes()
```


Представляет оценку количества байтов в документе.

**Returns:**
int
### getCategory() {#getCategory--}
```
public String getCategory()
```


Получает категорию документа.

**Returns:**
java.lang.String
### getCharacters() {#getCharacters--}
```
public int getCharacters()
```


Представляет оценку количества символов в документе.

**Returns:**
int
### getCharactersWithSpaces() {#getCharactersWithSpaces--}
```
public int getCharactersWithSpaces()
```


Представляет оценку количества символов (включая пробелы) в документе.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComments() {#getComments--}
```
public String getComments()
```


Получает комментарии к документу.

**Returns:**
java.lang.String
### getCompany() {#getCompany--}
```
public String getCompany()
```


Получает свойство компании.

**Returns:**
java.lang.String
### getContentStatus() {#getContentStatus--}
```
public String getContentStatus()
```


Получает статус содержимого документа.

**Returns:**
java.lang.String
### getContentType() {#getContentType--}
```
public String getContentType()
```


Получает тип содержимого документа.

**Returns:**
java.lang.String
### getCount() {#getCount--}
```
public int getCount()
```


Получает количество элементов, содержащихся в экземпляре CollectionBase.

**Returns:**
int — количество элементов, содержащихся в экземпляре CollectionBase.
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Получает дату создания документа в локальном часовом поясе.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCreatedUniversalTime() {#getCreatedUniversalTime--}
```
public DateTime getCreatedUniversalTime()
```


Получает универсальное время создания документа.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDocumentVersion() {#getDocumentVersion--}
```
public String getDocumentVersion()
```


Представляет версию файла.

**Returns:**
java.lang.String
### getHyperlinkBase() {#getHyperlinkBase--}
```
public String getHyperlinkBase()
```


Получает свойство hyperlinkbase.

**Returns:**
java.lang.String
### getKeywords() {#getKeywords--}
```
public String getKeywords()
```


Получает ключевые слова документа.

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public String getLanguage()
```


Получает язык документа.

**Returns:**
java.lang.String
### getLastPrinted() {#getLastPrinted--}
```
public DateTime getLastPrinted()
```


Получает дату последней печати документа в локальном часовом поясе.

**Remarks**

Если документ никогда не печатался, это свойство вернёт DateTime.MinValue.

Aspose.Cells не обновляет это свойство при изменении документа.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastPrintedUniversalTime() {#getLastPrintedUniversalTime--}
```
public DateTime getLastPrintedUniversalTime()
```


Получает универсальное время последней печати документа.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedBy() {#getLastSavedBy--}
```
public String getLastSavedBy()
```


Получает имя последнего автора.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Returns:**
java.lang.String
### getLastSavedTime() {#getLastSavedTime--}
```
public DateTime getLastSavedTime()
```


Получает время последнего сохранения в локальном часовом поясе.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedUniversalTime() {#getLastSavedUniversalTime--}
```
public DateTime getLastSavedUniversalTime()
```


Получает универсальное время последнего сохранения.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLines() {#getLines--}
```
public int getLines()
```


Представляет оценку количества строк в документе.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Returns:**
int
### getLinksUpToDate() {#getLinksUpToDate--}
```
public boolean getLinksUpToDate()
```


Указывает, актуальны ли гиперссылки в документе.

**Returns:**
boolean
### getManager() {#getManager--}
```
public String getManager()
```


Получает свойство manager.

**Returns:**
java.lang.String
### getNameOfApplication() {#getNameOfApplication--}
```
public String getNameOfApplication()
```


Получает имя приложения.

**Returns:**
java.lang.String
### getPages() {#getPages--}
```
public int getPages()
```


Представляет оценку количества страниц в документе.

**Returns:**
int
### getParagraphs() {#getParagraphs--}
```
public int getParagraphs()
```


Представляет оценку количества абзацев в документе.

**Returns:**
int
### getRevisionNumber() {#getRevisionNumber--}
```
public String getRevisionNumber()
```


Получает номер ревизии документа.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Returns:**
java.lang.String
### getScaleCrop() {#getScaleCrop--}
```
public boolean getScaleCrop()
```


Указывает режим отображения миниатюры документа.

**Returns:**
boolean
### getSubject() {#getSubject--}
```
public String getSubject()
```


Получает тему документа.

**Returns:**
java.lang.String
### getTemplate() {#getTemplate--}
```
public String getTemplate()
```


Получает информационное имя шаблона документа.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Получает заголовок документа.

**Returns:**
java.lang.String
### getTotalEditingTime() {#getTotalEditingTime--}
```
public double getTotalEditingTime()
```


Получает общее время редактирования в минутах.

**Returns:**
double
### getVersion() {#getVersion--}
```
public String getVersion()
```


Представляет номер версии приложения, создавшего документ.

**Remarks**

Её формат "00.0000", например: 12.0000

**Returns:**
java.lang.String
### getWords() {#getWords--}
```
public int getWords()
```


Представляет оценку количества слов в документе.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Получает индекс свойства по имени.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя свойства без учёта регистра. |

**Returns:**
int - Нулевой индекс. Отрицательное значение, если не найдено.
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Удаляет свойство с указанным именем из коллекции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя свойства без учёта регистра. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удаляет свойство по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Нулевой индекс. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Устанавливает имя автора документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setBytes(int value) {#setBytes-int-}
```
public void setBytes(int value)
```


Представляет оценку количества байтов в документе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public void setCategory(String value)
```


Устанавливает категорию документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCharacters(int value) {#setCharacters-int-}
```
public void setCharacters(int value)
```


Представляет оценку количества символов в документе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCharactersWithSpaces(int value) {#setCharactersWithSpaces-int-}
```
public void setCharactersWithSpaces(int value)
```


Представляет оценку количества символов (включая пробелы) в документе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


Устанавливает комментарии к документу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public void setCompany(String value)
```


Устанавливает свойство company.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setContentStatus(String value) {#setContentStatus-java.lang.String-}
```
public void setContentStatus(String value)
```


Устанавливает статус содержимого документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setContentType(String value) {#setContentType-java.lang.String-}
```
public void setContentType(String value)
```


Устанавливает тип содержимого документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


Устанавливает дату создания документа в локальном часовом поясе.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCreatedUniversalTime(DateTime value) {#setCreatedUniversalTime-com.aspose.cells.DateTime-}
```
public void setCreatedUniversalTime(DateTime value)
```


Устанавливает универсальное время создания документа.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setDocumentVersion(String value) {#setDocumentVersion-java.lang.String-}
```
public void setDocumentVersion(String value)
```


Представляет версию файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public void setHyperlinkBase(String value)
```


Устанавливает свойство hyperlinkbase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public void setKeywords(String value)
```


Устанавливает ключевые слова документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setLanguage(String value) {#setLanguage-java.lang.String-}
```
public void setLanguage(String value)
```


Устанавливает язык документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setLastPrinted(DateTime value) {#setLastPrinted-com.aspose.cells.DateTime-}
```
public void setLastPrinted(DateTime value)
```


Устанавливает дату последней печати документа в локальном часовом поясе.

**Remarks**

Если документ никогда не печатался, это свойство вернёт DateTime.MinValue.

Aspose.Cells не обновляет это свойство при изменении документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastPrintedUniversalTime(DateTime value) {#setLastPrintedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastPrintedUniversalTime(DateTime value)
```


Устанавливает универсальное время последней печати документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedBy(String value) {#setLastSavedBy-java.lang.String-}
```
public void setLastSavedBy(String value)
```


Устанавливает имя последнего автора.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setLastSavedTime(DateTime value) {#setLastSavedTime-com.aspose.cells.DateTime-}
```
public void setLastSavedTime(DateTime value)
```


Устанавливает время последнего сохранения в локальном часовом поясе.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedUniversalTime(DateTime value) {#setLastSavedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastSavedUniversalTime(DateTime value)
```


Устанавливает универсальное время последнего сохранения.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLines(int value) {#setLines-int-}
```
public void setLines(int value)
```


Представляет оценку количества строк в документе.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLinksUpToDate(boolean value) {#setLinksUpToDate-boolean-}
```
public void setLinksUpToDate(boolean value)
```


Указывает, актуальны ли гиперссылки в документе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setManager(String value) {#setManager-java.lang.String-}
```
public void setManager(String value)
```


Устанавливает свойство manager.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setNameOfApplication(String value) {#setNameOfApplication-java.lang.String-}
```
public void setNameOfApplication(String value)
```


Устанавливает имя приложения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPages(int value) {#setPages-int-}
```
public void setPages(int value)
```


Представляет оценку количества страниц в документе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setParagraphs(int value) {#setParagraphs-int-}
```
public void setParagraphs(int value)
```


Представляет оценку количества абзацев в документе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRevisionNumber(String value) {#setRevisionNumber-java.lang.String-}
```
public void setRevisionNumber(String value)
```


Устанавливает номер ревизии документа.

**Remarks**

Aspose.Cells не обновляет это свойство при изменении документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setScaleCrop(boolean value) {#setScaleCrop-boolean-}
```
public void setScaleCrop(boolean value)
```


Указывает режим отображения миниатюры документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public void setSubject(String value)
```


Устанавливает тему документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public void setTemplate(String value)
```


Устанавливает информационное имя шаблона документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Устанавливает заголовок документа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTotalEditingTime(double value) {#setTotalEditingTime-double-}
```
public void setTotalEditingTime(double value)
```


Устанавливает общее время редактирования в минутах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setVersion(String value) {#setVersion-java.lang.String-}
```
public void setVersion(String value)
```


Представляет номер версии приложения, создавшего документ.

**Remarks**

Её формат "00.0000", например: 12.0000

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setWords(int value) {#setWords-int-}
```
public void setWords(int value)
```


Представляет оценку количества слов в документе.

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

