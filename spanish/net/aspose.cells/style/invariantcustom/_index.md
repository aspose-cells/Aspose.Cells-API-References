---
title: "Style.InvariantCustom"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene la cadena de patrón independiente de la cultura para el formato numérico. Si no se ha establecido ningún formato numérico para este objeto, se devolverá null. Si el formato numérico es incorporado, se devolverá la cadena de patrón correspondiente al número incorporado."
type: docs
url: /es/net/aspose.cells/style/invariantcustom/
---
## Style.InvariantCustom property

Obtiene la cadena de patrón independiente de la cultura para el formato numérico. Si no se ha establecido un formato numérico para este objeto, se devolverá null. Si el formato numérico es incorporado, se devolverá la cadena de patrón correspondiente al número incorporado.

```csharp
public string InvariantCustom { get; }
```

### Observaciones

Para los formatos numéricos incorporados, el contenido del patrón devuelto sigue siendo dependiente de la cultura, por ejemplo, para algunas configuraciones regionales devuelve "m/d/y" y para otras devuelve "d/m/y". La diferencia con [`CultureCustom`](../culturecustom/) es (eso también es lo que significa independiente de la cultura): los especificadores y separadores de formato se mantienen como estándar, de modo que '/' siempre se usará como separador de fecha y hora y "y" siempre se usará como la parte de "año" sin importar qué otro carácter especial se utilice para la configuración regional específica.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyInvariantCustomDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            
            // Establecer formato y valor de fecha
            style.Number = 14; // Date format
            style.Custom = "dd/MM/yyyy"; // Set custom format which affects both CultureCustom and InvariantCustom
            cell.PutValue(new DateTime(2019, 10, 12));
            cell.SetStyle(style);

            // Mostrar resultados
            Console.WriteLine("Formatted value: " + cell.StringValue);
            Console.WriteLine("CultureCustom: " + style.CultureCustom);
            Console.WriteLine("InvariantCustom: " + style.InvariantCustom);
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


