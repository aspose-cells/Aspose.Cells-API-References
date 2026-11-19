---
title: "DataLabels"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection de tous les objets DataLabel pour la série spécifiée."
type: docs
url: /fr/java/com.aspose.cells/datalabels/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class DataLabels extends ChartTextFrame
```

Encapsule une collection de tous les objets DataLabel pour la série spécifiée.

**Example**

```
         //Set the DataLabels in the chart
         Workbook wb = new Workbook("chart.xlsx");
         Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
         DataLabels datalabels;
         for (int i = 0; i  <chart.getNSeries().getCount(); i++)
         {
             datalabels = chart.getNSeries().get(i).getDataLabels();
             //Set the position of DataLabels
             datalabels.setPosition(LabelPositionType.INSIDE_BASE);
             //Show the category name in the DataLabels
             datalabels.setShowCategoryName(true);
             //Show the value in the DataLabels
             datalabels.setShowValue(true);
             //Not show the percentage in the DataLabels
             datalabels.setShowPercentage(false);
             //Not show the legend key.
             datalabels.setShowLegendKey(false);
         }
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [applyFont()](#applyFont--) | Appliquer la police des étiquettes de données à tous les nœuds enfants. |
| [characters(int startIndex, int length)](#characters-int-int-) | Renvoie un objet Characters qui représente une plage de caractères dans le texte. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Obtient le [getArea()](../../com.aspose.cells/datalabels\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. |
| [getBackground()](#getBackground--) | Obtient le mode d'affichage de l'arrière‑plan. |
| [getBackgroundMode()](#getBackgroundMode--) | Obtient le mode d'affichage de l'arrière-plan |
| [getBorder()](#getBorder--) | Obtient le [Line](../../com.aspose.cells/line). |
| [getChart()](#getChart--) | Obtient le graphique auquel cet objet appartient. |
| [getClass()](#getClass--) |  |
| [getDefaultHeight()](#getDefaultHeight--) | Représente la hauteur de la position par défaut en unités de 1/4000 de la zone du graphique. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--) | Représente la hauteur de la position par défaut en unités de la fraction de la zone du graphique. |
| [getDefaultWidth()](#getDefaultWidth--) | Représente la largeur de la position par défaut en unités de 1/4000 de la zone du graphique. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--) | Représente la largeur de la position par défaut en unités de fraction de la zone du graphique. |
| [getDefaultX()](#getDefaultX--) | Représente x de la position par défaut en unités de 1/4000 de la zone du graphique. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--) | Représente x de la position par défaut en unités de fraction de la zone du graphique. |
| [getDefaultY()](#getDefaultY--) | Représente y de la position par défaut en unités de 1/4000 de la zone du graphique. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--) | Représente y de la position par défaut en unités de la fraction de la zone du graphique. |
| [getDirectionType()](#getDirectionType--) | Obtient la direction du texte. |
| [getFont()](#getFont--) | Obtient la police des DataLabels ; |
| [getHeight()](#getHeight--) | Obtient la hauteur du cadre en unités de 1/4000 de la zone du graphique. |
| [getHeightPixel()](#getHeightPixel--) | Obtient la hauteur du cadre en unités de pixels. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Obtient la hauteur du cadre en unités du rapport de la zone du graphique. |
| [getLinkedSource()](#getLinkedSource--) | Obtient une référence à la feuille de calcul. |
| [getNumber()](#getNumber--) | Obtient le format numérique intégré. |
| [getNumberFormat()](#getNumberFormat--) | Représente la chaîne de format pour l'objet DataLabels. |
| [getNumberFormatLinked()](#getNumberFormatLinked--) | Vrai si le format numérique est lié aux cellules (de sorte que le format numérique change dans les étiquettes lorsqu'il change dans les cellules). |
| [getPosition()](#getPosition--) | Représente la position de l'étiquette de données. |
| [getReadingOrder()](#getReadingOrder--) | Représente l'ordre de lecture du texte. |
| [getRotationAngle()](#getRotationAngle--) | Représente l'angle de rotation du texte. |
| [getSeparatorType()](#getSeparatorType--) | Obtient le type de séparateur utilisé pour les étiquettes de données sur un graphique. |
| [getSeparatorValue()](#getSeparatorValue--) | Obtient la valeur du séparateur utilisée pour les étiquettes de données sur un graphique. |
| [getShadow()](#getShadow--) | Vrai si le cadre possède une ombre. |
| [getShapeProperties()](#getShapeProperties--) | Obtient l'objet [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getShapeType()](#getShapeType--) | Obtient le type de forme de l'étiquette de données. |
| [getShowBubbleSize()](#getShowBubbleSize--) | Représente le comportement d'affichage de la valeur de pourcentage de l'étiquette de données d'un graphique spécifié. |
| [getShowCategoryName()](#getShowCategoryName--) | Représente le comportement d'affichage du nom de catégorie de l'étiquette de données d'un graphique spécifié. Vrai pour afficher le nom de catégorie pour les étiquettes de données sur un graphique. |
| [getShowCellRange()](#getShowCellRange--) | Indique s'il faut afficher la plage de cellules comme les étiquettes de données. |
| [getShowLegendKey()](#getShowLegendKey--) | Représente le comportement d'affichage de la clé de légende de l'étiquette de données d'un graphique spécifié. |
| [getShowPercentage()](#getShowPercentage--) | Représente le comportement d'affichage de la valeur de pourcentage de l'étiquette de données d'un graphique spécifié. |
| [getShowSeriesName()](#getShowSeriesName--) | Indique si le nom de la série s'affiche sur les étiquettes de données d'un graphique. |
| [getShowValue()](#getShowValue--) | Représente le comportement d'affichage des valeurs de l'étiquette de données d'un graphique spécifié. |
| [getText()](#getText--) | Obtient le texte de l'étiquette de données. |
| [getTextDirection()](#getTextDirection--) | Représente l'ordre de lecture du texte. |
| [getTextFont()](#getTextFont--) | Obtient un objet [getFont()](../../com.aspose.cells/chartframe\#getFont--) du cadre de graphique spécifié. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Obtient l'alignement horizontal du texte. |
| [getTextOptions()](#getTextOptions--) | Obtient les options du texte. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Obtient l'alignement vertical du texte. |
| [getWidth()](#getWidth--) | Obtient la largeur du cadre en unités de 1/4000 de la zone du graphique. |
| [getWidthPixel()](#getWidthPixel--) | Obtient la largeur du cadre en unités de Pixel. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Obtient la largeur du cadre en unités du rapport de la zone du graphique. |
| [getX()](#getX--) | Obtient la coordonnée x du coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| [getXPixel()](#getXPixel--) | Obtient la coordonnée x du coin supérieur gauche en unités de Pixel. |
| [getXRatioToChart()](#getXRatioToChart--) | Obtient la coordonnée x du coin supérieur gauche en unités de proportion de la zone du graphique. |
| [getY()](#getY--) | Obtient la coordonnée y du coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| [getYPixel()](#getYPixel--) | Obtient la coordonnée y du coin supérieur gauche en unités de pixels. |
| [getYRatioToChart()](#getYRatioToChart--) | Obtient la coordonnée y du coin supérieur gauche en unités de proportion de la zone du graphique. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Indique que le texte est généré automatiquement. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Indique si le texte du graphique est automatiquement pivoté. |
| [isAutomaticSize()](#isAutomaticSize--) | Indique si le cadre du graphique a une taille automatique. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indique si la position par défaut (DefaultX, DefaultY, DefaultWidth et DefaultHeight) est définie. |
| [isDeleted()](#isDeleted--) | Indique si cette étiquette de données est supprimée. |
| [isInnerMode()](#isInnerMode--) | Indique si la taille de la zone de tracé inclut les marques de graduation et les libellés des axes. |
| [isNeverOverlap()](#isNeverOverlap--) | Indique si les étiquettes de données ne se chevauchent jamais lors de la conversion d'un graphique circulaire en image. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Obtient si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. |
| [isTextWrapped()](#isTextWrapped--) | Obtient une valeur indiquant si le texte est renvoyé à la ligne. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Indique que le texte est généré automatiquement. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indique si le cadre du graphique a une taille automatique. |
| [setBackground(int value)](#setBackground-int-) | Définit le mode d'affichage de l'arrière-plan. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Définit le mode d'affichage de l'arrière-plan |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indique si cette étiquette de données est supprimée. |
| [setDirectionType(int value)](#setDirectionType-int-) | Définit la direction du texte. |
| [setHeight(int value)](#setHeight-int-) | Définit la hauteur du cadre en unités de 1/4000 de la zone du graphique. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Définit la hauteur du cadre en unités de pixels. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Définit la hauteur du cadre en unités du ratio de la zone du graphique. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indique si la taille de la zone de tracé inclut les marques de graduation et les libellés des axes. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Définit une référence à la feuille de calcul. |
| [setNeverOverlap(boolean value)](#setNeverOverlap-boolean-) | Indique si les étiquettes de données ne se chevauchent jamais lors de la conversion d'un graphique circulaire en image. |
| [setNumber(int value)](#setNumber-int-) | Définit le format numérique intégré. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Représente la chaîne de format pour l'objet DataLabels. |
| [setNumberFormatLinked(boolean value)](#setNumberFormatLinked-boolean-) | Vrai si le format numérique est lié aux cellules (de sorte que le format numérique change dans les étiquettes lorsqu'il change dans les cellules). |
| [setPosition(int value)](#setPosition-int-) | Représente la position de l'étiquette de données. |
| [setPositionAuto()](#setPositionAuto--) | Définir la position du cadre sur automatique |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Représente l'ordre de lecture du texte. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Définit si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Représente l'angle de rotation du texte. |
| [setSeparatorType(int value)](#setSeparatorType-int-) | Définit le type de séparateur utilisé pour les étiquettes de données sur un graphique. |
| [setSeparatorValue(String value)](#setSeparatorValue-java.lang.String-) | Définit la valeur du séparateur utilisée pour les étiquettes de données sur un graphique. |
| [setShadow(boolean value)](#setShadow-boolean-) | Vrai si le cadre possède une ombre. |
| [setShapeType(int value)](#setShapeType-int-) | Définit le type de forme de l'étiquette de données. |
| [setShowBubbleSize(boolean value)](#setShowBubbleSize-boolean-) | Représente le comportement d'affichage de la valeur de pourcentage de l'étiquette de données d'un graphique spécifié. |
| [setShowCategoryName(boolean value)](#setShowCategoryName-boolean-) | Représente le comportement d'affichage du nom de catégorie de l'étiquette de données d'un graphique spécifié. Vrai pour afficher le nom de catégorie pour les étiquettes de données sur un graphique. |
| [setShowCellRange(boolean value)](#setShowCellRange-boolean-) | Indique s'il faut afficher la plage de cellules comme les étiquettes de données. |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | Représente le comportement d'affichage de la clé de légende de l'étiquette de données d'un graphique spécifié. |
| [setShowPercentage(boolean value)](#setShowPercentage-boolean-) | Représente le comportement d'affichage de la valeur de pourcentage de l'étiquette de données d'un graphique spécifié. |
| [setShowSeriesName(boolean value)](#setShowSeriesName-boolean-) | Indique si le nom de la série s'affiche sur les étiquettes de données d'un graphique. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Représente le comportement d'affichage des valeurs de l'étiquette de données d'un graphique spécifié. |
| [setText(String value)](#setText-java.lang.String-) | Définit le texte de l'étiquette de données. |
| [setTextDirection(int value)](#setTextDirection-int-) | Représente l'ordre de lecture du texte. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Définit l'alignement horizontal du texte. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Définit l'alignement vertical du texte. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Définit une valeur indiquant si le texte est renvoyé à la ligne. |
| [setWidth(int value)](#setWidth-int-) | Définit la largeur du cadre en unités de 1/4000 de la zone du graphique. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Définit la largeur du cadre en unités de pixel. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Définit la largeur du cadre en unités du ratio de la zone du graphique. |
| [setX(int value)](#setX-int-) | Définit la coordonnée x du coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| [setXPixel(int value)](#setXPixel-int-) | Définit la coordonnée x du coin supérieur gauche en unités de pixel. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Définit la coordonnée x du coin supérieur gauche en unités de proportion de la zone du graphique. |
| [setY(int value)](#setY-int-) | Définit la coordonnée y du coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| [setYPixel(int value)](#setYPixel-int-) | Définit la coordonnée y du coin supérieur gauche en unités de pixels. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Définit la coordonnée y du coin supérieur gauche en unités de proportion de la zone du graphique. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyFont() {#applyFont--}
```
public void applyFont()
```


Appliquer la police des étiquettes de données à tous les nœuds enfants.

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Renvoie un objet Characters qui représente une plage de caractères dans le texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | int | L'index du début du caractère. |
| length | int | Le nombre de caractères. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArea() {#getArea--}
```
public Area getArea()
```


Obtient le [getArea()](../../com.aspose.cells/datalabels\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai.

**Returns:**
boolean
### getBackground() {#getBackground--}
```
public int getBackground()
```


Obtient le mode d'affichage de l'arrière-plan. Cette propriété n'est valable que dans Excel 2003 ou les versions antérieures.

Voir [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Area.FillFormat.FillType. Par exemple, si vous devez définir BackgroundMode sur Opaque, vous pouvez utiliser le code suivant : Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Cette propriété sera supprimée 12 mois plus tard à compter de JANVIER 2012. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Obtient le mode d'affichage de l'arrière-plan

Voir [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Obtient le [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getChart() {#getChart--}
```
public Chart getChart()
```


Obtient le graphique auquel cet objet appartient.

**Returns:**
[Chart](../../com.aspose.cells/chart)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultHeight() {#getDefaultHeight--}
```
public int getDefaultHeight()
```


Représente la hauteur de la position par défaut en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété ChartFrame.DefaultHeightRatioToChart. DefaultHeight = (int)(DefaultHeightRatioToChart \* 4000); Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}
```
public double getDefaultHeightRatioToChart()
```


Représente la hauteur de la position par défaut en unités de la fraction de la zone du graphique.

**Returns:**
double
### getDefaultWidth() {#getDefaultWidth--}
```
public int getDefaultWidth()
```


Représente la largeur de la position par défaut en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété ChartFrame.DefaultWidthRatioToChart. DefaultWidth = (int)(DefaultWidthRatioToChart \* 4000); Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}
```
public double getDefaultWidthRatioToChart()
```


Représente la largeur de la position par défaut en unités de fraction de la zone du graphique.

**Returns:**
double
### getDefaultX() {#getDefaultX--}
```
public int getDefaultX()
```


Représente x de la position par défaut en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété ChartFrame.DefaultXRatioToChart. DefaultX = (int)(DefaultXRatioToChart \* 4000); Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}
```
public double getDefaultXRatioToChart()
```


Représente x de la position par défaut en unités de fraction de la zone du graphique.

**Returns:**
double
### getDefaultY() {#getDefaultY--}
```
public int getDefaultY()
```


Représente y de la position par défaut en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété ChartFrame.DefaultYRatioToChart. DefaultY = (int)(DefaultYRatioToChart \* 4000); Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}
```
public double getDefaultYRatioToChart()
```


Représente y de la position par défaut en unités de la fraction de la zone du graphique.

**Returns:**
double
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Obtient la direction du texte.

Voir [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Obtient la police des DataLabels ;

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Obtient la hauteur du cadre en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété ChartFrame.HeightRatioToChart. Height = HeightRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Obtient la hauteur du cadre en unités de pixels.

**Returns:**
int
### getHeightRatioToChart() {#getHeightRatioToChart--}
```
public double getHeightRatioToChart()
```


Obtient la hauteur du cadre en unités du rapport de la zone du graphique.

**Remarks**

Ceci est une valeur fractionnaire, sa plage valide est comprise entre 0 et 1. Comment convertir les unités de ratio en pixels ? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


Obtient une référence à la feuille de calcul.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


Obtient le format numérique intégré.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Représente la chaîne de format pour l'objet DataLabels.

**Returns:**
java.lang.String
### getNumberFormatLinked() {#getNumberFormatLinked--}
```
public boolean getNumberFormatLinked()
```


Vrai si le format numérique est lié aux cellules (de sorte que le format numérique change dans les étiquettes lorsqu'il change dans les cellules).

**Returns:**
boolean
### getPosition() {#getPosition--}
```
public int getPosition()
```


Représente la position de l'étiquette de données.

Voir [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


Représente l'ordre de lecture du texte.

Voir [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Représente l'angle de rotation du texte.

**Remarks**


0: Non pivoté.

255: De haut en bas.

\-90: Vers le bas.

90: Vers le haut.


**Returns:**
int
### getSeparatorType() {#getSeparatorType--}
```
public int getSeparatorType()
```


Obtient le type de séparateur utilisé pour les étiquettes de données sur un graphique.

Voir [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

Pour définir un séparateur personnalisé, veuillez définir la propriété [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) comme [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) puis spécifier la valeur attendue pour [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--).

**Returns:**
int
### getSeparatorValue() {#getSeparatorValue--}
```
public String getSeparatorValue()
```


Obtient la valeur du séparateur utilisée pour les étiquettes de données sur un graphique.

**Returns:**
java.lang.String
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Vrai si le cadre possède une ombre.

**Remarks**

Uniquement pour les graphiques dans les fichiers xls.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Obtient l'objet [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--).

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeType() {#getShapeType--}
```
public int getShapeType()
```


Obtient le type de forme de l'étiquette de données.

Voir [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Returns:**
int
### getShowBubbleSize() {#getShowBubbleSize--}
```
public boolean getShowBubbleSize()
```


Représente le comportement d'affichage de la valeur de pourcentage du libellé de données d'un graphique spécifié. True affiche la valeur du pourcentage. False masque la valeur du pourcentage.

**Returns:**
boolean
### getShowCategoryName() {#getShowCategoryName--}
```
public boolean getShowCategoryName()
```


Représente le comportement d'affichage du nom de catégorie du libellé de données d'un graphique spécifié. True pour afficher le nom de catégorie des libellés de données sur un graphique. False pour masquer.

**Returns:**
boolean
### getShowCellRange() {#getShowCellRange--}
```
public boolean getShowCellRange()
```


Indique s'il faut afficher la plage de cellules comme les étiquettes de données.

**Returns:**
boolean
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


Représente le comportement d'affichage de la clé de légende du libellé de données d'un graphique spécifié. True si la clé de légende du libellé de données est visible.

**Returns:**
boolean
### getShowPercentage() {#getShowPercentage--}
```
public boolean getShowPercentage()
```


Représente le comportement d'affichage de la valeur de pourcentage du libellé de données d'un graphique spécifié. True affiche la valeur du pourcentage. False masque la valeur du pourcentage.

**Returns:**
boolean
### getShowSeriesName() {#getShowSeriesName--}
```
public boolean getShowSeriesName()
```


Indique si le nom de la série s'affiche sur les libellés de données d'un graphique. True pour afficher le nom de la série. False pour masquer.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Représente le comportement d'affichage des valeurs du libellé de données d'un graphique spécifié. True affiche les valeurs. False pour masquer.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Obtient le texte de l'étiquette de données.

**Remarks**

Fonctionne uniquement lorsque c'est un libellé de données d'un point de graphique.

**Returns:**
java.lang.String
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Représente l'ordre de lecture du texte.

Voir [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartTextFrame.ReadingOrder. Cette propriété sera supprimée 12 mois plus tard à compter de mars 2020. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
int
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Obtient un objet [getFont()](../../com.aspose.cells/chartframe\#getFont--) du cadre de graphique spécifié.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Font. Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2012. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Obtient l'alignement horizontal du texte.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Obtient les options du texte.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


Obtient l'alignement vertical du texte.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Obtient la largeur du cadre en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété ChartFrame.WidthRatioToChart, à la place. Width = WidthRatioToChart \\* 4000; Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Obtient la largeur du cadre en unités de Pixel.

**Returns:**
int
### getWidthRatioToChart() {#getWidthRatioToChart--}
```
public double getWidthRatioToChart()
```


Obtient la largeur du cadre en unités du rapport de la zone du graphique.

**Remarks**

Il s'agit d'une valeur fractionnaire, sa plage valide est entre 0 et 1. Comment convertir les unités de ratio en pixels ? WidthPixel = WidthRatioToChart \\* Chart.ChartObject.Width;

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Obtient la coordonnée x du coin supérieur gauche en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété ChartFrame.XRatioToChart, à la place. X = XRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Obtient la coordonnée x du coin supérieur gauche en unités de Pixel.

**Returns:**
int
### getXRatioToChart() {#getXRatioToChart--}
```
public double getXRatioToChart()
```


Obtient la coordonnée x du coin supérieur gauche en unités de proportion de la zone du graphique.

**Remarks**

Il s'agit d'une valeur fractionnaire, sa plage valide est comprise entre 0 et 1. Comment convertir les unités de ratio en pixels ? XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Obtient la coordonnée y du coin supérieur gauche en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété ChartFrame.YRatioToChart, à la place. Y = YRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Obtient la coordonnée y du coin supérieur gauche en unités de pixels.

**Returns:**
int
### getYRatioToChart() {#getYRatioToChart--}
```
public double getYRatioToChart()
```


Obtient la coordonnée y du coin supérieur gauche en unités de proportion de la zone du graphique.

**Remarks**

Il s'agit d'une valeur fractionnaire, sa plage valide est comprise entre 0 et 1. Comment convertir les unités de ratio en pixels ? YPixel = YRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoText() {#isAutoText--}
```
public boolean isAutoText()
```


Indique que le texte est généré automatiquement.

**Returns:**
boolean
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


Indique si le texte du graphique est automatiquement pivoté.

**Returns:**
boolean
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


Indique si le cadre du graphique a une taille automatique.

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


Indique si la position par défaut (DefaultX, DefaultY, DefaultWidth et DefaultHeight) est définie.

**Returns:**
boolean
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Indique si cette étiquette de données est supprimée.

**Returns:**
boolean
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


Indique si la taille de la zone de tracé inclut les marques de graduation et les étiquettes d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les marques de graduation et les étiquettes d'axe.

**Remarks**

Uniquement pour les fichiers Xlsx.

**Returns:**
boolean
### isNeverOverlap() {#isNeverOverlap--}
```
public boolean isNeverOverlap()
```


Indique si les libellés de données ne se chevauchent jamais lors de la conversion d'un graphique circulaire en image. Remarque : cette propriété n'est pertinente que lors d'un graphique circulaire en image.

**Returns:**
boolean
### isResizeShapeToFitText() {#isResizeShapeToFitText--}
```
public boolean isResizeShapeToFitText()
```


Obtient si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. L'ajustement automatique consiste à mettre à l'échelle le texte à l'intérieur d'une forme afin de contenir tout le texte.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Obtient une valeur indiquant si le texte est renvoyé à la ligne.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutoText(boolean value) {#setAutoText-boolean-}
```
public void setAutoText(boolean value)
```


Indique que le texte est généré automatiquement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


Indique si le cadre du graphique a une taille automatique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBackground(int value) {#setBackground-int-}
```
public void setBackground(int value)
```


Définit le mode d'affichage de l'arrière-plan. Cette propriété n'est valable que dans Excel 2003 ou les versions antérieures.

Voir [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Area.FillFormat.FillType. Par exemple, si vous devez définir BackgroundMode sur Opaque, vous pouvez utiliser le code suivant : Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Cette propriété sera supprimée 12 mois plus tard à compter de JANVIER 2012. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Définit le mode d'affichage de l'arrière-plan

Voir [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Indique si cette étiquette de données est supprimée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


Définit la direction du texte.

Voir [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Définit la hauteur du cadre en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété ChartFrame.HeightRatioToChart. Height = HeightRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Définit la hauteur du cadre en unités de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHeightRatioToChart(double value) {#setHeightRatioToChart-double-}
```
public void setHeightRatioToChart(double value)
```


Définit la hauteur du cadre en unités du ratio de la zone du graphique.

**Remarks**

Ceci est une valeur fractionnaire, sa plage valide est comprise entre 0 et 1. Comment convertir les unités de ratio en pixels ? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setInnerMode(boolean value) {#setInnerMode-boolean-}
```
public void setInnerMode(boolean value)
```


Indique si la taille de la zone de tracé inclut les marques de graduation et les étiquettes d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les marques de graduation et les étiquettes d'axe.

**Remarks**

Uniquement pour les fichiers Xlsx.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLinkedSource(String value) {#setLinkedSource-java.lang.String-}
```
public void setLinkedSource(String value)
```


Définit une référence à la feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setNeverOverlap(boolean value) {#setNeverOverlap-boolean-}
```
public void setNeverOverlap(boolean value)
```


Indique si les libellés de données ne se chevauchent jamais lors de la conversion d'un graphique circulaire en image. Remarque : cette propriété n'est pertinente que lors d'un graphique circulaire en image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Définit le format numérique intégré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Représente la chaîne de format pour l'objet DataLabels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setNumberFormatLinked(boolean value) {#setNumberFormatLinked-boolean-}
```
public void setNumberFormatLinked(boolean value)
```


Vrai si le format numérique est lié aux cellules (de sorte que le format numérique change dans les étiquettes lorsqu'il change dans les cellules).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Représente la position de l'étiquette de données.

Voir [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Définir la position du cadre sur automatique

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


Représente l'ordre de lecture du texte.

Voir [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setResizeShapeToFitText(boolean value) {#setResizeShapeToFitText-boolean-}
```
public void setResizeShapeToFitText(boolean value)
```


Définit si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. L'ajustement automatique consiste à mettre à l'échelle le texte à l'intérieur d'une forme afin de contenir tout le texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Représente l'angle de rotation du texte.

**Remarks**


0: Non pivoté.

255: De haut en bas.

\-90: Vers le bas.

90: Vers le haut.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSeparatorType(int value) {#setSeparatorType-int-}
```
public void setSeparatorType(int value)
```


Définit le type de séparateur utilisé pour les étiquettes de données sur un graphique.

Voir [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

Pour définir un séparateur personnalisé, veuillez définir la propriété [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) comme [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) puis spécifier la valeur attendue pour [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSeparatorValue(String value) {#setSeparatorValue-java.lang.String-}
```
public void setSeparatorValue(String value)
```


Définit la valeur du séparateur utilisée pour les étiquettes de données sur un graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Vrai si le cadre possède une ombre.

**Remarks**

Uniquement pour les graphiques dans les fichiers xls.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShapeType(int value) {#setShapeType-int-}
```
public void setShapeType(int value)
```


Définit le type de forme de l'étiquette de données.

Voir [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setShowBubbleSize(boolean value) {#setShowBubbleSize-boolean-}
```
public void setShowBubbleSize(boolean value)
```


Représente le comportement d'affichage de la valeur de pourcentage du libellé de données d'un graphique spécifié. True affiche la valeur du pourcentage. False masque la valeur du pourcentage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowCategoryName(boolean value) {#setShowCategoryName-boolean-}
```
public void setShowCategoryName(boolean value)
```


Représente le comportement d'affichage du nom de catégorie du libellé de données d'un graphique spécifié. True pour afficher le nom de catégorie des libellés de données sur un graphique. False pour masquer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowCellRange(boolean value) {#setShowCellRange-boolean-}
```
public void setShowCellRange(boolean value)
```


Indique s'il faut afficher la plage de cellules comme les étiquettes de données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


Représente le comportement d'affichage de la clé de légende du libellé de données d'un graphique spécifié. True si la clé de légende du libellé de données est visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowPercentage(boolean value) {#setShowPercentage-boolean-}
```
public void setShowPercentage(boolean value)
```


Représente le comportement d'affichage de la valeur de pourcentage du libellé de données d'un graphique spécifié. True affiche la valeur du pourcentage. False masque la valeur du pourcentage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowSeriesName(boolean value) {#setShowSeriesName-boolean-}
```
public void setShowSeriesName(boolean value)
```


Indique si le nom de la série s'affiche sur les libellés de données d'un graphique. True pour afficher le nom de la série. False pour masquer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Représente le comportement d'affichage des valeurs du libellé de données d'un graphique spécifié. True affiche les valeurs. False pour masquer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Définit le texte de l'étiquette de données.

**Remarks**

Fonctionne uniquement lorsque c'est un libellé de données d'un point de graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Représente l'ordre de lecture du texte.

Voir [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartTextFrame.ReadingOrder. Cette propriété sera supprimée 12 mois plus tard à compter de mars 2020. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Définit l'alignement horizontal du texte.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Définit l'alignement vertical du texte.

Voir [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Définit une valeur indiquant si le texte est renvoyé à la ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Définit la largeur du cadre en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété ChartFrame.WidthRatioToChart, à la place. Width = WidthRatioToChart \\* 4000; Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Définit la largeur du cadre en unités de pixel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWidthRatioToChart(double value) {#setWidthRatioToChart-double-}
```
public void setWidthRatioToChart(double value)
```


Définit la largeur du cadre en unités du ratio de la zone du graphique.

**Remarks**

Il s'agit d'une valeur fractionnaire, sa plage valide est entre 0 et 1. Comment convertir les unités de ratio en pixels ? WidthPixel = WidthRatioToChart \\* Chart.ChartObject.Width;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Définit la coordonnée x du coin supérieur gauche en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété ChartFrame.XRatioToChart, à la place. X = XRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Définit la coordonnée x du coin supérieur gauche en unités de pixel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setXRatioToChart(double value) {#setXRatioToChart-double-}
```
public void setXRatioToChart(double value)
```


Définit la coordonnée x du coin supérieur gauche en unités de proportion de la zone du graphique.

**Remarks**

Il s'agit d'une valeur fractionnaire, sa plage valide est comprise entre 0 et 1. Comment convertir les unités de ratio en pixels ? XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Définit la coordonnée y du coin supérieur gauche en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété ChartFrame.YRatioToChart, à la place. Y = YRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Définit la coordonnée y du coin supérieur gauche en unités de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setYRatioToChart(double value) {#setYRatioToChart-double-}
```
public void setYRatioToChart(double value)
```


Définit la coordonnée y du coin supérieur gauche en unités de proportion de la zone du graphique.

**Remarks**

Il s'agit d'une valeur fractionnaire, sa plage valide est comprise entre 0 et 1. Comment convertir les unités de ratio en pixels ? YPixel = YRatioToChart \* Chart.ChartObject.Height;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

