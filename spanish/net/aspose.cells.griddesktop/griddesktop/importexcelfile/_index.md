---
title: "GridDesktop.ImportExcelFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de GridDesktop. Importa desde un flujo de archivo Excel, incluyendo flujo de archivo en disco o flujo de memoria"
type: docs
url: /es/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Importa desde un flujo de archivo Excel, incluyendo flujo de archivo en disco o flujo de memoria.

```csharp
public void ImportExcelFile(Stream stream)
```

### Ejemplos

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

### Ver también

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Importa desde un flujo de archivo Excel, incluyendo flujo de archivo en disco o flujo de memoria.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | objeto de flujo. |
| runFormulas | Booleano | si es verdadero, este método invocará el método RunAllFormulas. |

### Ver también

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

Importa desde un archivo Excel.

```csharp
public void ImportExcelFile(string fileName)
```

### Ejemplos

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

### Ver también

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Importa desde un archivo Excel.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String | nombre del archivo excel. |
| runFormulas | Booleano | si es verdadero, este método invocará el método RunAllFormulas. |

### Ver también

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Importa desde un archivo Excel.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | flujo del archivo excel. |
| passwordtoOpen | String | la contraseña de apertura para el archivo que está cifrado. |
| passwordtoModify | String | la contraseña de modificación para el archivo que está protegido. |
| openasReadOnly | Booleano | si se debe abrir el archivo como solo lectura. |
| runFormulas | Booleano | si es verdadero, este método invocará el método RunAllFormulas. |

### Ver también

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

Importa desde un archivo Excel.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String | nombre del archivo excel. |
| passwordtoOpen | String | la contraseña de apertura para el archivo que está cifrado. |
| passwordtoModify | String | la contraseña de modificación para el archivo que está protegido. |
| openasReadOnly | Booleano | si se debe abrir el archivo como solo lectura. |
| runFormulas | Booleano | si es verdadero, este método invocará el método RunAllFormulas. |

### Ver también

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Importa una hoja de cálculo desde un archivo Excel.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String | nombre del archivo excel. |
| sheetIndex | Int32 | índice de la hoja a importar. |

### Ver también

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


