---
title: "PowerQueryFormula.GroupName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormula. Obtiene el nombre del grupo que contiene esta fórmula Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformula/groupname/
---
## PowerQueryFormula.GroupName property

Obtiene el nombre del grupo que contiene esta fórmula de Power Query.

```csharp
public string GroupName { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una fórmula Power Query (simulada ya que no podemos crear PowerQueryFormulas reales directamente)
            // Normalmente cargarías desde un archivo existente con fórmulas Power Query
            string sourcePath = "example.xlsx";
            
            try
            {
                workbook = new Workbook(sourcePath);
                PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
                
                if (queries.Count > 0)
                {
                    Console.WriteLine("First Power Query Formula Group Name: " + queries[0].GroupName);
                    
                    // Demostrar el acceso a la propiedad GroupName
                    string groupName = queries[0].GroupName;
                    Console.WriteLine($"Group Name: {groupName}");
                    
                    // Guarde y vuelva a cargar para demostrar la persistencia
                    string destPath = "output.xlsx";
                    workbook.Save(destPath);
                    
                    Workbook workbook2 = new Workbook(destPath);
                    PowerQueryFormulaCollection queries2 = workbook2.DataMashup.PowerQueryFormulas;
                    if (queries2.Count > 0)
                    {
                        Console.WriteLine("After reload - Group Name: " + queries2[0].GroupName);
                    }
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the file.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
                Console.WriteLine("Please ensure the example.xlsx file exists and contains Power Query formulas.");
            }
        }
    }
}
```

### Ver también

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


