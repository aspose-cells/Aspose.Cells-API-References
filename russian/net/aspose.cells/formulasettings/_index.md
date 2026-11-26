---
title: "Класс FormulaSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FormulaSettings. Параметры формул и вычислений"
type: docs
url: /ru/net/aspose.cells/formulasettings/
---
## FormulaSettings class

Настройки формул и вычислений.

```csharp
public class FormulaSettings
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CalculateOnOpen](../../aspose.cells/formulasettings/calculateonopen/) { get; set; } | Указывает, требуется ли приложению выполнить полное вычисление при открытии книги. |
| [CalculateOnSave](../../aspose.cells/formulasettings/calculateonsave/) { get; set; } | Указывает, следует ли пересчитывать книгу перед сохранением документа в режиме ручных вычислений. |
| [CalculationId](../../aspose.cells/formulasettings/calculationid/) { get; set; } | Указывает версию движка вычислений, используемого для расчёта значений в книге. |
| [CalculationMode](../../aspose.cells/formulasettings/calculationmode/) { get; set; } | Получает или задаёт режим вычисления книги в MS Excel. |
| [EnableCalculationChain](../../aspose.cells/formulasettings/enablecalculationchain/) { get; set; } | Указывает, включить ли цепочку вычислений для формул. По умолчанию — false. |
| [EnableIterativeCalculation](../../aspose.cells/formulasettings/enableiterativecalculation/) { get; set; } | Указывает, включить ли итеративные вычисления для разрешения циклических ссылок. |
| [ForceFullCalculation](../../aspose.cells/formulasettings/forcefullcalculation/) { get; set; } | Указывает, вычислять ли все формулы каждый раз при запуске вычисления. |
| [MaxChange](../../aspose.cells/formulasettings/maxchange/) { get; set; } | Максимальное изменение для разрешения циклической ссылки. |
| [MaxIteration](../../aspose.cells/formulasettings/maxiteration/) { get; set; } | Максимальное количество итераций для разрешения циклической ссылки. |
| [PrecisionAsDisplayed](../../aspose.cells/formulasettings/precisionasdisplayed/) { get; set; } | Указывает, должна ли точность вычисленного результата устанавливаться в соответствии с отображением при вычислении формул. |
| [PreservePaddingSpaces](../../aspose.cells/formulasettings/preservepaddingspaces/) { get; set; } | Указывает, сохранять ли пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaSettingsDemo
    {
        public static void FormulaSettingsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к настройкам формул книги
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Установка свойств
            formulaSettings.CalculateOnOpen = true;
            formulaSettings.CalculateOnSave = true;
            formulaSettings.ForceFullCalculation = false;
            formulaSettings.CalculationMode = CalcModeType.Automatic;
            formulaSettings.CalculationId = "0";
            formulaSettings.EnableIterativeCalculation = true;
            formulaSettings.MaxIteration = 100;
            formulaSettings.MaxChange = 0.001;
            formulaSettings.PrecisionAsDisplayed = false;
            formulaSettings.EnableCalculationChain = true;
            formulaSettings.PreservePaddingSpaces = false;

            // Сохраните книгу
            workbook.Save("FormulaSettingsExample.xlsx");
            workbook.Save("FormulaSettingsExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


