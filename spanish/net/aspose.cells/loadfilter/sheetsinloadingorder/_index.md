---
title: "LoadFilter.SheetsInLoadingOrder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadFilter. Especifica los índices de las hojas y el orden a cargar. El valor predeterminado es null, lo que indica cargar todas las hojas en el orden predeterminado del archivo de plantilla. Si no es null y algún índice de hoja no está en la matriz devuelta, entonces la hoja no se cargará."
type: docs
url: /es/net/aspose.cells/loadfilter/sheetsinloadingorder/
---
## LoadFilter.SheetsInLoadingOrder property

Especifica las hojas (índices) y el orden que se cargarán. El valor predeterminado es null, lo que indica cargar todas las hojas en el orden predeterminado del archivo de plantilla. Si no es null y el índice de alguna hoja no está en la matriz devuelta, entonces esa hoja no se cargará.

```csharp
public virtual int[] SheetsInLoadingOrder { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertySheetsInLoadingOrderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con varias hojas
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Crear un filtro de carga personalizado
            LoadFilter loadFilter = new LoadFilter(LoadDataFilterOptions.All);
            
            // Mostrar el SheetsInLoadingOrder predeterminado (null significa cargar todas las hojas)
            Console.WriteLine("Initial SheetsInLoadingOrder is null: " + (loadFilter.SheetsInLoadingOrder == null));
            
            // Crear un archivo de plantilla para demostrar la carga con un orden de hoja personalizado
            workbook.Save("Template.xlsx");
            
            // Crear opciones de carga con nuestro filtro personalizado
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = loadFilter;
            
            // Cargar el libro de trabajo con la configuración predeterminada (todas las hojas)
            Workbook loadedWorkbook1 = new Workbook("Template.xlsx", loadOptions);
            Console.WriteLine("Sheets loaded with default filter: " + loadedWorkbook1.Worksheets.Count);
            
            // Crear un filtro nuevo con un orden de carga de hoja específico
            LoadFilter orderedFilter = new LoadFilter(LoadDataFilterOptions.All)
            {
                // Nota: SheetsInLoadingOrder es de solo lectura, por lo que necesitamos crear un filtro nuevo
                // con el orden deseado en el constructor o mediante otros medios
                // Esto demuestra la limitación de que la propiedad sea de solo lectura
            };
            
            // Dado que SheetsInLoadingOrder es de solo lectura, necesitaremos crear una subclase de LoadFilter
            // para demostrar un orden de carga de hoja personalizado
            CustomLoadFilter customFilter = new CustomLoadFilter(new int[] { 2, 0 }); // Load Sheet3 first, then Sheet1
            
            LoadOptions customLoadOptions = new LoadOptions();
            customLoadOptions.LoadFilter = customFilter;
            
            // Cargar libro de trabajo con orden de hoja personalizado
            Workbook loadedWorkbook2 = new Workbook("Template.xlsx", customLoadOptions);
            Console.WriteLine("Sheets loaded with custom filter: " + loadedWorkbook2.Worksheets.Count);
            Console.WriteLine("First sheet in custom order: " + loadedWorkbook2.Worksheets[0].Name);
        }
    }

    // Implementación personalizada de LoadFilter para demostrar la funcionalidad de SheetsInLoadingOrder
    public class CustomLoadFilter : LoadFilter
    {
        private readonly int[] _sheetsOrder;
        
        public CustomLoadFilter(int[] sheetsOrder) : base(LoadDataFilterOptions.All)
        {
            _sheetsOrder = sheetsOrder;
        }
        
        public override int[] SheetsInLoadingOrder => _sheetsOrder;
    }
}
```

### Ver también

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


