---
title: "Workbook"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет корневой объект для создания электронной таблицы Excel."
type: docs
url: /ru/java/com.aspose.cells/workbook/
---

**Inheritance:**
java.lang.Object
```
public class Workbook
```

Представляет корневой объект для создания электронной таблицы Excel.

**Remarks**

Класс Workbook обозначает электронную таблицу Excel. Каждая таблица может содержать несколько листов. Основная функция класса — открывать и сохранять родные файлы Excel. Класс имеет некоторые расширенные возможности, такие как копирование данных из других Workbook, объединение двух Workbook, преобразование Excel в PDF, рендеринг Excel в изображение и защита электронной таблицы Excel.

**Example**

В следующем примере загружается Workbook из файла Excel с именем designer.xls и делаются горизонтальная и вертикальная полосы прокрутки невидимыми. Затем в таблице заменяются два строковых значения на целочисленное значение и строковое значение соответственно, и в конце рабочая книга сохраняется как файл Excel xlsx.

```
         //Open a designer file
         String designerFile = "designer.xls";
         Workbook workbook = new Workbook(designerFile);
 
         //Set scroll bars
         workbook.getSettings().setHScrollBarVisible(false);
         workbook.getSettings().setVScrollBarVisible(false);
 
         //Replace the placeholder string with new values
         int newInt = 100;
         workbook.replace("OldInt", newInt);
 
         String newString = "Hello!";
         workbook.replace("OldString", newString);
         workbook.save("result.xlsx");
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Workbook()](#Workbook--) | Инициализирует новый экземпляр класса [Workbook](../../com.aspose.cells/workbook). |
| [Workbook(int fileFormatType)](#Workbook-int-) | Инициализирует новый экземпляр класса [Workbook](../../com.aspose.cells/workbook). |
| [Workbook(LoadOptions loadOptions)](#Workbook-com.aspose.cells.LoadOptions-) | Инициализирует новый пустой экземпляр класса [Workbook](../../com.aspose.cells/workbook) с параметрами |
| [Workbook(String file)](#Workbook-java.lang.String-) | Инициализирует новый экземпляр класса [Workbook](../../com.aspose.cells/workbook) и открывает файл. |
| [Workbook(InputStream stream)](#Workbook-java.io.InputStream-) | Инициализирует новый экземпляр класса [Workbook](../../com.aspose.cells/workbook) и открывает поток. |
| [Workbook(String file, LoadOptions loadOptions)](#Workbook-java.lang.String-com.aspose.cells.LoadOptions-) | Инициализирует новый экземпляр класса [Workbook](../../com.aspose.cells/workbook) и открывает файл. |
| [Workbook(InputStream stream, LoadOptions loadOptions)](#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-) | Инициализирует новый экземпляр класса [Workbook](../../com.aspose.cells/workbook) и открывает поток. |
## Методы

| Метод | Описание |
| --- | --- |
| [acceptAllRevisions()](#acceptAllRevisions--) | Принимает все отслеживаемые изменения в рабочей книге. |
| [addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Добавляет цифровую подпись в файл электронной таблицы OOXML (Excel2007 и новее). |
| [calculateFormula()](#calculateFormula--) | Вычисляет результат формул. |
| [calculateFormula(boolean ignoreError)](#calculateFormula-boolean-) | Вычисляет результат формул. |
| [calculateFormula(CalculationOptions options)](#calculateFormula-com.aspose.cells.CalculationOptions-) | Вычисление формул в этой рабочей книге. |
| [changePalette(Color color, int index)](#changePalette-com.aspose.cells.Color-int-) | Изменяет палитру электронной таблицы по указанному индексу. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Закрывает сеанс, использующий кэши для доступа к данным. |
| [combine(Workbook secondWorkbook)](#combine-com.aspose.cells.Workbook-) | Объединяет другой объект Workbook. |
| [copy(Workbook source)](#copy-com.aspose.cells.Workbook-) | Копирует данные из исходного объекта Workbook. |
| [copy(Workbook source, CopyOptions copyOptions)](#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-) | Копирует другой объект Workbook. |
| [copyTheme(Workbook source)](#copyTheme-com.aspose.cells.Workbook-) | Копирует тему из другой рабочей книги. |
| [createBuiltinStyle(int type)](#createBuiltinStyle-int-) | Создаёт встроенный стиль указанного типа. |
| [createCellsColor()](#createCellsColor--) | Создаёт объект [CellsColor](../../com.aspose.cells/cellscolor). |
| [createStyle()](#createStyle--) | Создаёт новый стиль. |
| [createStyle(boolean cloneDefaultStyle)](#createStyle-boolean-) | Создаёт новый стиль. |
| [customTheme(String themeName, Color[] colors)](#customTheme-java.lang.String-com.aspose.cells.Color---) | Настраивает тему. |
| [dispose()](#dispose--) | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportXml(String mapName, OutputStream stream)](#exportXml-java.lang.String-java.io.OutputStream-) | Экспортирует XML-данные, связанные указанной XML-картой. |
| [exportXml(String mapName, String path)](#exportXml-java.lang.String-java.lang.String-) | Экспортирует XML-данные, связанные указанной XML-картой. |
| [getAbsolutePath()](#getAbsolutePath--) | Получает абсолютный путь к файлу. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Возвращает коллекцию [DocumentProperty](../../com.aspose.cells/documentproperty), представляющую все встроенные свойства документа электронной таблицы. |
| [getCellsDataTableFactory()](#getCellsDataTableFactory--) | Получает фабрику для создания ICellsDataTable из пользовательских объектов |
| [getClass()](#getClass--) |  |
| [getColors()](#getColors--) | Возвращает цвета в палитре электронной таблицы. |
| [getContentTypeProperties()](#getContentTypeProperties--) | Получает список объектов [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) в рабочей книге. |
| [getCountOfStylesInPool()](#getCountOfStylesInPool--) | Получает количество стилей в пуле стилей. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Возвращает коллекцию [DocumentProperty](../../com.aspose.cells/documentproperty), представляющую все пользовательские свойства документа электронной таблицы. |
| [getCustomXmlParts()](#getCustomXmlParts--) | Представляет часть хранилища пользовательских XML‑данных (пользовательские XML‑данные внутри пакета). |
| [getDataConnections()](#getDataConnections--) | Получает коллекцию [ExternalConnection](../../com.aspose.cells/externalconnection). |
| [getDataMashup()](#getDataMashup--) | Получает данные mashup. |
| [getDataModel()](#getDataModel--) | Получает модель данных в рабочей книге. |
| [getDataSorter()](#getDataSorter--) | Получает объект DataSorter для сортировки данных. |
| [getDefaultStyle()](#getDefaultStyle--) | Получает объект [Style](../../com.aspose.cells/style) по умолчанию рабочей книги. |
| [getDigitalSignature()](#getDigitalSignature--) | Получает цифровую подпись из файла. |
| [getFileFormat()](#getFileFormat--) | Получает формат файла. |
| [getFileName()](#getFileName--) | Получает текущее имя файла. |
| [getFonts()](#getFonts--) | Получает все шрифты в пуле стилей. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Получает монитор прерываний. |
| [getMatchingColor(Color rawColor)](#getMatchingColor-com.aspose.cells.Color-) | Находит наиболее подходящий цвет в текущей палитре. |
| [getNamedStyle(String name)](#getNamedStyle-java.lang.String-) | Получает именованный стиль в пуле стилей. |
| [getRibbonXml()](#getRibbonXml--) | Получает XML‑файл, определяющий пользовательский интерфейс Ribbon. |
| [getSettings()](#getSettings--) | Представляет настройки рабочей книги. |
| [getStyleInPool(int index)](#getStyleInPool-int-) | Получает стиль в пуле стилей. |
| [getTheme()](#getTheme--) | Получает название темы. |
| [getThemeColor(int type)](#getThemeColor-int-) | Получает цвет темы. |
| [getVbaProject()](#getVbaProject--) | Получает [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) в электронной таблице. |
| [getWorksheets()](#getWorksheets--) | Получает коллекцию [WorksheetCollection](../../com.aspose.cells/worksheetcollection) в электронной таблице. |
| [hasCustomFunction()](#hasCustomFunction--) | Определяет, используется ли в этой рабочей книге пользовательская функция, например в формулах ячеек, в определённых именах... |
| [hasExernalLinks()](#hasExernalLinks--) | Указывает, содержит ли эта рабочая книга внешние ссылки на другие источники данных. |
| [hasMacro()](#hasMacro--) | Указывает, содержит ли эта электронная таблица макросы/VBA. |
| [hasRevisions()](#hasRevisions--) | Получает, есть ли в рабочей книге отслеживаемые изменения |
| [hashCode()](#hashCode--) |  |
| [importXml(InputStream stream, String sheetName, int row, int col)](#importXml-java.io.InputStream-java.lang.String-int-int-) | Импортирует/обновляет XML‑файл данных в рабочую книгу. |
| [importXml(String url, String sheetName, int row, int col)](#importXml-java.lang.String-java.lang.String-int-int-) | Импортирует/обновляет XML‑файл данных в рабочую книгу. |
| [isColorInPalette(Color color)](#isColorInPalette-com.aspose.cells.Color-) | Проверяет, находится ли цвет в палитре электронной таблицы. |
| [isDigitallySigned()](#isDigitallySigned--) | Указывает, подписана ли эта электронная таблица цифровой подписью. |
| [isLicensed()](#isLicensed--) | Указывает, установлен ли лицензионный ключ. |
| [isWorkbookProtectedWithPassword()](#isWorkbookProtectedWithPassword--) | Указывает, защищены ли структура или окно паролем. |
| [mergeNamedStyles(Workbook source)](#mergeNamedStyles-com.aspose.cells.Workbook-) | Объединяет именованные стили из другого файла Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parseFormulas(boolean ignoreError)](#parseFormulas-boolean-) | Разбирает все формулы, которые не были разобраны при загрузке из шаблонного файла или при установке в ячейку. |
| [protect(int protectionType, String password)](#protect-int-java.lang.String-) | Защищает рабочую книгу. |
| [protectSharedWorkbook(String password)](#protectSharedWorkbook-java.lang.String-) | Защищает общую рабочую книгу. |
| [refreshAll()](#refreshAll--) | Обновить связанные фигуры, все сводные таблицы и диаграммы с источником сводных данных. |
| [refreshDynamicArrayFormulas(boolean calculate)](#refreshDynamicArrayFormulas-boolean-) | Обновляет формулы динамических массивов (распространяются в новый диапазон соседних ячеек в соответствии с текущими данными) Другие формулы в книге не будут вычисляться рекурсивно, даже если они использовались формулами динамических массивов. |
| [refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)](#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-) | Обновляет формулы динамических массивов (распространяются в новый диапазон соседних ячеек в соответствии с текущими данными) |
| [removeDigitalSignature()](#removeDigitalSignature--) | Удаляет цифровую подпись из этой таблицы. |
| [removeExternalLinks()](#removeExternalLinks--) | Удаляет все внешние ссылки в книге. |
| [removeMacro()](#removeMacro--) | Удаляет VBA/макрос из этой таблицы. |
| [removePersonalInformation()](#removePersonalInformation--) | Удаляет личную информацию. |
| [removeUnusedStyles()](#removeUnusedStyles--) | Удалить все неиспользуемые стили. |
| [replace(boolean boolValue, Object newValue)](#replace-boolean-java.lang.Object-) | Заменяет значения ячеек новыми данными. |
| [replace(int intValue, Object newValue)](#replace-int-java.lang.Object-) | Заменяет значения ячеек новыми данными. |
| [replace(String placeHolder, double newValue)](#replace-java.lang.String-double-) | Заменяет значение ячейки новым числом с плавающей точкой. |
| [replace(String placeHolder, double[] newValues, boolean isVertical)](#replace-java.lang.String-double---boolean-) | Заменяет значения ячеек массивом чисел с плавающей точкой. |
| [replace(String placeHolder, int newValue)](#replace-java.lang.String-int-) | Заменяет значение ячейки новым целым числом. |
| [replace(String placeHolder, int[] newValues, boolean isVertical)](#replace-java.lang.String-int---boolean-) | Заменяет значения ячеек массивом целых чисел. |
| [replace(String placeHolder, String newValue)](#replace-java.lang.String-java.lang.String-) | Заменяет значение ячейки новой строкой. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Заменяет значение ячейки новой строкой. |
| [replace(String placeHolder, String[] newValues, boolean isVertical)](#replace-java.lang.String-java.lang.String---boolean-) | Заменяет значение ячейки новым массивом строк. |
| [save(OutputStream stream, SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.cells.SaveOptions-) | Сохранить книгу в поток. |
| [save(OutputStream stream, int saveFormat)](#save-java.io.OutputStream-int-) | Сохранить книгу в поток. |
| [save(String fileName)](#save-java.lang.String-) | Сохранить книгу на диск. |
| [save(String fileName, SaveOptions saveOptions)](#save-java.lang.String-com.aspose.cells.SaveOptions-) | Сохраняет книгу на диск. |
| [save(String fileName, int saveFormat)](#save-java.lang.String-int-) | Сохраняет книгу на диск. |
| [setAbsolutePath(String value)](#setAbsolutePath-java.lang.String-) | Устанавливает абсолютный путь к файлу. |
| [setDefaultStyle(Style value)](#setDefaultStyle-com.aspose.cells.Style-) | Устанавливает объект [Style](../../com.aspose.cells/style) по умолчанию для книги. |
| [setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Устанавливает цифровую подпись для файла электронной таблицы (Excel2007 и новее). |
| [setEncryptionOptions(int encryptionType, int keyLength)](#setEncryptionOptions-int-int-) | Установить параметры шифрования. |
| [setFileFormat(int value)](#setFileFormat-int-) | Устанавливает формат файла. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Устанавливает текущее имя файла. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Устанавливает монитор прерываний. |
| [setRibbonXml(String value)](#setRibbonXml-java.lang.String-) | Устанавливает XML‑файл, определяющий интерфейс Ribbon. |
| [setThemeColor(int type, Color color)](#setThemeColor-int-com.aspose.cells.Color-) | Устанавливает цвет темы |
| [startAccessCache(int opts)](#startAccessCache-int-) | Запускает сеанс, использующий кэши для доступа к данным. |
| [toString()](#toString--) |  |
| [unprotect(String password)](#unprotect-java.lang.String-) | Снимает защиту с книги. |
| [unprotectSharedWorkbook(String password)](#unprotectSharedWorkbook-java.lang.String-) | Снимает защиту с общей книги. |
| [updateCustomFunctionDefinition(CustomFunctionDefinition definition)](#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Обновляет определение пользовательских функций. |
| [updateLinkedDataSource(Workbook[] externalWorkbooks)](#updateLinkedDataSource-com.aspose.cells.Workbook---) | Если эта книга содержит внешние ссылки на другие источники данных, Aspose.Cells попытается получить последние данные из указанных источников. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Workbook() {#Workbook--}
```
public Workbook()
```


Инициализирует новый экземпляр класса [Workbook](../../com.aspose.cells/workbook).

**Remarks**

Тип файла по умолчанию — Xlsx. Если вы хотите создавать другие типы файлов, используйте Workbook(FileFormatType).

**Example**

Следующий код показывает, как использовать конструктор Workbook для создания и инициализации нового экземпляра класса.

```
         Workbook workbook = new Workbook();
