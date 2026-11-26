---
title: "Класс VbaProjectReference"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Vba.VbaProjectReference. Представляет ссылку на проект VBA"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreference/
---
## VbaProjectReference class

Представляет ссылку проекта VBA.

```csharp
public class VbaProjectReference
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ExtendedLibid](../../aspose.cells.vba/vbaprojectreference/extendedlibid/) { get; set; } | Получает и задает расширенный Libid ссылки. |
| [Libid](../../aspose.cells.vba/vbaprojectreference/libid/) { get; set; } | Получает и задает Libid ссылки. |
| [Name](../../aspose.cells.vba/vbaprojectreference/name/) { get; set; } | Получает и задает имя ссылки. |
| [RelativeLibid](../../aspose.cells.vba/vbaprojectreference/relativelibid/) { get; set; } | Получает и задает идентификатор ссылочного проекта VBA с относительным путем. |
| [Twiddledlibid](../../aspose.cells.vba/vbaprojectreference/twiddledlibid/) { get; set; } | Получает и задает изменённый (twiddled) Libid ссылки. |
| [Type](../../aspose.cells.vba/vbaprojectreference/type/) { get; } | Получает тип этой ссылки. |

## Методы

| Имя | Описание |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaprojectreference/copy/)(VbaProjectReference) |  |

### Примеры

```csharp

[C#]

//Создание объекта Workbook
Workbook workbook = new Workbook();
 // Инициализировать проект VBA.
VbaProject vbaProject = workbook.VbaProject;
// Добавить ссылку на проект VBA
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Сохранение файла Excel
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

### См. также

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


