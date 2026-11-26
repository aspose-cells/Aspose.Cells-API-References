---
title: "Класс Metered"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Metered класс. Предоставляет методы для установки metered‑ключа"
type: docs
url: /ru/net/aspose.cells/metered/
---
## Metered class

Предоставляет методы установки измеряемого ключа.

```csharp
public class Metered
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Metered](metered/)() | Инициализирует новый экземпляр этого класса. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetProductName](../../aspose.cells/metered/getproductname/)() | Получает название продукта |
| [SetMeteredKey](../../aspose.cells/metered/setmeteredkey/)(string, string) | Устанавливает metered public and private key. Если вы приобрели metered‑лицензию, при запуске приложения этот API должен быть вызван, обычно этого достаточно. Однако, если постоянно не удаётся загрузить данные о потреблении и прошло более 24 часов, лицензия будет переведена в статус оценки; чтобы избежать такой ситуации, следует регулярно проверять статус лицензии, и если он находится в статусе оценки, вызвать этот API снова. |
| static [GetConsumptionCredit](../../aspose.cells/metered/getconsumptioncredit/)() | Получает кредит потребления |
| static [GetConsumptionQuantity](../../aspose.cells/metered/getconsumptionquantity/)() | Получает размер файла потребления |
| static [IsMeteredLicensed](../../aspose.cells/metered/ismeteredlicensed/)() | Проверьте, лицензирован ли metered |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredDemo
    {
        public static void MeteredExample()
        {
            // Создайте экземпляр класса Metered
            Metered metered = new Metered();

            // Установите metered‑ключ
            string publicKey = "YourPublicKey";
            string privateKey = "YourPrivateKey";
            metered.SetMeteredKey(publicKey, privateKey);

            // Получите и отобразите название продукта
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Дополнительный код, демонстрирующий, как может использоваться экземпляр
            // Например, создание рабочей книги и её сохранение
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            workbook.Save("MeteredExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


