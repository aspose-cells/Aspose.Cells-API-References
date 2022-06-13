---
title: ImportExcelFile
second_title: Справочник по Aspose.Cells для .NET API
description: Импорт из потока файлов Excel включая поток файлов на диске или поток памяти.
type: docs
weight: 730
url: /ru/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Импорт из потока файлов Excel, включая поток файлов на диске или поток памяти.

```csharp
public void ImportExcelFile(Stream stream)
```

### Примеры

```csharp
[C#]
private void button1_Click(object sender, System.EventArgs e)
{
	FileStream fs = new FileStream("d:\\bookx.xls", FileMode.Open);
	try
	{
		gridDesktop1.ImportExcelFile(fs);
	}
	catch(Exception ex)
	{
	}
	finally
	{
		fs.Close();
	}
}

[Visual Basic]
Private Sub menuItem1_Click(ByVal sender As System.Object, ByVal e As System.EventArgs) Handles menuItem6.Click
	Dim fs As FileStream =  New FileStream("d:\bookx.xls",FileMode.Open)
	Try
		gridDesktop1.ImportExcelFile(fs)
	Catch ex As Exception
		Throw ex
	Finally
		fs.Close()
	End Try
End Sub

```

### Смотрите также

* class [GridDesktop](../../griddesktop)
* пространство имен [Aspose.Cells.GridDesktop](../../griddesktop)
* сборка [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Импорт из потока файлов Excel, включая поток файлов на диске или поток памяти.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | объект потока. |
| runFormulas | Boolean | если true, этот метод вызовет метод RunAllFormulas. |

### Смотрите также

* class [GridDesktop](../../griddesktop)
* пространство имен [Aspose.Cells.GridDesktop](../../griddesktop)
* сборка [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

Импорт из файла Excel.

```csharp
public void ImportExcelFile(string fileName)
```

### Примеры

```csharp
[C#]
private void button1_Click(object sender, System.EventArgs e)
{
	gridDesktop1.ImportExcelFile("FinancialPlan.xls");
}

[Visual Basic]
Private Sub menuItem1_Click(ByVal sender As System.Object, ByVal e As System.EventArgs) Handles menuItem6.Click
	gridDesktop1.ImportExcelFile("FinancialPlan.xls")
End Sub

```

### Смотрите также

* class [GridDesktop](../../griddesktop)
* пространство имен [Aspose.Cells.GridDesktop](../../griddesktop)
* сборка [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Импорт из файла Excel.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | имя файла excel. |
| runFormulas | Boolean | если true, этот метод вызовет метод RunAllFormulas. |

### Смотрите также

* class [GridDesktop](../../griddesktop)
* пространство имен [Aspose.Cells.GridDesktop](../../griddesktop)
* сборка [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Импорт из файла Excel.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | поток файла excel. |
| passwordtoOpen | String | пароль для открытия зашифрованного файла. |
| passwordtoOpen | String | пароль для изменения защищенного файла. |
| openasReadOnly | Boolean | следует ли открывать файл как ReadOnly . |
| runFormulas | Boolean | если true, этот метод вызовет метод RunAllFormulas. |

### Смотрите также

* class [GridDesktop](../../griddesktop)
* пространство имен [Aspose.Cells.GridDesktop](../../griddesktop)
* сборка [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

Импорт из файла Excel.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | имя файла excel. |
| passwordtoOpen | String | пароль для открытия зашифрованного файла. |
| passwordtoOpen | String | пароль для изменения защищенного файла. |
| openasReadOnly | Boolean | следует ли открывать файл как ReadOnly . |
| runFormulas | Boolean | если true, этот метод вызовет метод RunAllFormulas. |

### Смотрите также

* class [GridDesktop](../../griddesktop)
* пространство имен [Aspose.Cells.GridDesktop](../../griddesktop)
* сборка [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Импорт рабочего листа из файла Excel.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | имя файла excel. |
| sheetIndex | Int32 | индекс импортируемого листа. |

### Смотрите также

* class [GridDesktop](../../griddesktop)
* пространство имен [Aspose.Cells.GridDesktop](../../griddesktop)
* сборка [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
