---
title: "CustomImplementationFactory.CreateCultureInfo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CustomImplementationFactory. Создаёт один CultureInfo по заданному идентификатору"
type: docs
url: /ru/net/aspose.cells/customimplementationfactory/createcultureinfo/
---
## CustomImplementationFactory.CreateCultureInfo method

Создайте один CultureInfo по заданному идентификатору.

```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| lcid | Int32 |  |

### Возвращаемое значение

Экземпляр CultureInfo.

### Примечания

Эта реализация полезна в следующих ситуациях: 1. Некоторые культуры могут не поддерживаться окружением пользователя, и создание требуемого CultureInfo с заданным идентификатором может вызвать исключение. Чтобы избежать исключения, пользователь может переопределить этот метод и предоставить действительный экземпляр CultureInfo для неподдерживаемой культуры. 2. Пользователь может захотеть указать некоторые пользовательские свойства для некоторых культур, чтобы получить ожидаемый результат форматирования. Для этой цели пользователь может переопределить этот метод и предоставить экземпляр CultureInfo с указанными пользователем свойствами. Обратите внимание, что свойство UseUserOverride возвращаемого экземпляра CultureInfo может влиять на отформатированный результат. Если оно равно false, некоторые свойства возвращаемого CultureInfo могут быть переопределены нашим встроенным движком форматирования в соответствии с требованиями разных сценариев. Если оно равно true, мы не будем изменять какие-либо его свойства и будем использовать его для прямого форматирования значений. Поэтому, если пользователь указал пользовательские свойства для возвращаемого CultureInfo, убедитесь, что его UseUserOverride установлено в true.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class CustomImplementationFactoryMethodCreateCultureInfoWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Вызовите CreateCultureInfo с действительным LCID (1033 для английского — США)
                int lcid = 1033;
                CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);

                // Отобразите результаты
                Console.WriteLine($"CultureInfo created successfully with LCID: {lcid}");
                Console.WriteLine($"Culture Name: {cultureInfo.Name}");
                Console.WriteLine($"Display Name: {cultureInfo.DisplayName}");
                Console.WriteLine($"English Name: {cultureInfo.EnglishName}");

                // Продемонстрируйте установку фабрики в CellsHelper
                CellsHelper.CustomImplementationFactory = factory;
                Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateCultureInfo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


