---
title: "WorkbookSettings.CheckExcelRestriction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "propiedad WorkbookSettings. Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena mayor a 32 K. Cuando ingresas un valor mayor a 32 K, como mediante Cell.PutValuestring, si esta propiedad es verdadera obtendrás una excepción. Si la propiedad es falsa aceptaremos tu cadena ingresada como valor de la celda, de modo que luego puedas exportar el valor completo a otros formatos de archivo como CSV. Sin embargo, si estableces un valor que no es válido para el formato de archivo Excel, no deberías guardar el libro como formato Excel más adelante. De lo contrario, podría haber errores inesperados en el archivo Excel generado."
type: docs
url: /es/net/aspose.cells/workbooksettings/checkexcelrestriction/
---
## WorkbookSettings.CheckExcelRestriction property

Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena superior a 32 K. Cuando introduces un valor superior a 32 K, como mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una excepción. Si esta propiedad es falsa, aceptaremos la cadena introducida como el valor de la celda, de modo que posteriormente puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que no es válido para el formato de archivo Excel, no deberías guardar el libro posteriormente en formato Excel. De lo contrario, podría producirse un error inesperado en el archivo Excel generado.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Desactivar la verificación de restricciones de Excel
            workbook.Settings.CheckExcelRestriction = false;
            
            // Inserta una cadena que exceda los límites normales de Excel
            string longString = new string('a', 40000);
            workbook.Worksheets[0].Cells["A1"].PutValue(longString);
            
            // Guarda y recarga para verificar que la restricción se haya omitido
            string tempFile = Guid.NewGuid().ToString() + ".txt";
            workbook.Save(tempFile, new TxtSaveOptions());
            
            Workbook loadedWorkbook = new Workbook(tempFile, new LoadOptions { CheckExcelRestriction = false });
            Console.WriteLine("String length: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue.Length);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


