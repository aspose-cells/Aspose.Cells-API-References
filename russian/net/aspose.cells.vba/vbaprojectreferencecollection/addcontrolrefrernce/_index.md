---
title: "VbaProjectReferenceCollection.AddControlRefrernce"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VbaProjectReferenceCollection. Добавьте ссылку на модифицированную типовую библиотеку и её расширенную типовую библиотеку"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/
---
## VbaProjectReferenceCollection.AddControlRefrernce method

Добавить ссылку на изменённую типовую библиотеку и её расширенную типовую библиотеку.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddControlReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddControlRefrernce(string name, string libid, string twiddledlibid, 
    string extendedLibid)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя ссылки. |
| libid | String | Идентификатор библиотеки типов Automation. |
| twiddledlibid | String | Идентификатор модифицированной типовой библиотеки |
| extendedLibid | String | Идентификатор расширенной типовой библиотеки |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод VbaProjectReferenceCollection.AddControlReferernce(). Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Компания Aspose приносит извинения за любые причинённые неудобства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddControlRefrernceWithStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            // Добавьте ссылку на элемент управления со всеми строковыми параметрами
            vbaProject.References.AddControlRefrernce(
                "MSForms",
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library",
                "twiddledLibid",
                "extendedLibid");

            Console.WriteLine("Control reference added successfully. Total references: " + vbaProject.References.Count);
            
            workbook.Save("VbaProjectWithControlReference.xlsm");
        }
    }
}
```

### См. также

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


