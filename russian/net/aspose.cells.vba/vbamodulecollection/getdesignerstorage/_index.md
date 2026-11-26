---
title: "VbaModuleCollection.GetDesignerStorage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод VbaModuleCollection. Представляет данные дизайнера"
type: docs
url: /ru/net/aspose.cells.vba/vbamodulecollection/getdesignerstorage/
---
## VbaModuleCollection.GetDesignerStorage method

Представляет данные дизайнера.

```csharp
public byte[] GetDesignerStorage(string name)
```

### Примечания

Мы не поддерживаем их разбор. Только для копирования.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodGetDesignerStorageWithStringDemo
    {
        public static void Run()
        {
            // Создайте книгу с проектом VBA
            Workbook workbook = new Workbook();
            
            // Добавьте модуль дизайнера
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Designer, "TestForm");
            
            // Получите хранилище дизайнера (по умолчанию будет null)
            byte[] storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Initial designer storage: " + (storage == null ? "null" : "exists"));
            
            // Добавьте некоторые данные хранилища дизайнера
            byte[] sampleData = new byte[] { 0x01, 0x02, 0x03 };
            workbook.VbaProject.Modules.AddDesignerStorage("TestForm", sampleData);
            
            // Получите и отобразите хранилище дизайнера
            storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Storage after adding: " + (storage == null ? "null" : BitConverter.ToString(storage)));
        }
    }
}
```

### См. также

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


