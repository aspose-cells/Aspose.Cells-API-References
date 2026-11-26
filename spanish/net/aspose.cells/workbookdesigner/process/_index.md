---
title: "WorkbookDesigner.Process"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorkbookDesigner. Procesa los marcadores inteligentes y rellena los valores de la fuente de datos"
type: docs
url: /es/net/aspose.cells/workbookdesigner/process/
---
## Process(Range, bool) {#process_1}

Procesa los marcadores inteligentes y rellena los valores de la fuente de datos.

```csharp
[Obsolete("Use Range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Process(Range range, bool isPreserved)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | Rango | El rango a procesar |
| isPreserved | Booleano | Verdadero si el marcador inteligente no reconocido se conserva. |

### Observaciones

NOTA: Esta clase está ahora obsoleta. En su lugar, utilice los marcadores inteligentes Range. Esta propiedad será eliminada 12 meses después, a partir de julio de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithRangeBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = wb.Worksheets[0];
            
            // Crea datos de ejemplo en celdas
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("&=$Name");
            sheet.Cells["B2"].PutValue("&=$Value");
            
            // Crear diseñador de libros de trabajo
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = wb;
            
            // Crear fuente de datos JSON
            string jsonData = "{'Name':'Test Product','Value':100.50}";
            designer.SetJsonDataSource("Data", jsonData);
            
            // Procesar rango específico con marcadores inteligentes
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A2:B2");
            range.Name = "_CellsSmartMarkers";
            
            // Procesar el rango (true = procesar solo este rango)
            designer.Process(range, true);
            
            // Guardar el resultado
            wb.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process() {#process}

Procesa los marcadores inteligentes y rellena los valores de la fuente de datos.

```csharp
public void Process()
```

### Ejemplos

```csharp
using System;
using System.Collections;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir de un archivo de plantilla
            Workbook workbook = new Workbook("example.xlsx");
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // Preparar origen de datos
            ArrayList persons = new ArrayList();
            
            Person person1 = new Person("John Doe", 30);
            person1.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person1);

            Person person2 = new Person("Jane Smith", 28);
            person2.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person2);

            // Establecer origen de datos y procesar
            designer.SetDataSource("Datos", persons);
            designer.Process();

            // Guardar el resultado
            workbook.Save("output.xlsx");
        }
    }

    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public byte[] FOTO { get; set; }

        public Person(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(bool) {#process_2}

Procesa los marcadores inteligentes y rellena los valores de la fuente de datos.

```csharp
public void Process(bool isPreserved)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isPreserved | Booleano | Verdadero si el marcador inteligente no reconocido se conserva. |

### Ejemplos

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithBooleanDemo
    {
        public static void Run()
        {
            // Inicializar el libro de trabajo y cargar la plantilla
            Workbook workbook = new Workbook("example.xlsx");
            
            // Crear datos de muestra directamente en lugar de cargarlos desde JSON
            ABC_1_Data data = new ABC_1_Data
            {
                Directors = new List<Director>
                {
                    new Director { DRFNAME2 = "DRFNAME2" }
                }
            };

            // Configurar marcadores inteligentes
            workbook.Worksheets[0].Cells.CreateRange("A13:K19").Name = "_CellsSmartMarkers";

            // Preparar orígenes de datos
            List<ABC_1_Data> listData = new List<ABC_1_Data> { data };

            // Procesar el diseñador de libro de trabajo
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = workbook,
                LineByLine = false
            };
            
            designer.SetDataSource("RootData", listData);
            designer.SetDataSource("Directors", data.Directors);
            
            // Procesar con parámetro booleano
            designer.Process(true);
            
            // Guardar resultado
            workbook.Save("output.xlsx");
        }
    }

    // Clases de datos de muestra
    public class ABC_1_Data
    {
        public List<Director> Directors { get; set; }
    }

    public class Director
    {
        public string DRFNAME2 { get; set; }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(int, bool) {#process_3}

Procesa los marcadores inteligentes y rellena los valores de la fuente de datos.

```csharp
public void Process(int sheetIndex, bool isPreserved)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | Int32 | Índice de hoja de cálculo. |
| isPreserved | Booleano | Verdadero si el marcador inteligente no reconocido se conserva. |

### Observaciones

Este método funciona a nivel de hoja de cálculo.

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Exportar datos de la hoja de cálculo al DataTable
            Worksheet worksheet = workbook.Worksheets["Data"];
            DataTable dataTable = worksheet.Cells.ExportDataTable(
                0, 0, 
                worksheet.Cells.MaxDataRow, 
                worksheet.Cells.MaxDataColumn + 1, 
                new ExportTableOptions { 
                    CheckMixedValueType = true, 
                    ExportColumnName = true 
                });
            dataTable.TableName = "Table";

            // Crear diseñador de libro de trabajo y establecer origen de datos
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.SetDataSource(dataTable);

            // Procesar el diseñador con parámetros (Int32, Boolean)
            designer.Process(0, true);

            // Guardar el resultado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