```

### Workbook(int fileFormatType) {#Workbook-int-}
```
public Workbook(int fileFormatType)
```


Инициализирует новый экземпляр класса [Workbook](../../com.aspose.cells/workbook).

**Remarks**

Тип файла по умолчанию — Excel97To2003.

**Example**

Следующий код показывает, как использовать конструктор Workbook для создания и инициализации нового экземпляра класса с различными типами форматов файлов.

```
         Workbook workbook = new Workbook(FileFormatType.XLSX);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileFormatType | int | [FileFormatType](../../com.aspose.cells/fileformattype). Новый формат файла. |

### Workbook(LoadOptions loadOptions) {#Workbook-com.aspose.cells.LoadOptions-}
```
public Workbook(LoadOptions loadOptions)
```


Инициализирует новый пустой экземпляр класса [Workbook](../../com.aspose.cells/workbook) с параметрами

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Опции. |

### Workbook(String file) {#Workbook-java.lang.String-}
```
public Workbook(String file)
```


Инициализирует новый экземпляр класса [Workbook](../../com.aspose.cells/workbook) и открывает файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| файл | java.lang.String | Имя файла. |

### Workbook(InputStream stream) {#Workbook-java.io.InputStream-}
```
public Workbook(InputStream stream)
```


Инициализирует новый экземпляр класса [Workbook](../../com.aspose.cells/workbook) и открывает поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | Поток. |

