---
title: "Name.GetReferredAreas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Name. Obtiene todas las referencias referidas por este nombre"
type: docs
url: /es/net/aspose.cells/name/getreferredareas/
---
## Name.GetReferredAreas method

Obtiene todas las referencias referidas por este nombre.

```csharp
public ReferredArea[] GetReferredAreas(bool recalculate)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| recalcular | Booleano | si recalcularlo si este nombre ya ha sido calculado antes de esta invocación. |

### Valor de retorno

Todos los rangos.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetReferredAreasWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook wb = new Workbook();
            
            // Agregar algunos datos a la hoja de cálculo
            wb.Worksheets[0].Cells[3, 3].PutValue("v03");
            
            // Crear un rango con nombre con múltiples referencias
            Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
            n.RefersTo = "='C:\\[extlink1.xlsx]Sheet1'!$A$1:$B$2,'C:\\[extlink2.xlsx]Sheet2'!$C$3,Sheet1!$D$4,'C:\\[extlink1.xlsx]Sheet1'!E5";
            
            // Obtener áreas referidas con enlaces externos
            ReferredArea[] ras = n.GetReferredAreas(true);
            
            // Mostrar información sobre cada área referida
            Console.WriteLine("Number of referred areas: " + ras.Length);
            for (int i = 0; i < ras.Length; i++)
            {
                ReferredArea ra = ras[i];
                Console.WriteLine($"\nArea {i + 1}:");
                Console.WriteLine($"IsExternalLink: {ra.IsExternalLink}");
                if (ra.IsExternalLink)
                {
                    Console.WriteLine($"ExternalFileName: {ra.ExternalFileName}");
                }
                Console.WriteLine($"SheetName: {ra.SheetName}");
                Console.WriteLine($"IsArea: {ra.IsArea}");
                
                if (ra.IsArea)
                {
                    Console.WriteLine($"Range: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}" +
                                    $" to {CellsHelper.CellIndexToName(ra.EndRow, ra.EndColumn)}");
                }
                else
                {
                    Console.WriteLine($"Cell: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}");
                }
            }
            
            // Crear un libro de trabajo externo y actualizar valores
            Workbook wb1 = new Workbook();
            wb1.Worksheets[0].Cells[0, 0].PutValue("v10");
            wb1.Worksheets[0].Cells[1, 1].PutValue("v11");
            wb1.Worksheets[0].Cells[4, 4].PutValue("v14");
            
            // Actualizar la fuente de datos vinculada
            wb.UpdateLinkedDataSource(new Workbook[]{wb1});
            
            // Mostrar algunos valores de las áreas referidas
            Console.WriteLine("\nValues from referred areas:");
            Console.WriteLine($"Area1[0,0]: {ras[0].GetValue(0, 0)}");
            Console.WriteLine($"Area1[1,1]: {ras[0].GetValue(1, 1)}");
            Console.WriteLine($"Area3[0,0]: {ras[2].GetValue(0, 0)}");
            Console.WriteLine($"Area4[0,0]: {ras[3].GetValue(0, 0)}");
        }
    }
}
```

### Ver también

* class [ReferredArea](../../referredarea/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


