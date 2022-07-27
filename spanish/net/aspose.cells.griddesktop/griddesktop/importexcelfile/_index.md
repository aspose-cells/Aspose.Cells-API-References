---
title: ImportExcelFile
second_title: Referencia de API de Aspose.Cells para .NET
description: Importaciones desde una secuencia de archivos de Excel incluida la secuencia de archivos de disco o la secuencia de memoria.
type: docs
weight: 730
url: /es/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

Importaciones desde una secuencia de archivos de Excel, incluida la secuencia de archivos de disco o la secuencia de memoria.

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

* class [GridDesktop](../../griddesktop)
* espacio de nombres [Aspose.Cells.GridDesktop](../../griddesktop)
* asamblea [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

Importaciones desde una secuencia de archivos de Excel, incluida la secuencia de archivos de disco o la secuencia de memoria.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | objeto de flujo. |
| runFormulas | Boolean | si es verdadero, este método invocará el método RunAllFormulas. |

### Ver también

* class [GridDesktop](../../griddesktop)
* espacio de nombres [Aspose.Cells.GridDesktop](../../griddesktop)
* asamblea [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

Importaciones desde un archivo de Excel.

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

* class [GridDesktop](../../griddesktop)
* espacio de nombres [Aspose.Cells.GridDesktop](../../griddesktop)
* asamblea [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

Importaciones desde un archivo de Excel.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileName | String | nombre de archivo de Excel. |
| runFormulas | Boolean | si es verdadero, este método invocará el método RunAllFormulas. |

### Ver también

* class [GridDesktop](../../griddesktop)
* espacio de nombres [Aspose.Cells.GridDesktop](../../griddesktop)
* asamblea [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

Importaciones desde un archivo de Excel.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | flujo de archivo de Excel. |
| passwordtoOpen | String | la contraseña abierta para el archivo que está encriptado. |
| passwordtoOpen | String | la contraseña de modificación para el archivo que está protegido. |
| openasReadOnly | Boolean | si abrir el archivo como ReadOnly . |
| runFormulas | Boolean | si es verdadero, este método invocará el método RunAllFormulas. |

### Ver también

* class [GridDesktop](../../griddesktop)
* espacio de nombres [Aspose.Cells.GridDesktop](../../griddesktop)
* asamblea [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

Importaciones desde un archivo de Excel.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileName | String | nombre de archivo de Excel. |
| passwordtoOpen | String | la contraseña abierta para el archivo que está encriptado. |
| passwordtoOpen | String | la contraseña de modificación para el archivo que está protegido. |
| openasReadOnly | Boolean | si abrir el archivo como ReadOnly . |
| runFormulas | Boolean | si es verdadero, este método invocará el método RunAllFormulas. |

### Ver también

* class [GridDesktop](../../griddesktop)
* espacio de nombres [Aspose.Cells.GridDesktop](../../griddesktop)
* asamblea [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

Importa una hoja de cálculo desde un archivo de Excel.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileName | String | nombre de archivo de Excel. |
| sheetIndex | Int32 | índice de la hoja a importar. |

### Ver también

* class [GridDesktop](../../griddesktop)
* espacio de nombres [Aspose.Cells.GridDesktop](../../griddesktop)
* asamblea [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
