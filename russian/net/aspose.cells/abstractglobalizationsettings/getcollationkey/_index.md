---
title: "AbstractGlobalizationSettings.GetCollationKey"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractGlobalizationSettings. Преобразует строку в сравнимый объект согласно определённым правилам сортировки"
type: docs
url: /ru/net/aspose.cells/abstractglobalizationsettings/getcollationkey/
---
## AbstractGlobalizationSettings.GetCollationKey method

Преобразует строку в сравнимый объект в соответствии с определёнными правилами сортировки.

```csharp
public virtual IComparable GetCollationKey(string v, bool ignoreCase)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| v | String | Строковое значение должно сравниваться с другими. |
| ignoreCase | Boolean | нужно ли игнорировать регистр при сравнении значений |

### Возвращаемое значение

Объект может использоваться для сравнения или сортировки строковых значений

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractGlobalizationSettingsMethodGetCollationKeyWithStringBooleanDemo
    {
        public static void Run()
        {
            // Создать пользовательские настройки глобализации, переопределяющие метод GetCollationKey
            var settings = new CustomGlobalizationSettings();
            
            // Создать книгу с пользовательскими настройками глобализации
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Подготовить строку для ключа сортировки
            string inputString = "Sample Text";
            bool ignoreCase = true;

            try
            {
                // Вызвать GetCollationKey напрямую
                IComparable collationKey = settings.GetCollationKey(inputString, ignoreCase);
                
                Console.WriteLine($"Original string: {inputString}");
                Console.WriteLine($"Collation key: {collationKey}");
                Console.WriteLine($"Ignore case: {ignoreCase}");

                // Продемонстрировать эффект, используя в операциях листа
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Сортировка будет использовать GetCollationKey внутри
                DataSorter sorter = workbook.DataSorter;
                sorter.AddKey(0, SortOrder.Descending);

                sorter.Sort(worksheet.Cells, 0, 0, 2, 0);
                
                workbook.Save("GetCollationKeyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during GetCollationKey operation: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLowerInvariant() : v;
            }
        }

    }
}
```

### См. также

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