### Workbook(String file, LoadOptions loadOptions) {#Workbook-java.lang.String-com.aspose.cells.LoadOptions-}
```
public Workbook(String file, LoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [Workbook](../../com.aspose.cells/workbook) и открывает файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| файл | java.lang.String | Имя файла. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Параметры загрузки |

### Workbook(InputStream stream, LoadOptions loadOptions) {#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-}
```
public Workbook(InputStream stream, LoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [Workbook](../../com.aspose.cells/workbook) и открывает поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | Поток. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Параметры загрузки |

### acceptAllRevisions() {#acceptAllRevisions--}
```
public void acceptAllRevisions()
```


Принимает все отслеживаемые изменения в рабочей книге.

### addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Добавляет цифровую подпись в файл электронной таблицы OOXML (Excel2007 и новее).

**Remarks**

Поддерживается только добавление цифровой подписи Xmldsig в файл электронной таблицы OOXML

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Вычисляет результат формул.

**Remarks**

Для всех поддерживаемых формул, пожалуйста, смотрите список по адресу https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### calculateFormula(boolean ignoreError) {#calculateFormula-boolean-}
```
public void calculateFormula(boolean ignoreError)
```


Вычисляет результат формул.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ignoreError | boolean | Указывает, скрывать ли ошибку при вычислении формул. Ошибка может быть вызвана неподдерживаемой функцией, внешними ссылками и т.д. |

### calculateFormula(CalculationOptions options) {#calculateFormula-com.aspose.cells.CalculationOptions-}
```
public void calculateFormula(CalculationOptions options)
```


Вычисление формул в этой рабочей книге.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Параметры расчёта |

### changePalette(Color color, int index) {#changePalette-com.aspose.cells.Color-int-}
```
public void changePalette(Color color, int index)
```


Изменяет палитру электронной таблицы по указанному индексу.

**Remarks**

Палитра содержит 56 элементов, каждый представлен значением RGB.

Если установить цвет, которого нет в палитре, он не будет применён.

Поэтому, если вы хотите задать пользовательский цвет, сначала измените палитру.

Ниже представлена стандартная цветовая палитра.

| Color | Красный | Зелёный | Синий |
| ------- | --- | ----- | ---- |
| Чёрный | 0 | 0 | 0 |
| Белый | 255 | 255 | 255 |
| Красный | 255 | 0 | 0 |
| Лаймовый | 0 | 255 | 0 |
| Синий | 0 | 0 | 255 |
| Жёлтый | 255 | 255 | 0 |
| Пурпурный | 255 | 0 | 255 |
| Голубой | 0 | 255 | 255 |
| Бордовый | 128 | 0 | 0 |
| Зелёный | 0 | 128 | 0 |
| Темно-синий | 0 | 0 | 128 |
| Оливковый | 128 | 128 | 0 |
| Фиолетовый | 128 | 0 | 128 |
| Бирюзовый | 0 | 128 | 128 |
| Серебряный | 192 | 192 | 192 |
| Серый | 128 | 128 | 128 |
| Color17 | 153 | 153 | 255 |
| Color18 | 153 | 51 | 102 |
| Color19 | 255 | 255 | 204 |
| Color20 | 204 | 255 | 255 |
| Color21 | 102 | 0 | 102 |
| Цвет22 | 255 | 128 | 128 |
| Цвет23 | 0 | 102 | 204 |
| Цвет24 | 204 | 204 | 255 |
| Цвет25 | 0 | 0 | 128 |
| Цвет26 | 255 | 0 | 255 |
| Цвет27 | 255 | 255 | 0 |
| Цвет28 | 0 | 255 | 255 |
| Цвет29 | 128 | 0 | 128 |
| Цвет30 | 128 | 0 | 0 |
| Цвет31 | 0 | 128 | 128 |
| Цвет32 | 0 | 0 | 255 |
| Цвет33 | 0 | 204 | 255 |
| Цвет34 | 204 | 255 | 255 |
| Цвет35 | 204 | 255 | 204 |
| Цвет36 | 255 | 255 | 153 |
| Цвет37 | 153 | 204 | 255 |
| Цвет38 | 255 | 153 | 204 |
| Цвет39 | 204 | 153 | 255 |
| Цвет40 | 255 | 204 | 153 |
| Цвет41 | 51 | 102 | 255 |
| Цвет42 | 51 | 204 | 204 |
| Цвет43 | 153 | 204 | 0 |
| Цвет44 | 255 | 204 | 0 |
| Цвет45 | 255 | 153 | 0 |
| Цвет46 | 255 | 102 | 0 |
| Color47 | 102 | 102 | 153 |
| Color48 | 150 | 150 | 150 |
| Color49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Структура цвета. |
| индекс | int | Индекс палитры, 0 - 55. |

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Закрывает сеанс, использующий кэши для доступа к данным.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). параметры доступа к данным |

