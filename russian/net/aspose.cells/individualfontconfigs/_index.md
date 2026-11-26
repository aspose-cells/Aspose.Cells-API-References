---
title: "Класс IndividualFontConfigs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.IndividualFontConfigs. Конфигурации шрифтов для каждого объекта Workbook"
type: docs
url: /ru/net/aspose.cells/individualfontconfigs/
---
## IndividualFontConfigs class

Конфигурации шрифтов для каждого объекта [`Workbook`](../workbook/).

```csharp
public class IndividualFontConfigs
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [IndividualFontConfigs](individualfontconfigs/)() | Конструктор. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetFontSources](../../aspose.cells/individualfontconfigs/getfontsources/)() | Получает копию массива, содержащего список источников |
| [GetFontSubstitutes](../../aspose.cells/individualfontconfigs/getfontsubstitutes/)(string) | Возвращает массив, содержащий имена заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт не представлен. |
| [SetFontFolder](../../aspose.cells/individualfontconfigs/setfontfolder/)(string, bool) | Устанавливает папку шрифтов |
| [SetFontFolders](../../aspose.cells/individualfontconfigs/setfontfolders/)(string[], bool) | Устанавливает папки шрифтов |
| [SetFontSources](../../aspose.cells/individualfontconfigs/setfontsources/)(FontSourceBase[]) | Устанавливает источники шрифтов. |
| [SetFontSubstitutes](../../aspose.cells/individualfontconfigs/setfontsubstitutes/)(string, string[]) | Устанавливает имена заменяющих шрифтов для заданного оригинального имени шрифта. |

### Примеры

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIndividualFontConfigsDemo
    {
        public static void Run()
        {
            // Создаёт временные каталоги для источников шрифтов
            string tempFontFolder1 = Path.Combine(Path.GetTempPath(), "FontFolder1_" + Guid.NewGuid().ToString());
            string tempFontFolder2 = Path.Combine(Path.GetTempPath(), "FontFolder2_" + Guid.NewGuid().ToString());
            Directory.CreateDirectory(tempFontFolder1);
            Directory.CreateDirectory(tempFontFolder2);

            // Создаёт примерный CSV‑файл
            string csvFilePath = "sample_data.csv";
            File.WriteAllText(csvFilePath, "Name,Age\nJohn,30\nAlice,25", Encoding.UTF8);

            try
            {
                // Инициализирует конфигурацию шрифтов
                IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

                // Устанавливает заменяющие шрифты для Arial
                fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Verdana" });

                // Настраивает каталоги шрифтов
                fontConfigs.SetFontFolder(tempFontFolder1, false);
                fontConfigs.SetFontFolders(new string[] { tempFontFolder1, tempFontFolder2 }, true);

                // Настраивает источники шрифтов
                FontSourceBase[] fontSources = {
                    new FolderFontSource(tempFontFolder1, false),
                    new FolderFontSource(tempFontFolder2, true)
                };
                fontConfigs.SetFontSources(fontSources);

                // Создать параметры загрузки текста с конфигурациями шрифтов
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
                {
                    FontConfigs = fontConfigs
                };

                // Загрузить книгу с настроенными параметрами
                using (Workbook workbook = new Workbook(csvFilePath, loadOptions))
                {
                    // Сохранить как файл Excel
                    workbook.Save("output_with_font_config.xlsx");
                }
            }
            finally
            {
                // Очистить временные ресурсы
                if (Directory.Exists(tempFontFolder1)) Directory.Delete(tempFontFolder1, true);
                if (Directory.Exists(tempFontFolder2)) Directory.Delete(tempFontFolder2, true);
                if (File.Exists(csvFilePath)) File.Delete(csvFilePath);
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


