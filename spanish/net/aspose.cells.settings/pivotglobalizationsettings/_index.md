---
title: "Clase PivotGlobalizationSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Settings.PivotGlobalizationSettings. Representa la configuración de globalización para tablas dinámicas"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/
---
## PivotGlobalizationSettings class

Representa la configuración de globalización para tablas dinámicas.

```csharp
public class PivotGlobalizationSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PivotGlobalizationSettings](pivotglobalizationsettings/)() | El constructor predeterminado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [GetFormatOfDayGroup](../../aspose.cells.settings/pivotglobalizationsettings/getformatofdaygroup/)() | Obtiene el formato numérico del grupo de día de la tabla dinámica. Solo se usa al agrupar el campo dinámico por días. El valor predeterminado es "d-MMM"; |
| virtual [GetNameOfDataField](../../aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/)(ConsolidationFunction, string) | Obtiene el nombre para mostrar del campo de datos de la tabla dinámica. El formato predeterminado es "Sum Of Field". |
| virtual [GetShortTextOf12Months](../../aspose.cells.settings/pivotglobalizationsettings/getshorttextof12months/)() | Obtiene todas las cadenas de formato corto de los 12 meses. |
| virtual [GetTextOf24Hours](../../aspose.cells.settings/pivotglobalizationsettings/gettextof24hours/)() | Obtiene todas las cadenas formateadas localmente de las 24 horas. El valor predeterminado es 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM. |
| virtual [GetTextOf4Quarters](../../aspose.cells.settings/pivotglobalizationsettings/gettextof4quarters/)() | Obtiene el texto local de 4 trimestres. |
| virtual [GetTextOf4Quaters](../../aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/)() | (**Obsoleto.**) Obtiene el texto local de 4 trimestres. |
| virtual [GetTextOfAll](../../aspose.cells.settings/pivotglobalizationsettings/gettextofall/)() | Obtiene el texto de la etiqueta "(All)" en la tabla dinámica. |
| virtual [GetTextOfAllPeriods](../../aspose.cells.settings/pivotglobalizationsettings/gettextofallperiods/)() | Obtiene el texto localizado de "All Periods". |
| virtual [GetTextOfColumnLabels](../../aspose.cells.settings/pivotglobalizationsettings/gettextofcolumnlabels/)() | Obtiene el texto de la etiqueta "Column Labels" en la tabla dinámica. |
| virtual [GetTextOfDataFieldHeader](../../aspose.cells.settings/pivotglobalizationsettings/gettextofdatafieldheader/)() | Obtiene el texto del encabezado del campo del área de valores en la tabla dinámica. |
| virtual [GetTextOfDays](../../aspose.cells.settings/pivotglobalizationsettings/gettextofdays/)() | Obtiene el texto local de "Days". |
| virtual [GetTextOfEmptyData](../../aspose.cells.settings/pivotglobalizationsettings/gettextofemptydata/)() | Obtiene el texto de la etiqueta "(blank)" en la tabla dinámica. |
| virtual [GetTextOfGrandTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextofgrandtotal/)() | Obtiene el texto de la etiqueta "Grand Total" en la tabla dinámica. |
| virtual [GetTextOfHours](../../aspose.cells.settings/pivotglobalizationsettings/gettextofhours/)() | Obtiene el texto local de "Hours". |
| virtual [GetTextOfMinutes](../../aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/)() | Obtiene el texto local de "Minutes". |
| virtual [GetTextOfMonths](../../aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/)() | Obtiene el texto local de "Months". |
| virtual [GetTextOfMultipleItems](../../aspose.cells.settings/pivotglobalizationsettings/gettextofmultipleitems/)() | Obtiene el texto de la etiqueta "(Multiple Items)" en la tabla dinámica. |
| virtual [GetTextOfOr](../../aspose.cells.settings/pivotglobalizationsettings/gettextofor/)() | Obtiene todas las cadenas formateadas localmente de "or". |
| virtual [GetTextOfProtectedName](../../aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/)(string) | Obtiene el texto para el nombre protegido especificado. |
| virtual [GetTextOfProtection](../../aspose.cells.settings/pivotglobalizationsettings/gettextofprotection/)() | (**Obsolete.**) Obtiene el nombre de protección en la tabla dinámica. |
| virtual [GetTextOfQuarters](../../aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/)() | Obtén el texto local de "Quarters". |
| virtual [GetTextOfRange](../../aspose.cells.settings/pivotglobalizationsettings/gettextofrange/)() | Obtiene el texto local de "Range" |
| virtual [GetTextOfRowLabels](../../aspose.cells.settings/pivotglobalizationsettings/gettextofrowlabels/)() | Obtiene el texto de la etiqueta "Row Labels" en la tabla dinámica. |
| virtual [GetTextOfSeconds](../../aspose.cells.settings/pivotglobalizationsettings/gettextofseconds/)() | Obtiene el texto local de "Seconds" |
| virtual [GetTextOfSubTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextofsubtotal/)(PivotFieldSubtotalType) | Obtiene el texto del tipo [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) en la tabla dinámica. |
| virtual [GetTextOfTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextoftotal/)() | Obtiene el texto de la etiqueta "Total" en la tabla dinámica. Necesita sobrescribir este método cuando la tabla dinámica contiene dos o más PivotFields en el área de datos. |
| virtual [GetTextOfYears](../../aspose.cells.settings/pivotglobalizationsettings/gettextofyears/)() | Obtiene el texto local de "Years". |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGlobalizationSettingsDemo
    {
        public static void PivotGlobalizationSettingsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Fruit");
            worksheet.Cells["B4"].PutValue(150);
            worksheet.Cells["A5"].PutValue("Vegetable");
            worksheet.Cells["B5"].PutValue(250);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crear una instancia de PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demostrar el uso de varios métodos
            Console.WriteLine("Text of Total: " + globalizationSettings.GetTextOfTotal());
            Console.WriteLine("Text of Grand Total: " + globalizationSettings.GetTextOfGrandTotal());
            Console.WriteLine("Text of Multiple Items: " + globalizationSettings.GetTextOfMultipleItems());
            Console.WriteLine("Text of All: " + globalizationSettings.GetTextOfAll());
            Console.WriteLine("Text of Protection: " + globalizationSettings.GetTextOfProtection());
            Console.WriteLine("Text of Column Labels: " + globalizationSettings.GetTextOfColumnLabels());
            Console.WriteLine("Text of Row Labels: " + globalizationSettings.GetTextOfRowLabels());
            Console.WriteLine("Text of Empty Data: " + globalizationSettings.GetTextOfEmptyData());
            Console.WriteLine("Text of Data Field Header: " + globalizationSettings.GetTextOfDataFieldHeader());
            Console.WriteLine("Text of Years: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Text of Quarters: " + globalizationSettings.GetTextOfQuarters());
            Console.WriteLine("Text of Months: " + globalizationSettings.GetTextOfMonths());
            Console.WriteLine("Text of Days: " + globalizationSettings.GetTextOfDays());
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
            Console.WriteLine("Text of Range: " + globalizationSettings.GetTextOfRange());

            // Ejemplo del método GetTextOfProtectedName
            string protectedName = "ProtectedNameExample";
            Console.WriteLine("Text of Protected Name: " + globalizationSettings.GetTextOfProtectedName(protectedName));

            // Ejemplo del método GetTextOfSubTotal
            PivotFieldSubtotalType subTotalType = PivotFieldSubtotalType.Sum;
            Console.WriteLine("Text of SubTotal (Sum): " + globalizationSettings.GetTextOfSubTotal(subTotalType));

            // Guarda el libro de trabajo
            workbook.Save("PivotGlobalizationSettingsExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Settings](../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../)


