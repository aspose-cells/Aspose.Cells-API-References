---
title: "PageSetup.SetFitToPages"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PageSetup method. Establece el número de páginas al que se escalará la hoja de cálculo cuando se imprima"
type: docs
url: /es/net/aspose.cells/pagesetup/setfittopages/
---
## PageSetup.SetFitToPages method

Establece el número de páginas al que se escalará la hoja de cálculo cuando se imprima.

```csharp
public void SetFitToPages(int wide, int tall)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ancho | Int32 | Páginas de ancho. |
| alto | Int32 | Alto en páginas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFitToPagesWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder al PageSetup de la primera hoja de cálculo
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Establecer la configuración de ajuste a páginas
            setup.SetFitToPages(2, 3);
            
            // Verificar y mostrar la configuración
            Console.WriteLine("IsPercentScale: " + setup.IsPercentScale);
            Console.WriteLine("FitToPagesWide: " + setup.FitToPagesWide);
            Console.WriteLine("FitToPagesTall: " + setup.FitToPagesTall);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