### combine(Workbook secondWorkbook) {#combine-com.aspose.cells.Workbook-}
```
public void combine(Workbook secondWorkbook)
```


Объединяет другой объект Workbook.

**Remarks**

Объединить Excel, ODS , CSV и другие файлы в один файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| secondWorkbook | [Workbook](../../com.aspose.cells/workbook) | Другой объект Workbook. |

### copy(Workbook source) {#copy-com.aspose.cells.Workbook-}
```
public void copy(Workbook source)
```


Копирует данные из исходного объекта Workbook.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Объект Source Workbook. |

### copy(Workbook source, CopyOptions copyOptions) {#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-}
```
public void copy(Workbook source, CopyOptions copyOptions)
```


Копирует другой объект Workbook.

**Remarks**

Клонировать файл Excel очень просто.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Объект Source Workbook. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Параметры копирования другой рабочей книги. |

### copyTheme(Workbook source) {#copyTheme-com.aspose.cells.Workbook-}
```
public void copyTheme(Workbook source)
```


Копирует тему из другой рабочей книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Исходный workbook. |

### createBuiltinStyle(int type) {#createBuiltinStyle-int-}
```
public Style createBuiltinStyle(int type)
```


Создаёт встроенный стиль указанного типа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [BuiltinStyleType](../../com.aspose.cells/builtinstyletype). Встроенный стиль stype. |

**Returns:**
[Style](../../com.aspose.cells/style) - [Style](../../com.aspose.cells/style) object
### createCellsColor() {#createCellsColor--}
```
public CellsColor createCellsColor()
```


Создаёт объект [CellsColor](../../com.aspose.cells/cellscolor).

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor) - Returns a [CellsColor](../../com.aspose.cells/cellscolor) object.
### createStyle() {#createStyle--}
```
public Style createStyle()
```


Создаёт новый стиль.

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### createStyle(boolean cloneDefaultStyle) {#createStyle-boolean-}
```
public Style createStyle(boolean cloneDefaultStyle)
```


Создаёт новый стиль.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cloneDefaultStyle | boolean | Указывает, клонирует ли стиль по умолчанию |

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### customTheme(String themeName, Color[] colors) {#customTheme-java.lang.String-com.aspose.cells.Color---}
```
public void customTheme(String themeName, Color[] colors)
```


Настраивает тему.

**Remarks**

Длина массива цветов должна быть 12.

| Индекс массива | Тип темы |
| ----------- | ------------------ |
| 0 | Фон1 |
| 1 | Текст1 |
| 2 | Фон2 |
| 3 | Текст2 |
| 4 | Акцент1 |
| 5 | Акцент2 |
| 6 | Акцент3 |
| 7 | Акцент4 |
| 8 | Акцент5 |
| 9 | Акцент6 |
| 10 | Гиперссылка |
| 11 | Отслеживаемая гиперссылка |

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| themeName | java.lang.String | Имя темы |
| colors | [Color\[\]](../../com.aspose.cells/color) | Тематические цвета |

