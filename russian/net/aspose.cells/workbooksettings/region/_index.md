---
title: "WorkbookSettings.Region"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает или задает региональные настройки для рабочей книги"
type: docs
url: /ru/net/aspose.cells/workbooksettings/region/
---
## WorkbookSettings.Region property

Получает или задает региональные настройки для книги.

```csharp
public CountryCode Region { get; set; }
```

### Примечания

1. Региональные настройки, используемые компонентом Aspose.Cells для рабочей книги, загруженной из шаблонного файла: i). Для файла XLS существуют поля, определённые для региональных настроек, и MS Excel сохраняет данные региональных настроек в файл при сохранении XLS‑файла. Поэтому мы используем сохранённый регион из шаблонного файла для рабочей книги. Если вы не хотите использовать регион, сохранённый в XLS‑файле, пожалуйста, сбросьте его на требуемый (например, CountryCode.Default) после загрузки шаблонного файла. И мы также сохраняем пользовательское значение (через этот метод) в файл при сохранении XLS‑файла. ii). Для других форматов файлов, таких как XLSX, XLSB… и т.д., в спецификации формата файла нет поля, определяющего региональные настройки. Поэтому мы используем региональные настройки среды приложения для рабочей книги. И пользовательское значение (через этот метод) не может быть сохранено в сгенерированных файлах этих форматов. 2. Для отображения в MS Excel: Применённые здесь региональные настройки могут действовать только во время выполнения с компонентом Aspose.Cells и не влияют при просмотре сгенерированного файла в MS Excel. Даже для сгенерированного XLS‑файла, в котором данные региональных настроек были сохранены, при просмотре/редактировании его в MS Excel регион, используемый MS Excel для форматирования, всегда берётся из стандартных региональных настроек среды, где запущен MS Excel, а не из сохранённого в файле. Это поведение MS Excel и его нельзя изменить программно.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRegionDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Japan;
            
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(44089); // Represents 2020-09-15
            
            Style style = cell.GetStyle();
            style.Custom = "[$-F800]yyyy年m月d日";
            cell.SetStyle(style);
            
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### См. также

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


