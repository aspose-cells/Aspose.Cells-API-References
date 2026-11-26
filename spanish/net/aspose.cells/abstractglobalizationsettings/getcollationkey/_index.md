---
title: "AbstractGlobalizationSettings.GetCollationKey"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractGlobalizationSettings. Transforma la cadena en un objeto comparable según ciertas reglas de ordenación"
type: docs
url: /es/net/aspose.cells/abstractglobalizationsettings/getcollationkey/
---
## AbstractGlobalizationSettings.GetCollationKey method

Transforma la cadena en un objeto comparable según ciertas reglas de ordenación.

```csharp
public virtual IComparable GetCollationKey(string v, bool ignoreCase)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| v | String | El valor de cadena necesita compararse con otros. |
| ignoreCase | Booleano | si se ignora mayúsculas y minúsculas al comparar valores |

### Valor de retorno

El objeto puede usarse para comparar o ordenar valores de cadena

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractGlobalizationSettingsMethodGetCollationKeyWithStringBooleanDemo
    {
        public static void Run()
        {
            // Crear configuraciones de globalización personalizadas que sobrescriban el método GetCollationKey
            var settings = new CustomGlobalizationSettings();
            
            // Crear un libro de trabajo con configuraciones de globalización personalizadas
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Preparar la cadena para la clave de ordenación
            string inputString = "Sample Text";
            bool ignoreCase = true;

            try
            {
                // Llamar a GetCollationKey directamente
                IComparable collationKey = settings.GetCollationKey(inputString, ignoreCase);
                
                Console.WriteLine($"Original string: {inputString}");
                Console.WriteLine($"Collation key: {collationKey}");
                Console.WriteLine($"Ignore case: {ignoreCase}");

                // Demostrar el efecto utilizándolo en operaciones de hoja de cálculo
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // La ordenación usará GetCollationKey internamente
                DataSorter sorter = workbook.DataSorter;
                sorter.AddKey(0, SortOrder.Descending);

                sorter.Sort(worksheet.Cells, 0, 0, 2, 0);
                
                workbook.Save("GetCollationKeyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during GetCollationKey operation: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLowerInvariant() : v;
            }
        }

    }
}
```

### Ver también

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