### dispose() {#dispose--}
```
public void dispose()
```


Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов.

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
### exportXml(String mapName, OutputStream stream) {#exportXml-java.lang.String-java.io.OutputStream-}
```
public void exportXml(String mapName, OutputStream stream)
```


Экспортирует XML-данные, связанные указанной XML-картой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| mapName | java.lang.String | имя XML‑карты, которую нужно экспортировать |
| stream | java.io.OutputStream | поток экспорта |

### exportXml(String mapName, String path) {#exportXml-java.lang.String-java.lang.String-}
```
public void exportXml(String mapName, String path)
```


Экспортирует XML-данные, связанные указанной XML-картой.

**Example**

Следующий код экспортировал данные, связанные с первой XmlMap.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         //Make sure that the source xlsx file contains a XmlMap.
         XmlMap xmlMap = wb.getWorksheets().getXmlMaps().get(0);
 
         wb.exportXml(xmlMap.getName(), "output.xml");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| mapName | java.lang.String | имя XML‑карты, которую нужно экспортировать |
| путь | java.lang.String | путь экспорта |

### getAbsolutePath() {#getAbsolutePath--}
```
public String getAbsolutePath()
```


Получает абсолютный путь к файлу.

**Remarks**

Используется только для внешних ссылок.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Возвращает коллекцию [DocumentProperty](../../com.aspose.cells/documentproperty), представляющую все встроенные свойства документа электронной таблицы.

**Remarks**

Новый параметр нельзя добавить в список встроенных свойств документа. Можно только получить встроенное свойство и изменить его значение. Ниже приведён список имён встроенных свойств:

Title

Тема

Автор

Ключевые слова

Комментарии

Шаблон

Последний автор

Номер ревизии

Имя приложения

Дата последней печати

Дата создания

Время последнего сохранения

Общее время редактирования

Количество страниц

Количество слов

Количество символов

Безопасность

Категория

Формат

Менеджер

Компания

Количество байт

Количество строк

Количество абзацев

Количество слайдов

Количество заметок

Количество скрытых слайдов

