---
title: "AbstractLowCodeProtectionProvider.GetWorksheetProtectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractLowCodeProtectionProvider. Получает тип защиты для защиты указанного листа"
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetprotectiontype/
---
## AbstractLowCodeProtectionProvider.GetWorksheetProtectionType method

Получает тип защиты для защиты указанного листа.

```csharp
public virtual ProtectionType GetWorksheetProtectionType(string sheetName)
```

### Возвращаемое значение

Тип защиты для защиты указанного листа. None означает отсутствие защиты листа.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetProtectionTypeWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("newSheet");
            string name = worksheet.Name;
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                worksheet.Protect(protectionProvider.GetWorksheetProtectionType(name), protectionProvider.GetWorksheetPassword(name), "");
               
                // Отобразить результат
                Console.WriteLine($"Worksheet '{name}' protection type: {protectionProvider.GetWorksheetProtectionType(name)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error retrieving protection type: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("GetWorksheetProtectionTypeDemo.xlsx");
        }

        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override ProtectionType GetWorksheetProtectionType(string sheetName)
            {
                return ProtectionType.Structure;
            }

            public override string GetWorksheetPassword(string sheetName)
            {
                return $"aspose123_{sheetName}";
            }
        }

    }
    
}
```

### См. также

* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


