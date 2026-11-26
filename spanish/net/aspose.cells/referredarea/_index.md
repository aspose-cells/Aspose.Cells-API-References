---
title: "Clase ReferredArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.ReferredArea class. Representa un área referida por la fórmula"
type: docs
url: /es/net/aspose.cells/referredarea/
---
## ReferredArea class

Representa un área referida por la fórmula.

```csharp
public class ReferredArea
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [EndColumn](../../aspose.cells/referredarea/endcolumn/) { get; } | La columna final del área. |
| [EndRow](../../aspose.cells/referredarea/endrow/) { get; } | La fila final del área. |
| [ExternalFileName](../../aspose.cells/referredarea/externalfilename/) { get; } | Obtener el nombre del archivo externo si es una referencia externa. |
| [IsArea](../../aspose.cells/referredarea/isarea/) { get; } | Indica si esto es un área. |
| [IsEntireColumn](../../aspose.cells/referredarea/isentirecolumn/) { get; } | Indica si este área contiene todas las filas (columna completa). |
| [IsEntireRow](../../aspose.cells/referredarea/isentirerow/) { get; } | Indica si esta área contiene todas las columnas (fila completa). |
| [IsExternalLink](../../aspose.cells/referredarea/isexternallink/) { get; } | Indica si es un enlace externo. |
| [SheetName](../../aspose.cells/referredarea/sheetname/) { get; } | Indica en qué hoja se encuentra esta referencia. |
| [SheetNames](../../aspose.cells/referredarea/sheetnames/) { get; } | Nombres de todas las hojas de cálculo a las que hace referencia esta instancia. |
| [StartColumn](../../aspose.cells/referredarea/startcolumn/) { get; } | La columna inicial del área. |
| [StartRow](../../aspose.cells/referredarea/startrow/) { get; } | La fila inicial del área. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue)(int, int) | Obtiene el valor de la celda con el desplazamiento dado desde la esquina superior izquierda de esta área. |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue_1)(int, int, bool) | Obtiene el valor de la celda con el desplazamiento dado desde la esquina superior izquierda de esta área. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues)() | Obtiene los valores de las celdas en esta área. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues_1)(bool) | Obtiene los valores de las celdas en esta área. |
| override [ToString](../../aspose.cells/referredarea/tostring/)() | Devuelve la dirección de referencia de esta área. Generalmente es la dirección de la referencia que puede usarse en una fórmula, como "Sheet1!A1:C3". |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassReferredAreaDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Configura algunos datos y una fórmula que haga referencia a un rango
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["B1"].PutValue(30);
                worksheet.Cells["B2"].PutValue(40);

                // Crea una fórmula que haga referencia al rango A1:B2
                Cell formulaCell = worksheet.Cells["C1"];
                formulaCell.Formula = "=SUM(A1:B2)";

                // Obtén las áreas referenciadas de la fórmula
                ReferredAreaCollection referredAreas = formulaCell.GetPrecedents();
                if (referredAreas.Count > 0)
                {
                    // Obtén la primera área referenciada
                    ReferredArea referredArea = referredAreas[0];

                    // Muestra las propiedades básicas del área referenciada
                    Console.WriteLine($"Referred Area Details:");
                    Console.WriteLine($"- Is External Link: {referredArea.IsExternalLink}");
                    Console.WriteLine($"- Sheet Name: {referredArea.SheetName}");
                    Console.WriteLine($"- Start Row: {referredArea.StartRow}");
                    Console.WriteLine($"- Start Column: {referredArea.StartColumn}");
                    Console.WriteLine($"- End Row: {referredArea.EndRow}");
                    Console.WriteLine($"- End Column: {referredArea.EndColumn}");
                    Console.WriteLine($"- Is Area: {referredArea.IsArea}");
                    Console.WriteLine($"- Is Entire Row: {referredArea.IsEntireRow}");
                    Console.WriteLine($"- Is Entire Column: {referredArea.IsEntireColumn}");

                    // Obtén valores del área referenciada
                    object values = referredArea.GetValues();
                    if (values is Array)
                    {
                        object[][] valueArray = (object[][])values;
                        Console.WriteLine("\nValues in the referred area:");
                        foreach (object[] row in valueArray)
                        {
                            foreach (object val in row)
                            {
                                Console.Write($"{val}\t");
                            }
                            Console.WriteLine();
                        }
                    }

                    // Obtén un valor específico del área referenciada
                    object specificValue = referredArea.GetValue(0, 1);
                    Console.WriteLine($"\nValue at row 0, column 1: {specificValue}");

                    // Muestra la dirección de referencia
                    Console.WriteLine($"Reference address: {referredArea.ToString()}");
                }

                // Guarda el libro de trabajo
                workbook.Save("ReferredAreaDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReferredArea: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


