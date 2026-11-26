---
title: "VbaProjectReferenceCollection.AddProjectRefrernce"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VbaProjectReferenceCollection. Добавляет ссылку на внешний проект VBA"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/
---
## VbaProjectReferenceCollection.AddProjectRefrernce method

Добавляет ссылку на внешний VBA‑проект.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddProjectReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddProjectRefrernce(string name, string absoluteLibid, string relativeLibid)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя ссылки. |
| absoluteLibid | String | Идентификатор ссылочного проекта VBA с абсолютным путём. |
| relativeLibid | String | Идентификатор ссылочного проекта VBA с относительным путём. |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод VbaProjectReferenceCollection.AddProjectReferernce(). Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Компания Aspose приносит извинения за любые причинённые неудобства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddProjectRefrernceWithStringStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Инициализировать проект VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Добавьте ссылку на проект с абсолютными и относительными libid
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Отобразить количество ссылок
            Console.WriteLine("Total References: " + vbaProject.References.Count);
            
            // Сохраните книгу
            workbook.Save("VbaProjectReferenceExample.xlsm");
        }
    }
}
```

### См. также

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


