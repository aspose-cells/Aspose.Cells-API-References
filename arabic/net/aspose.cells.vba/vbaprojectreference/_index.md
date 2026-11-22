---
title: "الفئة VbaProjectReference"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Vba.VbaProjectReference. تمثل مرجع مشروع VBA"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreference/
---
## VbaProjectReference class

يمثل مرجع مشروع VBA.

```csharp
public class VbaProjectReference
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ExtendedLibid](../../aspose.cells.vba/vbaprojectreference/extendedlibid/) { get; set; } | يحصل ويضبط Libid الموسع للمرجع. |
| [Libid](../../aspose.cells.vba/vbaprojectreference/libid/) { get; set; } | يحصل ويضبط Libid للمرجع. |
| [Name](../../aspose.cells.vba/vbaprojectreference/name/) { get; set; } | يحصل ويضبط اسم المرجع. |
| [RelativeLibid](../../aspose.cells.vba/vbaprojectreference/relativelibid/) { get; set; } | يحصل ويضبط معرف مشروع VBA المشار إليه بمسار نسبي. |
| [Twiddledlibid](../../aspose.cells.vba/vbaprojectreference/twiddledlibid/) { get; set; } | يحصل ويضبط Libid المعدل للمرجع. |
| [Type](../../aspose.cells.vba/vbaprojectreference/type/) { get; } | يحصل على نوع هذا المرجع. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaprojectreference/copy/)(VbaProjectReference) |  |

### أمثلة

```csharp

[C#]

//إنشاء كائن Workbook
Workbook workbook = new Workbook();
 // تهيئة مشروع VBA.
VbaProject vbaProject = workbook.VbaProject;
// إضافة مرجع مشروع VBA
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//حفظ ملف Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Init VBA project.
Dim vbaProject as VbaProject  = workbook.VbaProject
'Add vba project reference
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
'Saving the Excel file
workbook.Save("book1.xlsm")
```

### انظر أيضًا

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


