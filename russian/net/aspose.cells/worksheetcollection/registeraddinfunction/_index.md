---
title: "WorksheetCollection.RegisterAddInFunction"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WorksheetCollection метод. Добавляет функцию addin в книгу"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/registeraddinfunction/
---
## RegisterAddInFunction(string, string, bool) {#registeraddinfunction}

Добавляет функцию надстройки в книгу

```csharp
public int RegisterAddInFunction(string addInFile, string functionName, bool lib)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| addInFile | String | файл содержит функции addin |
| functionName | String | имя функции addin |
| lib | Boolean | является ли указанный файл addin в каталоге или подкаталоге библиотеки Workbook Add-In. Этот флаг вступает в силу и имеет значение, когда указанный addInFile имеет относительный путь: true обозначает, что путь относителен к библиотеке Add-In, а false обозначает, что путь относителен к этой книге. |

### Возвращаемое значение

Идентификатор данных, содержащих указанную функцию addin

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Получить первый лист
            Worksheet sheet = wb.Worksheets[0];
            
            // Установить примерные пути к файлам (они должны существовать в вашей среде)
            string addInFile1 = Path.Combine("AddIns", "MyAddIn1.xlam");
            string addInFile2 = Path.Combine("AddIns", "MyAddIn2.xlam");
            
            // Зарегистрировать функции add-in с разными параметрами
            int id1 = wb.Worksheets.RegisterAddInFunction(addInFile1, "MY_UDF1", false);
            int id2 = wb.Worksheets.RegisterAddInFunction(addInFile2, "MY_UDF2", true);
            
            // Использовать зарегистрированные функции в ячейках
            sheet.Cells["A1"].Formula = "=MY_UDF1()";
            sheet.Cells["A2"].Formula = "=MY_UDF2()";
            
            // Сохраните книгу
            wb.Save("RegisterAddInFunctionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RegisterAddInFunction(int, string) {#registeraddinfunction_1}

Добавляет функцию надстройки в книгу

```csharp
public string RegisterAddInFunction(int id, string functionName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| id | Int32 | Идентификатор данных, содержащих функции дополнения, можно получить при первом вызове `RegisterAddInFunction` для того же файла дополнения. |
| functionName | String | имя функции addin |

### Возвращаемое значение

URL файла дополнения, содержащего функции дополнения

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithInt32StringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Зарегистрировать первую функцию дополнения и получить её идентификатор
            int functionId = workbook.Worksheets.RegisterAddInFunction("externallink1.xlam", "customfunc1", false);
            
            // Зарегистрировать вторую функцию дополнения, используя тот же идентификатор
            workbook.Worksheets.RegisterAddInFunction(functionId, "customfunc2");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Использовать зарегистрированные функции в формулах
            cells["A1"].Formula = "=customfunc1()";
            cells["A2"].Formula = "=customfunc2()";
            
            // Сохраните книгу
            workbook.Save("RegisterAddInFunctionDemo.xlsx");
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


