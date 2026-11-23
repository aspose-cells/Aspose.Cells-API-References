---
title: "Enum ShapePathPointValueType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Drawing.ShapePathPointValueType. Spécifie le type de valeur de l'objet ShapePathPoint"
type: docs
url: /fr/net/aspose.cells.drawing/shapepathpointvaluetype/
---
## ShapePathPointValueType enumeration

Spécifie le type de valeur de l'objet [`ShapePathPoint`](../shapepathpoint/)

```csharp
public enum ShapePathPointValueType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Position | `0` | Spécifie que le type de l'objet est les coordonnées de localisation. L'objet [`ShapePathPoint`](../shapepathpoint/) stocke les valeurs de coordonnées d'un point. |
| Angle | `1` | Spécifie que le type de l'objet est les repères d'angle. L'objet [`ShapePathPoint`](../shapepathpoint/) stocke les angles de début et de fin de l'arc. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointValueTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Démontrer les valeurs de l'énumération ShapePathPointValueType
                ShapePathPointValueType positionType = ShapePathPointValueType.Position;
                ShapePathPointValueType angleType = ShapePathPointValueType.Angle;

                // Afficher les valeurs d'énumération
                Console.WriteLine($"Position type value: {(int)positionType}");
                Console.WriteLine($"Angle type value: {(int)angleType}");

                // Vérifiez que les valeurs d'énumération correspondent aux constantes attendues
                Console.WriteLine($"Position equals 0: {positionType == ShapePathPointValueType.Position}");
                Console.WriteLine($"Angle equals 1: {angleType == ShapePathPointValueType.Angle}");

                Console.WriteLine("ShapePathPointValueType enum demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPointValueType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


