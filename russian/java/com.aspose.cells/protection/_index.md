---
title: "Защита"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет различные типы параметров защиты, доступных для листа."
type: docs
url: /ru/java/com.aspose.cells/protection/
---

**Inheritance:**
java.lang.Object
```
public class Protection
```

Представляет различные типы параметров защиты, доступных для листа.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Allowing users to select locked cells of the worksheet
         worksheet.getProtection().setAllowSelectingLockedCell(true);
         //Allowing users to select unlocked cells of the worksheet
         worksheet.getProtection().setAllowSelectingUnlockedCell(true);
```
## Методы

| Метод | Описание |
| --- | --- |
| [copy(Protection source)](#copy-com.aspose.cells.Protection-) | Копировать информацию о защите. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--) | Представляет, разрешено ли удаление столбцов на защищённом листе. |
| [getAllowDeletingRow()](#getAllowDeletingRow--) | Представляет, разрешено ли удаление строк на защищённом листе. |
| [getAllowEditingContent()](#getAllowEditingContent--) | Представляет, разрешено ли пользователю редактировать содержимое заблокированных ячеек на защищённом листе. |
| [getAllowEditingObject()](#getAllowEditingObject--) | Представляет, разрешено ли пользователю манипулировать графическими объектами на защищённом листе. |
| [getAllowEditingScenario()](#getAllowEditingScenario--) | Представляет, разрешено ли пользователю редактировать сценарии на защищённом листе. |
| [getAllowFiltering()](#getAllowFiltering--) | Представляет, разрешено ли пользователю использовать AutoFilter, созданный до защиты листа. |
| [getAllowFormattingCell()](#getAllowFormattingCell--) | Представляет, разрешено ли форматирование ячеек на защищённом листе. |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--) | Представляет, разрешено ли форматирование столбцов на защищённом листе |
| [getAllowFormattingRow()](#getAllowFormattingRow--) | Представляет, разрешено ли форматирование строк на защищённом листе |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--) | Представляет, разрешено ли вставка столбцов на защищённом листе |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--) | Представляет, разрешена ли вставка гиперссылок на защищённом листе |
| [getAllowInsertingRow()](#getAllowInsertingRow--) | Представляет, разрешена ли вставка строк на защищённом листе |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--) | Представляет, разрешено ли пользователю выбирать заблокированные ячейки на защищённом листе. |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--) | Представляет, разрешено ли пользователю выбирать разблокированные ячейки на защищённом листе. |
| [getAllowSorting()](#getAllowSorting--) | Представляет, разрешена ли опция сортировки на защищённом листе. |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--) | Представляет, разрешено ли пользователю манипулировать сводными таблицами на защищённом листе. |
| [getClass()](#getClass--) |  |
| [getPassword()](#getPassword--) | Представляет пароль для защиты листа. |
| [getPasswordHash()](#getPasswordHash--) | Получает хеш текущего пароля. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Указывает, защищен ли лист паролем. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDeletingColumn(boolean value)](#setAllowDeletingColumn-boolean-) | Представляет, разрешено ли удаление столбцов на защищённом листе. |
| [setAllowDeletingRow(boolean value)](#setAllowDeletingRow-boolean-) | Представляет, разрешено ли удаление строк на защищённом листе. |
| [setAllowEditingContent(boolean value)](#setAllowEditingContent-boolean-) | Представляет, разрешено ли пользователю редактировать содержимое заблокированных ячеек на защищённом листе. |
| [setAllowEditingObject(boolean value)](#setAllowEditingObject-boolean-) | Представляет, разрешено ли пользователю манипулировать графическими объектами на защищённом листе. |
| [setAllowEditingScenario(boolean value)](#setAllowEditingScenario-boolean-) | Представляет, разрешено ли пользователю редактировать сценарии на защищённом листе. |
| [setAllowFiltering(boolean value)](#setAllowFiltering-boolean-) | Представляет, разрешено ли пользователю использовать AutoFilter, созданный до защиты листа. |
| [setAllowFormattingCell(boolean value)](#setAllowFormattingCell-boolean-) | Представляет, разрешено ли форматирование ячеек на защищённом листе. |
| [setAllowFormattingColumn(boolean value)](#setAllowFormattingColumn-boolean-) | Представляет, разрешено ли форматирование столбцов на защищённом листе |
| [setAllowFormattingRow(boolean value)](#setAllowFormattingRow-boolean-) | Представляет, разрешено ли форматирование строк на защищённом листе |
| [setAllowInsertingColumn(boolean value)](#setAllowInsertingColumn-boolean-) | Представляет, разрешено ли вставка столбцов на защищённом листе |
| [setAllowInsertingHyperlink(boolean value)](#setAllowInsertingHyperlink-boolean-) | Представляет, разрешена ли вставка гиперссылок на защищённом листе |
| [setAllowInsertingRow(boolean value)](#setAllowInsertingRow-boolean-) | Представляет, разрешена ли вставка строк на защищённом листе |
| [setAllowSelectingLockedCell(boolean value)](#setAllowSelectingLockedCell-boolean-) | Представляет, разрешено ли пользователю выбирать заблокированные ячейки на защищённом листе. |
| [setAllowSelectingUnlockedCell(boolean value)](#setAllowSelectingUnlockedCell-boolean-) | Представляет, разрешено ли пользователю выбирать разблокированные ячейки на защищённом листе. |
| [setAllowSorting(boolean value)](#setAllowSorting-boolean-) | Представляет, разрешена ли опция сортировки на защищённом листе. |
| [setAllowUsingPivotTable(boolean value)](#setAllowUsingPivotTable-boolean-) | Представляет, разрешено ли пользователю манипулировать сводными таблицами на защищённом листе. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Представляет пароль для защиты листа. |
| [toString()](#toString--) |  |
| [verifyPassword(String password)](#verifyPassword-java.lang.String-) | Проверяет пароль. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(Protection source) {#copy-com.aspose.cells.Protection-}
```
public void copy(Protection source)
```


Копировать информацию о защите.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [Protection](../../com.aspose.cells/protection) |  |

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
### getAllowDeletingColumn() {#getAllowDeletingColumn--}
```
public boolean getAllowDeletingColumn()
```


Представляет, разрешено ли удаление столбцов на защищённом листе.

**Remarks**

Столбцы, содержащие ячейки, подлежащие удалению, должны быть разблокированы, когда лист защищён, и опция "Select unlocked cells" должна быть включена.

**Returns:**
boolean
### getAllowDeletingRow() {#getAllowDeletingRow--}
```
public boolean getAllowDeletingRow()
```


Представляет, разрешено ли удаление строк на защищённом листе.

**Remarks**

Строки, содержащие ячейки, подлежащие удалению, должны быть разблокированы, когда лист защищён, и опция "Select unlocked cells" должна быть включена.

**Returns:**
boolean
### getAllowEditingContent() {#getAllowEditingContent--}
```
public boolean getAllowEditingContent()
```


Представляет, разрешено ли пользователю редактировать содержимое заблокированных ячеек на защищённом листе.

**Returns:**
boolean
### getAllowEditingObject() {#getAllowEditingObject--}
```
public boolean getAllowEditingObject()
```


Представляет, разрешено ли пользователю манипулировать графическими объектами на защищённом листе.

**Returns:**
boolean
### getAllowEditingScenario() {#getAllowEditingScenario--}
```
public boolean getAllowEditingScenario()
```


Представляет, разрешено ли пользователю редактировать сценарии на защищённом листе.

**Returns:**
boolean
### getAllowFiltering() {#getAllowFiltering--}
```
public boolean getAllowFiltering()
```


Представляет, разрешено ли пользователю использовать AutoFilter, созданный до защиты листа.

**Returns:**
boolean
### getAllowFormattingCell() {#getAllowFormattingCell--}
```
public boolean getAllowFormattingCell()
```


Представляет, разрешено ли форматирование ячеек на защищённом листе.

**Returns:**
boolean
### getAllowFormattingColumn() {#getAllowFormattingColumn--}
```
public boolean getAllowFormattingColumn()
```


Представляет, разрешено ли форматирование столбцов на защищённом листе

**Returns:**
boolean
### getAllowFormattingRow() {#getAllowFormattingRow--}
```
public boolean getAllowFormattingRow()
```


Представляет, разрешено ли форматирование строк на защищённом листе

**Returns:**
boolean
### getAllowInsertingColumn() {#getAllowInsertingColumn--}
```
public boolean getAllowInsertingColumn()
```


Представляет, разрешено ли вставка столбцов на защищённом листе

**Returns:**
boolean
### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}
```
public boolean getAllowInsertingHyperlink()
```


Представляет, разрешена ли вставка гиперссылок на защищённом листе

**Returns:**
boolean
### getAllowInsertingRow() {#getAllowInsertingRow--}
```
public boolean getAllowInsertingRow()
```


Представляет, разрешена ли вставка строк на защищённом листе

**Returns:**
boolean
### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}
```
public boolean getAllowSelectingLockedCell()
```


Представляет, разрешено ли пользователю выбирать заблокированные ячейки на защищённом листе.

**Returns:**
boolean
### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}
```
public boolean getAllowSelectingUnlockedCell()
```


Представляет, разрешено ли пользователю выбирать разблокированные ячейки на защищённом листе.

**Returns:**
boolean
### getAllowSorting() {#getAllowSorting--}
```
public boolean getAllowSorting()
```


Представляет, разрешена ли опция сортировки на защищённом листе.

**Returns:**
boolean
### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}
```
public boolean getAllowUsingPivotTable()
```


Представляет, разрешено ли пользователю манипулировать сводными таблицами на защищённом листе.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPassword() {#getPassword--}
```
public String getPassword()
```


Представляет пароль для защиты листа.

**Remarks**

Если пароль установлен как null или пустая строка, вы можете снять защиту листа или книги без использования пароля. В противном случае необходимо указать пароль для снятия защиты листа или книги.

**Returns:**
java.lang.String
### getPasswordHash() {#getPasswordHash--}
```
public int getPasswordHash()
```


Получает хеш текущего пароля.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


Указывает, защищен ли лист паролем.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllowDeletingColumn(boolean value) {#setAllowDeletingColumn-boolean-}
```
public void setAllowDeletingColumn(boolean value)
```


Представляет, разрешено ли удаление столбцов на защищённом листе.

**Remarks**

Столбцы, содержащие ячейки, подлежащие удалению, должны быть разблокированы, когда лист защищён, и опция "Select unlocked cells" должна быть включена.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowDeletingRow(boolean value) {#setAllowDeletingRow-boolean-}
```
public void setAllowDeletingRow(boolean value)
```


Представляет, разрешено ли удаление строк на защищённом листе.

**Remarks**

Строки, содержащие ячейки, подлежащие удалению, должны быть разблокированы, когда лист защищён, и опция "Select unlocked cells" должна быть включена.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowEditingContent(boolean value) {#setAllowEditingContent-boolean-}
```
public void setAllowEditingContent(boolean value)
```


Представляет, разрешено ли пользователю редактировать содержимое заблокированных ячеек на защищённом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowEditingObject(boolean value) {#setAllowEditingObject-boolean-}
```
public void setAllowEditingObject(boolean value)
```


Представляет, разрешено ли пользователю манипулировать графическими объектами на защищённом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowEditingScenario(boolean value) {#setAllowEditingScenario-boolean-}
```
public void setAllowEditingScenario(boolean value)
```


Представляет, разрешено ли пользователю редактировать сценарии на защищённом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowFiltering(boolean value) {#setAllowFiltering-boolean-}
```
public void setAllowFiltering(boolean value)
```


Представляет, разрешено ли пользователю использовать AutoFilter, созданный до защиты листа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowFormattingCell(boolean value) {#setAllowFormattingCell-boolean-}
```
public void setAllowFormattingCell(boolean value)
```


Представляет, разрешено ли форматирование ячеек на защищённом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowFormattingColumn(boolean value) {#setAllowFormattingColumn-boolean-}
```
public void setAllowFormattingColumn(boolean value)
```


Представляет, разрешено ли форматирование столбцов на защищённом листе

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowFormattingRow(boolean value) {#setAllowFormattingRow-boolean-}
```
public void setAllowFormattingRow(boolean value)
```


Представляет, разрешено ли форматирование строк на защищённом листе

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowInsertingColumn(boolean value) {#setAllowInsertingColumn-boolean-}
```
public void setAllowInsertingColumn(boolean value)
```


Представляет, разрешено ли вставка столбцов на защищённом листе

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowInsertingHyperlink(boolean value) {#setAllowInsertingHyperlink-boolean-}
```
public void setAllowInsertingHyperlink(boolean value)
```


Представляет, разрешена ли вставка гиперссылок на защищённом листе

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowInsertingRow(boolean value) {#setAllowInsertingRow-boolean-}
```
public void setAllowInsertingRow(boolean value)
```


Представляет, разрешена ли вставка строк на защищённом листе

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowSelectingLockedCell(boolean value) {#setAllowSelectingLockedCell-boolean-}
```
public void setAllowSelectingLockedCell(boolean value)
```


Представляет, разрешено ли пользователю выбирать заблокированные ячейки на защищённом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowSelectingUnlockedCell(boolean value) {#setAllowSelectingUnlockedCell-boolean-}
```
public void setAllowSelectingUnlockedCell(boolean value)
```


Представляет, разрешено ли пользователю выбирать разблокированные ячейки на защищённом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowSorting(boolean value) {#setAllowSorting-boolean-}
```
public void setAllowSorting(boolean value)
```


Представляет, разрешена ли опция сортировки на защищённом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAllowUsingPivotTable(boolean value) {#setAllowUsingPivotTable-boolean-}
```
public void setAllowUsingPivotTable(boolean value)
```


Представляет, разрешено ли пользователю манипулировать сводными таблицами на защищённом листе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Представляет пароль для защиты листа.

**Remarks**

Если пароль установлен как null или пустая строка, вы можете снять защиту листа или книги без использования пароля. В противном случае необходимо указать пароль для снятия защиты листа или книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### verifyPassword(String password) {#verifyPassword-java.lang.String-}
```
public boolean verifyPassword(String password)
```


Проверяет пароль.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| пароль | java.lang.String | Пароль. |

**Returns:**
boolean -
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

