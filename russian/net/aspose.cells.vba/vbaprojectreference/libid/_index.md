---
title: "VbaProjectReference.Libid"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProjectReference. Получает и задает Libid ссылки"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreference/libid/
---
## VbaProjectReference.Libid property

Получает и задает Libid ссылки.

```csharp
public string Libid { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyLibidDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook targetWorkbook = new Workbook();
            
            // Загрузить исходную книгу с проектом VBA
            Workbook sourceWorkbook = new Workbook("source.xlsm");
            
            // Очистить существующие ссылки в целевом объекте
            targetWorkbook.VbaProject.References.Clear();
            
            // Скопировать ссылки из источника в цель
            foreach (VbaProjectReference reference in sourceWorkbook.VbaProject.References)
            {
                if (reference.Type == VbaProjectReferenceType.Registered)
                {
                    // Продемонстрировать использование свойства Libid
                    targetWorkbook.VbaProject.References.AddRegisteredReference(reference.Name, reference.Libid);
                }
                else if (reference.Type == VbaProjectReferenceType.Control)
                {
                    targetWorkbook.VbaProject.References.AddControlRefrernce(
                        reference.Name, 
                        reference.Libid, 
                        reference.Twiddledlibid, 
                        reference.ExtendedLibid);
                }
            }
            
            // Сохранить результат
            targetWorkbook.Save("output.xlsm");
        }
    }
}
```

### См. также

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


