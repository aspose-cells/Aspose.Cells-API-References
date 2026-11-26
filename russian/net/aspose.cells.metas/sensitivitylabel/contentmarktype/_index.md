---
title: "SensitivityLabel.ContentMarkType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SensitivityLabel. Получает и задаёт типы маркировки содержимого, которые должны применяться к файлу"
type: docs
url: /ru/net/aspose.cells.metas/sensitivitylabel/contentmarktype/
---
## SensitivityLabel.ContentMarkType property

Получает и задает типы маркировки контента, которые должны быть применены к файлу.

```csharp
public SensitivityLabelMarkType ContentMarkType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyContentMarkTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создайте экземпляр метки чувствительности
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Установите базовые свойства
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // Продемонстрировать свойство ContentMarkType (чтение‑запись)
                Console.WriteLine("Initial ContentMarkType: " + label.ContentMarkType);
                
                // Установите различные типы маркировки содержимого
                label.ContentMarkType = SensitivityLabelMarkType.Header;
                Console.WriteLine("After setting Header: " + label.ContentMarkType);
                
                label.ContentMarkType = SensitivityLabelMarkType.Watermark;
                Console.WriteLine("After setting Watermark: " + label.ContentMarkType);
                
                // Показать использование комбинированных флагов
                label.ContentMarkType = SensitivityLabelMarkType.Header | SensitivityLabelMarkType.Footer;
                Console.WriteLine("Combined Header+Footer: " + label.ContentMarkType);
                
                // Сохраните книгу
                workbook.Save("ContentMarkTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


