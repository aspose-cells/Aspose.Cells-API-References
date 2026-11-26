---
title: "Workbook.UpdateLinkedDataSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método del libro de trabajo. Si este libro de trabajo contiene enlaces externos a otra fuente de datos, Aspose.Cells intentará recuperar los datos más recientes de las fuentes dadas."
type: docs
url: /es/net/aspose.cells/workbook/updatelinkeddatasource/
---
## Workbook.UpdateLinkedDataSource method

Si este libro de trabajo contiene enlaces externos a otras fuentes de datos, Aspose.Cells intentará recuperar los datos más recientes de las fuentes dadas.

```csharp
public void UpdateLinkedDataSource(Workbook[] externalWorkbooks)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | Libros de trabajo que se utilizarán para actualizar los datos de los enlaces externos referenciados por este libro de trabajo. La coincidencia de esos libros de trabajo con los enlaces externos se determina mediante [`FileName`](../filename/) y [`DataSource`](../../externallink/datasource/). Por lo tanto, asegúrese de que [`FileName`](../filename/) se haya especificado con el valor correcto para cada libro de trabajo, de modo que puedan enlazarse al enlace externo correspondiente. |

### Observaciones

Si no se encuentra el enlace externo correspondiente para un libro de trabajo, ese libro de trabajo será ignorado. Por lo tanto, cuando establezca una fórmula más adelante con un nuevo enlace externo que desea que el libro de trabajo ignorado se vincule, el enlace no podrá realizarse hasta que vuelva a llamar a este método con esos libros de trabajo.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodUpdateLinkedDataSourceWithWorkbookDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo principal con referencias externas
            Workbook mainWorkbook = new Workbook();
            Worksheet mainSheet = mainWorkbook.Worksheets[0];
            mainSheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]Sheet1!A1";

            // Cree un libro de trabajo externo que será vinculado
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["A1"].Value = "Updated External Value";

            try
            {
                // Llame a UpdateLinkedDataSource con la matriz de libros de trabajo externos
                mainWorkbook.UpdateLinkedDataSource(new Workbook[] { externalWorkbook });

                // Calcule las fórmulas para actualizar la referencia
                mainWorkbook.CalculateFormula();

                // Mostrar el valor actualizado
                Console.WriteLine("Updated value in main workbook: " + mainSheet.Cells["A1"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UpdateLinkedDataSource method: {ex.Message}");
            }

            // Guardar el resultado
            mainWorkbook.Save("UpdateLinkedDataSourceDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


