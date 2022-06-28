---
title: SetDataSource
second_title: Справочник по Aspose.Cells для .NET API
description: Устанавливает источник данных объектаICellsDataTableaspose.cells/icellsdatatable.
type: docs
weight: 120
url: /ru/net/aspose.cells/workbookdesigner/setdatasource/
---
## SetDataSource(string, ICellsDataTable) {#setdatasource_5}

Устанавливает источник данных объекта[`ICellsDataTable`](../../icellsdatatable).

```csharp
public void SetDataSource(string dataSource, ICellsDataTable cellsDataTable)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dataSource | String | Имя источника данных. |
| cellsDataTable | ICellsDataTable | таблица данных. |

### Смотрите также

* interface [ICellsDataTable](../../icellsdatatable)
* class [WorkbookDesigner](../../workbookdesigner)
* пространство имен [Aspose.Cells](../../workbookdesigner)
* сборка [Aspose.Cells](../../../)

---

## SetDataSource(DataSet) {#setdatasource}

Устанавливает источник данных объекта DataSet.

```csharp
public void SetDataSource(DataSet dataSet)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dataSet | DataSet | Объект DataSet |

### Примеры

```csharp

[C#]

  //Создаем объект подключения, указываем информацию о провайдере и устанавливаем источник данных.
OleDbConnection con = new OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb");
  //Открываем объект подключения.
con.Open();
  //Создаем командный объект и указываем SQL-запрос.
OleDbCommand cmd = new OleDbCommand("Select * from [Order Details]", con);
  //Создаем объект адаптера данных.
OleDbDataAdapter da = new OleDbDataAdapter();
  //Указываем команду.
da.SelectCommand = cmd;
  //Создаем объект набора данных.
DataSet ds = new DataSet();
  //Заполняем набор данных записями таблицы.
da.Fill(ds, "Order Details");
  //Создаем таблицу данных относительно таблицы набора данных.
DataTable dt = ds.Tables["Order Details"];
  //Создать объект WorkbookDesigner.
WorkbookDesigner wd = new WorkbookDesigner();
  //Открываем файл шаблона (который содержит смарт-маркеры).
wd.Workbook = new Workbook("SmartMarker_Designer.xls");
  // Установите таблицу данных в качестве источника данных.
wd.SetDataSource(dt);
  //Обработка интеллектуальных маркеров для заполнения данными рабочих листов.
wd.Process(true);
  // Сохраняем файл Excel.
wd.Workbook.Save("outSmartMarker_Designer.xls");

[Visual Basic]

'Создаем объект подключения, указываем информацию о провайдере и устанавливаем источник данных.
Dim con As OleDbConnection = New OleDbConnection("provider=microsoft.jet.oledb.4.0;data source=Northwind.mdb")
'Открываем объект подключения.
con.Open()
'Создаем командный объект и указываем SQL-запрос.
Dim cmd As OleDbCommand = New OleDbCommand("Select * from [Order Details]", con)
'Создаем объект адаптера данных.
Dim da As OleDbDataAdapter = New OleDbDataAdapter()
'Указываем команду.
da.SelectCommand = cmd
'Создаем объект набора данных.
Dim ds As DataSet = New DataSet()
'Заполняем набор данных записями таблицы.
da.Fill(ds, "Order Details")
'Создаем таблицу данных относительно таблицы набора данных.
Dim dt As DataTable = ds.Tables("Order Details")
'Создать объект WorkbookDesigner.
Dim wd As WorkbookDesigner = New WorkbookDesigner()
'Откройте файл шаблона (который содержит смарт-маркеры).
Dim workbook As Workbook = New Workbook("SmartMarker_Designer.xls")
wd.Workbook = workbook
'Установите datatable в качестве источника данных.
wd.SetDataSource(dt)
'Обработайте смарт-маркеры, чтобы заполнить данные на рабочих листах.
wd.Process(True)
'Сохраняем файл Excel.
wd.Workbook.Save("outSmartMarker_Designer.xls")
```

### Смотрите также

* class [WorkbookDesigner](../../workbookdesigner)
* пространство имен [Aspose.Cells](../../workbookdesigner)
* сборка [Aspose.Cells](../../../)

---

## SetDataSource(DataTable) {#setdatasource_1}

Устанавливает источник данных объекта DataTable.

```csharp
public void SetDataSource(DataTable dataTable)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dataTable | DataTable | Объект DataTable |

### Смотрите также

* class [WorkbookDesigner](../../workbookdesigner)
* пространство имен [Aspose.Cells](../../workbookdesigner)
* сборка [Aspose.Cells](../../../)

---

## SetDataSource(string, DataView) {#setdatasource_6}

Устанавливает источник данных объекта DataView и привязывает его к имени источника данных.

```csharp
public void SetDataSource(string dataSourceName, DataView dataView)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dataSourceName | String | Имя источника данных. |
| dataView | DataView | Объект DataView. |

### Смотрите также

* class [WorkbookDesigner](../../workbookdesigner)
* пространство имен [Aspose.Cells](../../workbookdesigner)
* сборка [Aspose.Cells](../../../)

---

## SetDataSource(DataView) {#setdatasource_2}

Устанавливает источник данных объекта DataView.

```csharp
public void SetDataSource(DataView dataView)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dataView | DataView | Объект DataView |

### Смотрите также

* class [WorkbookDesigner](../../workbookdesigner)
* пространство имен [Aspose.Cells](../../workbookdesigner)
* сборка [Aspose.Cells](../../../)

---

## SetDataSource(string, IDataReader, int) {#setdatasource_7}

Устанавливает источник данных объекта IDataReader.

```csharp
public void SetDataSource(string name, IDataReader dataReader, int rowCount)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя карты источника данных. |
| dataReader | IDataReader | Объект IDataReader |
| rowCount | Int32 | Количество строк данных. Если смарт-маркер не содержит "noadd", мы должны вставлять строки по количеству строк для снижения производительности и динамически повторяющихся формул. -1 означает, что параметр бесполезен. |

### Смотрите также

* class [WorkbookDesigner](../../workbookdesigner)
* пространство имен [Aspose.Cells](../../workbookdesigner)
* сборка [Aspose.Cells](../../../)

---

## SetDataSource(string, object) {#setdatasource_8}

Устанавливает привязку данных к переменной.

```csharp
public void SetDataSource(string variable, object data)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| variable | String | Имя переменной, созданное с помощью смарт-маркера. |
| data | Object | Исходные данные. |

### Смотрите также

* class [WorkbookDesigner](../../workbookdesigner)
* пространство имен [Aspose.Cells](../../workbookdesigner)
* сборка [Aspose.Cells](../../../)

---

## SetDataSource(OleDbConnection) {#setdatasource_3}

Устанавливает источник данных объекта OleDbConnection.

```csharp
public void SetDataSource(OleDbConnection connection)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| connection | OleDbConnection | Объект OleDbConnection |

### Смотрите также

* class [WorkbookDesigner](../../workbookdesigner)
* пространство имен [Aspose.Cells](../../workbookdesigner)
* сборка [Aspose.Cells](../../../)

---

## SetDataSource(SqlConnection) {#setdatasource_4}

Устанавливает источник данных объекта SqlConnection.

```csharp
public void SetDataSource(SqlConnection connection)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| connection | SqlConnection | Объект SqlConnection |

### Смотрите также

* class [WorkbookDesigner](../../workbookdesigner)
* пространство имен [Aspose.Cells](../../workbookdesigner)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
