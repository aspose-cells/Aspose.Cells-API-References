---
title: "WorkbookSettings.Region"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene o establece la configuración regional para el libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbooksettings/region/
---
## WorkbookSettings.Region property

Obtiene o establece la configuración regional para el workbook.

```csharp
public CountryCode Region { get; set; }
```

### Observaciones

1. Configuración regional utilizada por el componente Aspose.Cells para un libro de trabajo cargado desde un archivo de plantilla: i). Para un archivo XLS, existen campos definidos para la configuración regional y MS Excel guarda los datos de configuración regional en el archivo al guardar el archivo XLS. Por lo tanto, utilizamos la región guardada en el archivo de plantilla para el libro de trabajo. Si no desea usar la región guardada en el archivo XLS, restáurela al valor esperado (por ejemplo, CountryCode.Default) después de cargar el archivo de plantilla. Además, guardamos el valor especificado por el usuario (mediante este método) en el archivo también al guardar un archivo XLS. ii). Para otros formatos de archivo, como XLSX, XLSB... etc., no hay un campo definido para la configuración regional en la especificación del formato de archivo. Por lo tanto, utilizamos la configuración regional del entorno de la aplicación para el libro de trabajo. Y el valor especificado por el usuario (mediante este método) no puede conservarse en los archivos generados con esos formatos. 2. Para el efecto de visualización en MS Excel: La configuración regional aplicada aquí solo puede tener efecto en tiempo de ejecución con el componente Aspose.Cells y no al visualizar el archivo generado con MS Excel. Incluso para el archivo XLS generado en el que se han guardado los datos de configuración regional especificados, al visualizar/editarlo con MS Excel, la región utilizada por MS Excel para realizar el formato es siempre la configuración regional predeterminada del entorno donde se ejecuta MS Excel, no la que está guardada en el archivo. Es un comportamiento de MS Excel y no puede ser modificado mediante código.

### Ejemplos

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

### Ver también

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


