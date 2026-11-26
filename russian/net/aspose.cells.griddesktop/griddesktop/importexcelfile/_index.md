---
title: "GridDesktop.ImportExcelFile"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GridDesktop. Импортирует из потока Excel‑файла, включая поток файловой системы или поток памяти"
type: docs
url: /ru/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Импортирует из потока Excel‑файла, включая поток с диска или поток памяти.

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

### См. также

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Импортирует из потока Excel‑файла, включая поток с диска или поток памяти.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | объект потока. |
| runFormulas | Boolean | если true, этот метод вызовет метод RunAllFormulas. |

### См. также

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

Импортирует из Excel‑файла.

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

### См. также

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Импортирует из Excel‑файла.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | имя Excel‑файла. |
| runFormulas | Boolean | если true, этот метод вызовет метод RunAllFormulas. |

### См. также

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Импортирует из Excel‑файла.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | поток Excel‑файла. |
| passwordtoOpen | String | пароль для открытия зашифрованного файла. |
| passwordtoModify | String | пароль для изменения защищённого файла. |
| openasReadOnly | Boolean | открывать файл только для чтения. |
| runFormulas | Boolean | если true, этот метод вызовет метод RunAllFormulas. |

### См. также

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

Импортирует из Excel‑файла.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | имя Excel‑файла. |
| passwordtoOpen | String | пароль для открытия зашифрованного файла. |
| passwordtoModify | String | пароль для изменения защищённого файла. |
| openasReadOnly | Boolean | открывать файл только для чтения. |
| runFormulas | Boolean | если true, этот метод вызовет метод RunAllFormulas. |

### См. также

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Импортирует лист из файла Excel.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | String | имя Excel‑файла. |
| sheetIndex | Int32 | индекс листа для импорта. |

### См. также

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


