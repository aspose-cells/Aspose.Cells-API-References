---
title: "VbaProjectReferenceCollection.AddRegisteredReference"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VbaProjectReferenceCollection. Добавить ссылку на библиотеку типов Automation"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/
---
## VbaProjectReferenceCollection.AddRegisteredReference method

Добавить ссылку на типовую библиотеку Automation.

```csharp
public int AddRegisteredReference(string name, string libid)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя ссылки. |
| libid | String | Идентификатор библиотеки типов Automation. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddRegisteredReferenceWithStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к проекту VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Добавить зарегистрированную ссылку на stdole
            vbaProject.References.AddRegisteredReference(
                "stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Сохраните книгу
            workbook.Save("output.xlsm");
        }
    }
}
```

### См. также

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


