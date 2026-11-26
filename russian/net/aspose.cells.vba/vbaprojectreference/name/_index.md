---
title: "VbaProjectReference.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProjectReference. Получает и задает имя ссылки"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreference/name/
---
## VbaProjectReference.Name property

Получает и задает имя ссылки.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyNameDemo
    {
        public static void Run()
        {
            // Создать книгу (VBA проект автоматически создаётся для файлов .xlsm)
            Workbook workbook = new Workbook(FileFormatType.Xlsm);
            
            // Добавить ссылку в VBA проект
            string referenceName = "MyReference";
            string referencePath = @"C:\Temp\MyLibrary.dll";
            workbook.VbaProject.References.AddRegisteredReference(referenceName, referencePath);

            // Получить доступ и проверить ссылку по свойству Name
            VbaProjectReferenceCollection references = workbook.VbaProject.References;
            for (int i = 0; i < references.Count; i++)
            {
                if (references[i].Name.Equals(referenceName))
                {
                    Console.WriteLine($"Found reference: {references[i].Name}");
                    break;
                }
            }

            // Сохраните книгу
            workbook.Save("VbaProjectReferenceDemo.xlsm");
        }
    }
}
```

### См. также

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


