---
title: "GridJsWorkbook.RedactFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridJsWorkbook. تنفذ التشويه على ملف Excel بناءً على مصفوفة من عمليات JSON."
type: docs
url: /ar/net/aspose.cells.gridjs/gridjsworkbook/redactfile/
---
## GridJsWorkbook.RedactFile method

ينفذ حذفًا على ملف Excel بناءً على مصفوفة من عمليات JSON.

```csharp
public void RedactFile(string excelFilePath, string uid, string[] arrayOfRedactionOpr)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| excelFilePath | String | مسار ملف Excel الذي سيتم تشويهّه. |
| uid | String | المعرّف الفريد لدفتر العمل. إذا كان null أو فارغًا، سيتم إنشاء معرف جديد بناءً على مسار الملف. |
| arrayOfRedactionOpr | String[] | مصفوفة من سلاسل JSON تمثل عمليات التشويه التي سيتم تطبيقها. |

### الاستثناءات

| استثناء | شرط |
| --- | --- |
| [GridCellException](../../gridcellexception/) | يُرمى عندما يحدث CellsException أثناء عملية التشويه. |
| استثناء | يُرمى عندما يحدث استثناء عام أثناء عملية التشويه. |

### انظر أيضًا

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


