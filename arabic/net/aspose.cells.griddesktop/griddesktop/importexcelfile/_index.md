---
title: "GridDesktop.ImportExcelFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridDesktop. تستورد من تدفق ملف إكسل بما في ذلك تدفق ملف على القرص أو تدفق الذاكرة"
type: docs
url: /ar/net/aspose.cells.griddesktop/griddesktop/importexcelfile/
---
## ImportExcelFile(Stream) {#importexcelfile}

يستورد من تدفق ملف Excel، بما في ذلك تدفق ملف على القرص أو تدفق الذاكرة.

```csharp
public void ImportExcelFile(Stream stream)
```

### أمثلة

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

### انظر أيضًا

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, bool) {#importexcelfile_1}

يستورد من تدفق ملف Excel، بما في ذلك تدفق ملف على القرص أو تدفق الذاكرة.

```csharp
public void ImportExcelFile(Stream stream, bool runFormulas)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | كائن التدفق. |
| runFormulas | منطقي | إذا كان صحيحًا، ستستدعي هذه الطريقة طريقة RunAllFormulas. |

### انظر أيضًا

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string) {#importexcelfile_3}

يستورد من ملف Excel.

```csharp
public void ImportExcelFile(string fileName)
```

### أمثلة

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

### انظر أيضًا

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, bool) {#importexcelfile_4}

يستورد من ملف Excel.

```csharp
public void ImportExcelFile(string fileName, bool runFormulas)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | اسم ملف إكسل. |
| runFormulas | منطقي | إذا كان صحيحًا، ستستدعي هذه الطريقة طريقة RunAllFormulas. |

### انظر أيضًا

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(Stream, string, string, bool, bool) {#importexcelfile_2}

يستورد من ملف Excel.

```csharp
public void ImportExcelFile(Stream stream, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | تدفق ملف إكسل. |
| passwordtoOpen | String | كلمة المرور لفتح الملف المشفر. |
| passwordtoModify | String | كلمة المرور للتعديل للملف المحمي. |
| openasReadOnly | منطقي | ما إذا كان سيتم فتح الملف كقراءة فقط. |
| runFormulas | منطقي | إذا كان صحيحًا، ستستدعي هذه الطريقة طريقة RunAllFormulas. |

### انظر أيضًا

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, string, string, bool, bool) {#importexcelfile_6}

يستورد من ملف Excel.

```csharp
public void ImportExcelFile(string fileName, string passwordtoOpen, string passwordtoModify, 
    bool openasReadOnly, bool runFormulas)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | اسم ملف إكسل. |
| passwordtoOpen | String | كلمة المرور لفتح الملف المشفر. |
| passwordtoModify | String | كلمة المرور للتعديل للملف المحمي. |
| openasReadOnly | منطقي | ما إذا كان سيتم فتح الملف كقراءة فقط. |
| runFormulas | منطقي | إذا كان صحيحًا، ستستدعي هذه الطريقة طريقة RunAllFormulas. |

### انظر أيضًا

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ImportExcelFile(string, int) {#importexcelfile_5}

يستورد ورقة عمل من ملف إكسل.

```csharp
public void ImportExcelFile(string fileName, int sheetIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | اسم ملف إكسل. |
| sheetIndex | Int32 | فهرس الورقة التي سيتم استيرادها. |

### انظر أيضًا

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


