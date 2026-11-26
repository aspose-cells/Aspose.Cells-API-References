---
title: "VbaModuleCollection.Remove"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VbaModuleCollection. Удаляет модуль для рабочего листа"
type: docs
url: /ru/net/aspose.cells.vba/vbamodulecollection/remove/
---
## Remove(Worksheet) {#remove}

Удаляет модуль для листа.

```csharp
public void Remove(Worksheet sheet)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| лист | Worksheet | Рабочий лист |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleCollectionMethodRemoveWithWorksheetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте модуль VBA к рабочему листу
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Получите коллекцию модулей VBA
            VbaModuleCollection modules = workbook.VbaProject.Modules;
            
            try
            {
                // Вызовите метод Remove с параметром рабочего листа
                modules.Remove(worksheet);
                
                Console.WriteLine("VBA module removed successfully for the specified worksheet.");
                
                // Проверьте, что модуль был удалён
                if (modules.Count == 0)
                {
                    Console.WriteLine("No VBA modules remain in the collection.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("VbaModuleRemoveWithWorksheetDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove_1}

Удалить модуль по имени

```csharp
public void Remove(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String |  |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            // Создайте книгу с макросом
            Workbook workbook = new Workbook();
            
            // Получить доступ к проекту VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Добавить новый модуль
            int index = vbaProject.Modules.Add(VbaModuleType.Procedural, "TestModule");
            
            // Добавьте некоторый код в модуль
            vbaProject.Modules[index].Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";
            
            // Сохраните книгу
            workbook.Save("output_with_module.xlsm");
            
            // Удалите модуль по имени
            vbaProject.Modules.Remove("TestModule");
            
            // Сохраните книгу после удаления
            workbook.Save("output_after_removal.xlsm");
        }
    }
}
```

### См. также

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


