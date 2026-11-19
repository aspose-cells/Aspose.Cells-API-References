---
title: "Légende"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente la légende du graphique."
type: docs
url: /fr/java/com.aspose.cells/legend/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class Legend extends ChartTextFrame
```

Encapsule l'objet qui représente la légende du graphique.

**Example**

```
         Workbook workbook = new Workbook();
         	Worksheet sheet = workbook.getWorksheets().get(0);
 
         	Cells cells = sheet.getCells();
         	cells.get(0,1).putValue("Income");
         	cells.get(1,0).putValue("Company A");
         	cells.get(2,0).putValue("Company B");
         	cells.get(3,0).putValue("Company C");
         	cells.get(1,1).putValue(10000);
         	cells.get(2,1).putValue(20000);
         	cells.get(3,1).putValue(30000);
 
         	int chartIndex = sheet.getCharts().add(ChartType.COLUMN, 9, 9, 21, 15);
         	Chart chart = sheet.getCharts().get(chartIndex);
         	chart.setChartDataRange("A1:B4", true);
         //Set Legend's width and height
         Legend legend = chart.getLegend();
 
         //Legend is at right side of chart by default.
         //If the legend is at left or right side of the chart, setting Legend.X property will not take effect.
         //If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.
         legend.setY(1500);
         legend.setWidth(50);
         legend.setHeight(50); 
         //Set legend's position
         legend.setPosition(LegendPositionType.LEFT);
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [characters(int startIndex, int length)](#characters-int-int-) | Renvoie un objet Characters qui représente une plage de caractères dans le texte. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Obtient le [getArea()](../../com.aspose.cells/chartframe\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. |
| [getBackground()](#getBackground--) | Obtient le mode d'affichage de l'arrière‑plan. |
| [getBackgroundMode()](#getBackgroundMode--) | Obtient le mode d'affichage de l'arrière‑plan. |
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
| [getFont()](#getFont--) | Obtient un objet [getFont()](../../com.aspose.cells/chartframe\#getFont--) du cadre de graphique spécifié. |
| [getHeight()](#getHeight--) | Obtient la hauteur du cadre en unités de 1/4000 de la zone du graphique. |
| [getHeightPixel()](#getHeightPixel--) | Obtient la hauteur du cadre en unités de pixels. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Obtient la hauteur du cadre en unités du rapport de la zone du graphique. |
| [getLegendEntries()](#getLegendEntries--) | Obtient une collection de tous les objets LegendEntry dans la légende de graphique spécifiée. |
| [getLegendEntriesLabels()](#getLegendEntriesLabels--) | Obtient les libellés des entrées de légende après l'appel de la méthode Chart.Calculate(). |
| [getLegendLabels()](#getLegendLabels--) | Obtient les libellés des entrées de légende après l'appel de la méthode Chart.Calculate(). |
| [getLinkedSource()](#getLinkedSource--) | Obtient une référence à la feuille de calcul. |
| [getPosition()](#getPosition--) | Obtient le type de position de la légende. |
| [getReadingOrder()](#getReadingOrder--) | Représente l'ordre de lecture du texte. |
| [getRotationAngle()](#getRotationAngle--) | Représente l'angle de rotation du texte. |
| [getShadow()](#getShadow--) | Vrai si le cadre possède une ombre. |
| [getShapeProperties()](#getShapeProperties--) | Obtient l'objet [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getText()](#getText--) | Obtient le texte du titre d'un cadre. |
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
| [isOverLay()](#isOverLay--) | Obtient si la légende est affichée sans chevaucher le graphique. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Obtient si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. |
| [isTextWrapped()](#isTextWrapped--) | Obtient une valeur indiquant si le texte est renvoyé à la ligne. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Indique que le texte est généré automatiquement. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indique si le cadre du graphique a une taille automatique. |
| [setBackground(int value)](#setBackground-int-) | Définit le mode d'affichage de l'arrière-plan. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Définit le mode d'affichage de l'arrière-plan. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indique si cette étiquette de données est supprimée. |
| [setDirectionType(int value)](#setDirectionType-int-) | Définit la direction du texte. |
| [setHeight(int value)](#setHeight-int-) | Définit la hauteur du cadre en unités de 1/4000 de la zone du graphique. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Définit la hauteur du cadre en unités de pixels. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Définit la hauteur du cadre en unités du ratio de la zone du graphique. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indique si la taille de la zone de tracé inclut les marques de graduation et les libellés des axes. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Définit une référence à la feuille de calcul. |
| [setOverLay(boolean value)](#setOverLay-boolean-) | Définit si la légende doit être affichée sans chevaucher le graphique. |
| [setPosition(int value)](#setPosition-int-) | Définit le type de position de la légende. |
| [setPositionAuto()](#setPositionAuto--) | Définir la position du cadre sur automatique |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Représente l'ordre de lecture du texte. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Définit si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Représente l'angle de rotation du texte. |
| [setShadow(boolean value)](#setShadow-boolean-) | Vrai si le cadre possède une ombre. |
| [setText(String value)](#setText-java.lang.String-) | Définit le texte du titre d'un cadre. |
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


Obtient le [getArea()](../../com.aspose.cells/chartframe\#getArea--).

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


Obtient le mode d'affichage de l'arrière-plan. Cette propriété n'est valable que dans Excel 2003 ou les versions antérieures.

Voir [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Area.FillFormat.FillType. Par exemple, si vous devez définir BackgroundMode sur Opaque, vous pouvez utiliser le code suivant : Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Cette propriété sera supprimée 12 mois plus tard à compter de février 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

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


Obtient un objet [getFont()](../../com.aspose.cells/chartframe\#getFont--) du cadre de graphique spécifié.

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
### getLegendEntries() {#getLegendEntries--}
```
public LegendEntryCollection getLegendEntries()
```


Obtient une collection de tous les objets LegendEntry dans la légende de graphique spécifiée. La définition des entrées de légende pour un graphique de surface n'est pas prise en charge. Ainsi, elle renverra null si le type de graphique est un graphique de surface.

**Returns:**
[LegendEntryCollection](../../com.aspose.cells/legendentrycollection)
### getLegendEntriesLabels() {#getLegendEntriesLabels--}
```
public ArrayList getLegendEntriesLabels()
```


Obtient les libellés des entrées de légende après l'appel de la méthode Chart.Calculate().

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la méthode Legend.GetLegendLabels. Cette propriété sera supprimée 12 mois plus tard, à compter de novembre 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.util.ArrayList
### getLegendLabels() {#getLegendLabels--}
```
public String[] getLegendLabels()
```


Obtient les libellés des entrées de légende après l'appel de la méthode Chart.Calculate().

**Returns:**
java.lang.String[]
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


Obtient une référence à la feuille de calcul.

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


Obtient le type de position de la légende.

Voir [LegendPositionType](../../com.aspose.cells/legendpositiontype).

**Remarks**


La position par défaut est à droite.

Si la légende se trouve à gauche ou à droite du graphique, la définition de la propriété Legend.X n'aura aucun effet.

Si la légende se trouve en haut ou en bas du graphique, la définition de la propriété Legend.Y n'aura aucun effet.


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
### getText() {#getText--}
```
public String getText()
```


Obtient le texte du titre d'un cadre.

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
### isOverLay() {#isOverLay--}
```
public boolean isOverLay()
```


Obtient si la légende est affichée sans chevaucher le graphique.

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


Définit le mode d'affichage de l'arrière-plan. Cette propriété n'est valable que dans Excel 2003 ou les versions antérieures.

Voir [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Area.FillFormat.FillType. Par exemple, si vous devez définir BackgroundMode sur Opaque, vous pouvez utiliser le code suivant : Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Cette propriété sera supprimée 12 mois plus tard à compter de février 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

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

### setOverLay(boolean value) {#setOverLay-boolean-}
```
public void setOverLay(boolean value)
```


Définit si la légende doit être affichée sans chevaucher le graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Définit le type de position de la légende.

Voir [LegendPositionType](../../com.aspose.cells/legendpositiontype).

**Remarks**


La position par défaut est à droite.

Si la légende se trouve à gauche ou à droite du graphique, la définition de la propriété Legend.X n'aura aucun effet.

Si la légende se trouve en haut ou en bas du graphique, la définition de la propriété Legend.Y n'aura aucun effet.


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

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Définit le texte du titre d'un cadre.

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