Количество мультимедийных клипов

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getCellsDataTableFactory() {#getCellsDataTableFactory--}
```
public CellsDataTableFactory getCellsDataTableFactory()
```


Получает фабрику для создания ICellsDataTable из пользовательских объектов

**Returns:**
[CellsDataTableFactory](../../com.aspose.cells/cellsdatatablefactory)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColors() {#getColors--}
```
public Color[] getColors()
```


Возвращает цвета в палитре электронной таблицы.

**Remarks**

Палитра содержит 56 элементов, каждый представлен значением RGB.

**Returns:**
com.aspose.cells.Color[]
### getContentTypeProperties() {#getContentTypeProperties--}
```
public ContentTypePropertyCollection getContentTypeProperties()
```


Получает список объектов [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) в рабочей книге.

**Returns:**
[ContentTypePropertyCollection](../../com.aspose.cells/contenttypepropertycollection)
### getCountOfStylesInPool() {#getCountOfStylesInPool--}
```
public int getCountOfStylesInPool()
```


Получает количество стилей в пуле стилей.

**Returns:**
int
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Возвращает коллекцию [DocumentProperty](../../com.aspose.cells/documentproperty), представляющую все пользовательские свойства документа электронной таблицы.

**Example**

```
         Workbook excel = new Workbook();
         excel.getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getCustomXmlParts() {#getCustomXmlParts--}
```
public CustomXmlPartCollection getCustomXmlParts()
```


Представляет часть хранилища пользовательских XML‑данных (пользовательские XML‑данные внутри пакета).

**Returns:**
[CustomXmlPartCollection](../../com.aspose.cells/customxmlpartcollection)
### getDataConnections() {#getDataConnections--}
```
public ExternalConnectionCollection getDataConnections()
```


Получает коллекцию [ExternalConnection](../../com.aspose.cells/externalconnection).

**Returns:**
[ExternalConnectionCollection](../../com.aspose.cells/externalconnectioncollection)
### getDataMashup() {#getDataMashup--}
```
public DataMashup getDataMashup()
```


Получает данные mashup.

**Returns:**
[DataMashup](../../com.aspose.cells/datamashup)
### getDataModel() {#getDataModel--}
```
public DataModel getDataModel()
```


Получает модель данных в рабочей книге.

**Returns:**
[DataModel](../../com.aspose.cells/datamodel)
### getDataSorter() {#getDataSorter--}
```
public DataSorter getDataSorter()
```


Получает объект DataSorter для сортировки данных.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### getDefaultStyle() {#getDefaultStyle--}
```
public Style getDefaultStyle()
```


Получает объект [Style](../../com.aspose.cells/style) по умолчанию рабочей книги.

**Remarks**

Свойство DefaultStyle полезно для реализации стиля для всей Workbook.

**Example**

Следующий код создает и инициализирует новую Workbook и задает ей стиль по умолчанию [Style](../../com.aspose.cells/style).

```
         Workbook workbook = new Workbook();
         Style defaultStyle = workbook.getDefaultStyle();
         defaultStyle.getFont().setName("Tahoma");
         workbook.setDefaultStyle(defaultStyle);
```

**Returns:**
[Style](../../com.aspose.cells/style)
### getDigitalSignature() {#getDigitalSignature--}
```
public DigitalSignatureCollection getDigitalSignature()
```


Получает цифровую подпись из файла.

**Returns:**
[DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection)
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Получает формат файла.

Смотрите [FileFormatType](../../com.aspose.cells/fileformattype).

**Returns:**
int
### getFileName() {#getFileName--}
```
public String getFileName()
```


Получает текущее имя файла.

**Remarks**

Если файл открыт через поток и есть внешние ссылки на формулы, пожалуйста, укажите имя файла.

**Returns:**
java.lang.String
### getFonts() {#getFonts--}
```
public Font[] getFonts()
```


Получает все шрифты в пуле стилей.

**Returns:**
com.aspose.cells.Font[]
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Получает монитор прерываний.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getMatchingColor(Color rawColor) {#getMatchingColor-com.aspose.cells.Color-}
```
public Color getMatchingColor(Color rawColor)
```


Находит наиболее подходящий цвет в текущей палитре.

**Remarks**

В палитре цветов Excel 97-2003 содержится только 56 цветов. Если цвет отсутствует в палитре, будет установлен похожий цвет.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| rawColor | [Color](../../com.aspose.cells/color) | Исходный цвет. |

**Returns:**
[Color](../../com.aspose.cells/color) - Best matching color.
### getNamedStyle(String name) {#getNamedStyle-java.lang.String-}
```
public Style getNamedStyle(String name)
```


Получает именованный стиль в пуле стилей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | имя стиля |

**Returns:**
[Style](../../com.aspose.cells/style) - named style, maybe null.
### getRibbonXml() {#getRibbonXml--}
```
public String getRibbonXml()
```


Получает XML‑файл, определяющий пользовательский интерфейс Ribbon.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public WorkbookSettings getSettings()
```


Представляет настройки рабочей книги.

**Returns:**
[WorkbookSettings](../../com.aspose.cells/workbooksettings)
### getStyleInPool(int index) {#getStyleInPool-int-}
```
public Style getStyleInPool(int index)
```


Получает стиль из пула стилей. Все стили в книге будут собраны в пул. В ячейках хранится только простой индекс ссылки.

**Remarks**

Если изменён возвращённый стиль, стиль всех ячеек (которые ссылаются на этот стиль) будет изменён.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс. |

**Returns:**
[Style](../../com.aspose.cells/style) - The style in the pool corresponds to given index, may be null.
### getTheme() {#getTheme--}
```
public String getTheme()
```


Получает название темы.

**Returns:**
java.lang.String
### getThemeColor(int type) {#getThemeColor-int-}
```
public Color getThemeColor(int type)
```


Получает цвет темы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Тип цветовой темы. |

**Returns:**
[Color](../../com.aspose.cells/color) - The theme color.
### getVbaProject() {#getVbaProject--}
```
public VbaProject getVbaProject()
```


Получает [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) в электронной таблице.

**Returns:**
[VbaProject](../../com.aspose.cells/vbaproject)
### getWorksheets() {#getWorksheets--}
```
public WorksheetCollection getWorksheets()
```


Получает коллекцию [WorksheetCollection](../../com.aspose.cells/worksheetcollection) в электронной таблице.

**Returns:**
[WorksheetCollection](../../com.aspose.cells/worksheetcollection) - [WorksheetCollection](../../com.aspose.cells/worksheetcollection) collection
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Определяет, используется ли в этой рабочей книге пользовательская функция, например в формулах ячеек, в определённых именах...

**Returns:**
boolean
### hasExernalLinks() {#hasExernalLinks--}
```
public boolean hasExernalLinks()
```


Указывает, содержит ли эта рабочая книга внешние ссылки на другие источники данных.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого используйте ExternalLinkCollection.Count, чтобы проверить наличие внешних ссылок в этой книге. Этот метод будет удалён через 12 месяцев, начиная с декабря 2021 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

**Returns:**
boolean — содержит ли эта книга внешние ссылки на другие источники данных.
### hasMacro() {#hasMacro--}
```
public boolean hasMacro()
```


Указывает, содержит ли эта электронная таблица макросы/VBA.

**Returns:**
boolean
### hasRevisions() {#hasRevisions--}
```
public boolean hasRevisions()
```


Получает, есть ли в рабочей книге отслеживаемые изменения

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importXml(InputStream stream, String sheetName, int row, int col) {#importXml-java.io.InputStream-java.lang.String-int-int-}
```
public void importXml(InputStream stream, String sheetName, int row, int col)
```


Импортирует/обновляет XML‑файл данных в рабочую книгу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.InputStream | поток XML‑файла. |
| sheetName | java.lang.String | имя листа назначения. |
| строка | int | строка назначения. |
| col | int | целевой столбец. |

### importXml(String url, String sheetName, int row, int col) {#importXml-java.lang.String-java.lang.String-int-int-}
```
public void importXml(String url, String sheetName, int row, int col)
```


Импортирует/обновляет XML‑файл данных в рабочую книгу.

**Example**

Следующий код импортирует XML-данные в лист 'Sheet 1' в ячейку A1.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         wb.importXml("xml.xml", "Sheet1", 0, 0);
 
         wb.save("output.xlsx");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| url | java.lang.String | URL/путь XML‑файла. |
| sheetName | java.lang.String | имя листа назначения. |
| строка | int | целевой ряд |
| col | int | целевой столбец |

### isColorInPalette(Color color) {#isColorInPalette-com.aspose.cells.Color-}
```
public boolean isColorInPalette(Color color)
```


Проверяет, находится ли цвет в палитре электронной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Структура цвета. |

**Returns:**
логический тип — возвращает true, если этот цвет присутствует в палитре. В противном случае возвращает false.
### isDigitallySigned() {#isDigitallySigned--}
```
public boolean isDigitallySigned()
```


Указывает, подписана ли эта электронная таблица цифровой подписью.

**Returns:**
boolean
### isLicensed() {#isLicensed--}
```
public boolean isLicensed()
```


Указывает, установлен ли лицензионный ключ.

**Returns:**
boolean
### isWorkbookProtectedWithPassword() {#isWorkbookProtectedWithPassword--}
```
public boolean isWorkbookProtectedWithPassword()
```


Указывает, защищены ли структура или окно паролем.

**Returns:**
boolean
### mergeNamedStyles(Workbook source) {#mergeNamedStyles-com.aspose.cells.Workbook-}
```
public void mergeNamedStyles(Workbook source)
```


Объединяет именованные стили из другого файла Excel.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Другой файл |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### parseFormulas(boolean ignoreError) {#parseFormulas-boolean-}
```
public void parseFormulas(boolean ignoreError)
```


Разбирает все формулы, которые не были разобраны при загрузке из шаблонного файла или при установке в ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ignoreError | boolean | Игнорировать ли ошибку для недействительной формулы. Если формула недействительна и включено игнорирование ошибок, эта формула будет пропущена, и процесс продолжит разбор остальных формул, иначе будет выброшено исключение. |

### protect(int protectionType, String password) {#protect-int-java.lang.String-}
```
public void protect(int protectionType, String password)
```


Защищает рабочую книгу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| protectionType | int | [ProtectionType](../../com.aspose.cells/protectiontype). Тип защиты. |
| пароль | java.lang.String | Пароль для защиты книги. |

### protectSharedWorkbook(String password) {#protectSharedWorkbook-java.lang.String-}
```
public void protectSharedWorkbook(String password)
```


Защищает общую рабочую книгу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| пароль | java.lang.String | Пароль для защиты книги. |

### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Обновить связанные фигуры, все сводные таблицы и диаграммы с источником сводных данных.

### refreshDynamicArrayFormulas(boolean calculate) {#refreshDynamicArrayFormulas-boolean-}
```
public void refreshDynamicArrayFormulas(boolean calculate)
```


Обновляет формулы динамических массивов (распространяются в новый диапазон соседних ячеек в соответствии с текущими данными) Другие формулы в книге не будут вычисляться рекурсивно, даже если они использовались формулами динамических массивов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| вычислять | boolean | Выполнять ли вычисление и обновление значений ячеек для этих формул динамических массивов |

### refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts) {#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-}
```
public void refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)
```


Обновляет формулы динамических массивов (распространяются в новый диапазон соседних ячеек в соответствии с текущими данными)

**Remarks**

С учётом производительности мы не обновляем автоматически все формулы динамических массивов, когда меняется сама формула или данные, на которые она ссылается. Поэтому пользователю необходимо вызывать этот метод вручную после операций, которые могут влиять на формулы динамических массивов, таких как импорт/установка значений ячеек, вставка/удаление строк/столбцов/диапазонов и т.д.

Для большинства формул с функциями вычисление диапазона "spill" также требует вычисления самой формулы, поэтому обычно предпочтительно установить флаг "calculate" в значение true. Если формула проста, например ссылка на диапазон или массив (например "=C1:E5", "=\{1,2;3,4\}", ...), простая функция над диапазоном или массивом (например "=ABS(C1:E5)", "=1+\{1,2;3,4\}", ...), и все формулы будут вычислены позже (например с помощью [calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-)), то использование значения false для флага "calculate" может избежать двойного вычисления и повысить производительность.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| вычислять | boolean | Выполнять ли вычисление и обновление значений ячеек для этих формул динамических массивов |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Параметры вычисления формул |

### removeDigitalSignature() {#removeDigitalSignature--}
```
public void removeDigitalSignature()
```


Удаляет цифровую подпись из этой таблицы.

### removeExternalLinks() {#removeExternalLinks--}
```
public void removeExternalLinks()
```


Удаляет все внешние ссылки в книге.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте метод ExternalLinkCollection.Clear(). Этот метод будет удалён через 12 месяцев, начиная с декабря 2021 года. Aspose приносит извинения за любые причинённые неудобства.

### removeMacro() {#removeMacro--}
```
public void removeMacro()
```


Удаляет VBA/макрос из этой таблицы.

### removePersonalInformation() {#removePersonalInformation--}
```
public void removePersonalInformation()
```


Удаляет личную информацию.

### removeUnusedStyles() {#removeUnusedStyles--}
```
public void removeUnusedStyles()
```


Удалить все неиспользуемые стили.

### replace(boolean boolValue, Object newValue) {#replace-boolean-java.lang.Object-}
```
public int replace(boolean boolValue, Object newValue)
```


Заменяет значения ячеек новыми данными.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| boolValue | boolean | Логическое значение, которое будет заменено. |
| newValue | java.lang.Object | Новое значение. Может быть строкой, целым числом, типом double или значением DateTime. |

**Returns:**
int
### replace(int intValue, Object newValue) {#replace-int-java.lang.Object-}
```
public int replace(int intValue, Object newValue)
```


Заменяет значения ячеек новыми данными.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| intValue | int | Целочисленное значение, которое будет заменено. |
| newValue | java.lang.Object | Новое значение. Может быть строкой, целым числом, типом double или значением DateTime. |

**Returns:**
int
### replace(String placeHolder, double newValue) {#replace-java.lang.String-double-}
```
public int replace(String placeHolder, double newValue)
```


Заменяет значение ячейки новым числом с плавающей точкой.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double newValue = 100.0;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | java.lang.String | Заполнитель ячейки |
| newValue | double | Значение double для замены |

**Returns:**
int
### replace(String placeHolder, double[] newValues, boolean isVertical) {#replace-java.lang.String-double---boolean-}
```
public int replace(String placeHolder, double[] newValues, boolean isVertical)
```


Заменяет значения ячеек массивом чисел с плавающей точкой.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double[] newValues = new double[]{1.23, 2.56, 3.14159};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | java.lang.String | Заполнитель ячейки |
| newValues | double[] | Массив double для замены |
| isVertical | boolean | True - вертикально, False - горизонтально |

**Returns:**
int
### replace(String placeHolder, int newValue) {#replace-java.lang.String-int-}
```
public int replace(String placeHolder, int newValue)
```


Заменяет значение ячейки новым целым числом.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int newValue = 100;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | java.lang.String | Заполнитель ячейки |
| newValue | int | Целочисленное значение для замены |

**Returns:**
int
### replace(String placeHolder, int[] newValues, boolean isVertical) {#replace-java.lang.String-int---boolean-}
```
public int replace(String placeHolder, int[] newValues, boolean isVertical)
```


Заменяет значения ячеек массивом целых чисел.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int[] newValues = new int[]{1, 2, 3};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | java.lang.String | Заполнитель ячейки |
| newValues | int[] | Массив целых чисел для замены |
| isVertical | boolean | True - вертикально, False - горизонтально |

**Returns:**
int
### replace(String placeHolder, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String placeHolder, String newValue)
```


Заменяет значение ячейки новой строкой.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         workbook.replace("AnOldValue", "NewValue");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | java.lang.String | Заполнитель ячейки |
| newValue | java.lang.String | Строковое значение для замены |

**Returns:**
int
### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public int replace(String placeHolder, String newValue, ReplaceOptions options)
```


Заменяет значение ячейки новой строкой.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | java.lang.String | Заполнитель ячейки |
| newValue | java.lang.String | Строковое значение для замены |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Параметры замены |

**Returns:**
int
### replace(String placeHolder, String[] newValues, boolean isVertical) {#replace-java.lang.String-java.lang.String---boolean-}
```
public int replace(String placeHolder, String[] newValues, boolean isVertical)
```


Заменяет значение ячейки новым массивом строк.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         String[] newValues = new String[]{"Tom", "Alice", "Jerry"};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| placeHolder | java.lang.String | Заполнитель ячейки |
| newValues | java.lang.String[] | Массив строк для замены |
| isVertical | boolean | True - вертикально, False - горизонтально |

**Returns:**
int
### save(OutputStream stream, SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.cells.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions saveOptions)
```


Сохранить книгу в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток файла. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Параметры сохранения. |

### save(OutputStream stream, int saveFormat) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int saveFormat)
```


Сохранить книгу в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток файла. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Тип формата сохраняемого файла. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Сохранить книгу на диск.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String |  |

### save(String fileName, SaveOptions saveOptions) {#save-java.lang.String-com.aspose.cells.SaveOptions-}
```
public void save(String fileName, SaveOptions saveOptions)
```


Сохраняет книгу на диск.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Параметры сохранения. |

### save(String fileName, int saveFormat) {#save-java.lang.String-int-}
```
public void save(String fileName, int saveFormat)
```


Сохраняет книгу на диск.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Тип формата сохранения. |

### setAbsolutePath(String value) {#setAbsolutePath-java.lang.String-}
```
public void setAbsolutePath(String value)
```


Устанавливает абсолютный путь к файлу.

**Remarks**

Используется только для внешних ссылок.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setDefaultStyle(Style value) {#setDefaultStyle-com.aspose.cells.Style-}
```
public void setDefaultStyle(Style value)
```


Устанавливает объект [Style](../../com.aspose.cells/style) по умолчанию для книги.

**Remarks**

Свойство DefaultStyle полезно для реализации стиля для всей Workbook.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Устанавливает цифровую подпись для файла электронной таблицы (Excel2007 и новее).

**Remarks**

Поддерживается только добавление цифровой подписи Xmldsig

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### setEncryptionOptions(int encryptionType, int keyLength) {#setEncryptionOptions-int-int-}
```
public void setEncryptionOptions(int encryptionType, int keyLength)
```


Установить параметры шифрования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| encryptionType | int | [EncryptionType](../../com.aspose.cells/encryptiontype). Тип шифрования. |
| keyLength | int | Длина ключа. |

### setFileFormat(int value) {#setFileFormat-int-}
```
public void setFileFormat(int value)
```


Устанавливает формат файла.

Смотрите [FileFormatType](../../com.aspose.cells/fileformattype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFileName(String value) {#setFileName-java.lang.String-}
```
public void setFileName(String value)
```


Устанавливает текущее имя файла.

**Remarks**

Если файл открыт через поток и есть внешние ссылки на формулы, пожалуйста, укажите имя файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Устанавливает монитор прерываний.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setRibbonXml(String value) {#setRibbonXml-java.lang.String-}
```
public void setRibbonXml(String value)
```


Устанавливает XML‑файл, определяющий интерфейс Ribbon.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setThemeColor(int type, Color color) {#setThemeColor-int-com.aspose.cells.Color-}
```
public void setThemeColor(int type, Color color)
```


Устанавливает цвет темы

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Тип цветовой темы. |
| color | [Color](../../com.aspose.cells/color) | цвет темы |

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Запускает сеанс, использующий кэши для доступа к данным.

**Remarks**

Если кэш указанного доступа к данным требует, чтобы некоторые модели данных в листе были "только для чтения", то соответствующие модели данных во всех листах этой книги будут считаться "только для чтения", и пользователь не должен изменять их.

После завершения доступа к данным следует вызвать [closeAccessCache(int)](../../com.aspose.cells/workbook\#closeAccessCache-int-) с теми же параметрами, чтобы очистить все кэши и восстановить обычный режим доступа.



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). параметры доступа к данным |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Снимает защиту с книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| пароль | java.lang.String | Пароль для снятия защиты книги. |

### unprotectSharedWorkbook(String password) {#unprotectSharedWorkbook-java.lang.String-}
```
public void unprotectSharedWorkbook(String password)
```


Снимает защиту с общей книги.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| пароль | java.lang.String | Пароль для снятия защиты книги. |

### updateCustomFunctionDefinition(CustomFunctionDefinition definition) {#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void updateCustomFunctionDefinition(CustomFunctionDefinition definition)
```


Обновляет определение пользовательских функций.

**Remarks**

Этот метод может использоваться в некоторых специальных сценариях. Например, если пользователю нужны параметры некоторых пользовательских функций, вычисляемые в режиме массива, он может предоставить собственное определение с реализованным [CustomFunctionDefinition.getArrayModeParameters(String)](../../com.aspose.cells/customfunctiondefinition\#getArrayModeParameters-String-) для этих функций. После обновления данных формул указанные параметры будут автоматически вычисляться в режиме массива при расчёте соответствующих пользовательских функций.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| definition | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) | Специальное определение пользовательских функций для особых требований пользователя. |

### updateLinkedDataSource(Workbook[] externalWorkbooks) {#updateLinkedDataSource-com.aspose.cells.Workbook---}
```
public void updateLinkedDataSource(Workbook[] externalWorkbooks)
```


Если эта книга содержит внешние ссылки на другие источники данных, Aspose.Cells попытается получить последние данные из указанных источников.

**Remarks**

Если соответствующая внешняя ссылка не найдена для одной книги, эта книга будет игнорироваться. Поэтому, когда вы позже задаёте формулу с новой внешней ссылкой, которую планируете связать с игнорируемой книгой, связь не будет выполнена, пока вы не вызовете этот метод снова с этими книгами.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| externalWorkbooks | [Workbook\[\]](../../com.aspose.cells/workbook) | Книги, которые будут использоваться для обновления данных внешних ссылок, на которые ссылается эта книга. Соответствие этих книг внешним ссылкам определяется методами [getFileName()](../../com.aspose.cells/workbook\#getFileName--) и [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Пожалуйста, убедитесь, что для каждой книги метод [getFileName()](../../com.aspose.cells/workbook\#getFileName--) задан с правильным значением, чтобы они могли быть связаны с соответствующей внешней ссылкой. |

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

