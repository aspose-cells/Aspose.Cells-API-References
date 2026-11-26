---
title: "SensitivityLabel.SiteId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SensitivityLabel. Представляет идентификатор сайта Azure Active Directory (Azure AD), соответствующий политике метки чувствительности, описывающей метку чувствительности"
type: docs
url: /ru/net/aspose.cells.metas/sensitivitylabel/siteid/
---
## SensitivityLabel.SiteId property

Представляет идентификатор сайта Azure Active Directory (Azure AD), соответствующий политике метки конфиденциальности, описывающей метку конфиденциальности.

```csharp
public string SiteId { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertySiteIdDemo
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

                // Продемонстрируйте получение начального значения SiteId
                Console.WriteLine("Initial SiteId: " + label.SiteId);

                // Установите SiteId в пример идентификатора сайта Azure AD
                label.SiteId = "a1b2c3d4-5678-90ef-ghij-klmnopqrstuv";
                Console.WriteLine("After setting SiteId: " + label.SiteId);

                // Измените SiteId, чтобы продемонстрировать, что он доступен для чтения и записи
                label.SiteId = "z9y8x7w6-5432-10uv-wxyz-abcdefghijkl";
                Console.WriteLine("Updated SiteId: " + label.SiteId);

                // Покажите, как SiteId связан с другими свойствами
                Console.WriteLine($"Label {label.Id} with SiteId {label.SiteId} is enabled: {label.IsEnabled}");

                // Сохраните книгу
                workbook.Save("SiteIdDemo.xlsx");
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

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


