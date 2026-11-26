---
title: "Style.CultureCustom"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene y establece la cadena de patrón dependiente de la cultura para el formato numérico. Si no se ha establecido ningún formato numérico para este objeto, se devolverá null. Si el formato numérico es incorporado, se devolverá la cadena de patrón correspondiente al número incorporado."
type: docs
url: /es/net/aspose.cells/style/culturecustom/
---
## Style.CultureCustom property

Obtiene y establece la cadena de patrón dependiente de la cultura para el formato numérico. Si no se ha establecido un formato numérico para este objeto, se devolverá null. Si el formato numérico es incorporado, se devolverá la cadena de patrón correspondiente al número incorporado.

```csharp
public string CultureCustom { get; set; }
```

### Observaciones

Para el formato numérico incorporado, tanto el contenido del patrón (por ejemplo, un formato de fecha incorporado es "m/d/y" para algunas configuraciones regionales, pero para otras se convierte en "d/m/y") como el especificador de formato (por ejemplo, algunas configuraciones regionales utilizan un carácter distinto de 'y' para representar la parte del año en el formato de fecha) dependen de la cultura; para un formato personalizado especificado por el usuario, solo los especificadores de formato se cambian según la cultura, las demás partes del patrón de formato no se modificarán.

### Ejemplos

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCultureCustomDemo
    {
        public static void Run()
        {
            // Crea un libro de trabajo y establece la cultura húngara
            Workbook wb = new Workbook();
            wb.Settings.CultureInfo = new CultureInfo("hu-HU");

            // Obtén la primera celda y su estilo
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();

            // Establece un formato personalizado y demuestra la conversión CultureCustom
            string customFormat = "yyyy-MM-dd hh:mm:ss ddd dddd MMM MMMM MMMMM";
            string cultureCustomFormat = "éééé-hh-nn óó:pp:mm nnn nnnn hhh hhhh hhhhh";
            
            style.Custom = customFormat;
            Console.WriteLine("CultureCustom from Custom: " + style.CultureCustom);
            
            style.CultureCustom = cultureCustomFormat;
            Console.WriteLine("Custom from CultureCustom: " + style.Custom);

            // Aplica el estilo y demuestra el formato sensible a la cultura
            cell.SetStyle(style);
            cell.PutValue(47512); // January 29, 2030
            Console.WriteLine("Formatted value: " + cell.StringValue);

            // Demuestra una fórmula con formato cultural
            cell.Formula = "=TEXT(47512,\"" + cultureCustomFormat + "\")";
            wb.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.StringValue);
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


