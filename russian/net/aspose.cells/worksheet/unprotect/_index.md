---
title: "Worksheet.Unprotect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Снимает защиту с листа"
type: docs
url: /ru/net/aspose.cells/worksheet/unprotect/
---
## Unprotect() {#unprotect}

Снимает защиту с листа.

```csharp
public void Unprotect()
```

### Примечания

Этот метод снимает защиту с листа, защищённого без пароля.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodUnprotectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Защитить лист паролем
            worksheet.Protect(ProtectionType.All, "password123", null);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);
            
            try
            {
                // Снять защиту с листа без пароля (должно не удаться)
                worksheet.Unprotect();
                Console.WriteLine("Worksheet unprotected without password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect without password: " + ex.Message);
            }

            try
            {
                // Снять защиту с листа с неверным паролем (должно не удаться)
                worksheet.Unprotect("wrongpassword");
                Console.WriteLine("Worksheet unprotected with wrong password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect with wrong password: " + ex.Message);
            }

            try
            {
                // Снимите защиту листа с правильным паролем
                worksheet.Unprotect("password123");
                Console.WriteLine("Worksheet successfully unprotected: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect: " + ex.Message);
            }
            
            // Сохранить результат
            workbook.Save("WorksheetMethodUnprotectDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Unprotect(string) {#unprotect_1}

Снимает защиту с листа.

```csharp
public void Unprotect(string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пароль | String | Пароль |

### Примечания

Если лист защищён без пароля, вы можете установить значение null или пустую строку в параметр password.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Защитите лист паролем и типом защиты по умолчанию
            worksheet.Protect(ProtectionType.All, "test", null);
            
            // Снимите защиту листа с паролем
            worksheet.Unprotect("test");
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


