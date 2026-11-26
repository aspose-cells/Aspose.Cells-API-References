---
title: "WorksheetCollection.RegisterAddInFunction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Añade una función addin al libro de trabajo"
type: docs
url: /es/net/aspose.cells/worksheetcollection/registeraddinfunction/
---
## RegisterAddInFunction(string, string, bool) {#registeraddinfunction}

Agrega la función de complemento al libro de trabajo

```csharp
public int RegisterAddInFunction(string addInFile, string functionName, bool lib)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| addInFile | String | el archivo contiene las funciones addin |
| functionName | String | el nombre de la función addin |
| lib | Booleano | si el archivo addin proporcionado está en el directorio o subdirectorio de la biblioteca Workbook Add-In. Esta bandera entra en vigor y marca la diferencia cuando el addInFile proporcionado es una ruta relativa: true indica que la ruta es relativa a la biblioteca Add-In y false indica que la ruta es relativa a este Workbook. |

### Valor de retorno

ID de los datos que contienen la función addin proporcionada

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Obtener la primera hoja de cálculo
            Worksheet sheet = wb.Worksheets[0];
            
            // Establecer rutas de archivos de ejemplo (estos deberían existir en su entorno)
            string addInFile1 = Path.Combine("AddIns", "MyAddIn1.xlam");
            string addInFile2 = Path.Combine("AddIns", "MyAddIn2.xlam");
            
            // Registrar funciones add-in con diferentes parámetros
            int id1 = wb.Worksheets.RegisterAddInFunction(addInFile1, "MY_UDF1", false);
            int id2 = wb.Worksheets.RegisterAddInFunction(addInFile2, "MY_UDF2", true);
            
            // Utilizar las funciones registradas en celdas
            sheet.Cells["A1"].Formula = "=MY_UDF1()";
            sheet.Cells["A2"].Formula = "=MY_UDF2()";
            
            // Guarda el libro de trabajo
            wb.Save("RegisterAddInFunctionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RegisterAddInFunction(int, string) {#registeraddinfunction_1}

Agrega la función de complemento al libro de trabajo

```csharp
public string RegisterAddInFunction(int id, string functionName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| id | Int32 | ID de los datos que contienen funciones de complemento, se puede obtener mediante la primera llamada a `RegisterAddInFunction` para el mismo archivo de complemento. |
| functionName | String | el nombre de la función addin |

### Valor de retorno

URL del archivo de complemento que contiene funciones de complemento

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithInt32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Registrar la primera función de complemento y obtener su ID
            int functionId = workbook.Worksheets.RegisterAddInFunction("externallink1.xlam", "customfunc1", false);
            
            // Registrar la segunda función de complemento usando el mismo ID
            workbook.Worksheets.RegisterAddInFunction(functionId, "customfunc2");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Utilizar las funciones registradas en fórmulas
            cells["A1"].Formula = "=customfunc1()";
            cells["A2"].Formula = "=customfunc2()";
            
            // Guarda el libro de trabajo
            workbook.Save("RegisterAddInFunctionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


