##BorderType
Enumerates the border line and diagonal line types.
## BorderType enumeration
Enumerates the border line and diagonal line types.
### Values
| Name | Value | Description |
| --- | --- | --- |
| LeftBorder | `1` | Represents left border line. |
| RightBorder | `2` | Represents right border line exists. |
| TopBorder | `4` | Represents top border line. |
| BottomBorder | `8` | Represents bottom border line. |
| DiagonalDown | `16` | Represents the diagonal line from top left to right bottom. |
| DiagonalUp | `32` | Represents the diagonal line from bottom left to right top. |
| Vertical | `64` | Only for dynamic style, such as conditional formatting. |
| Horizontal | `128` | Only for dynamic style, such as conditional formatting. |
| SideBorders | `15` | Indicates the four side borders: [LeftBorder](../leftborder/), [RightBorder](../rightborder/), [TopBorder](../topborder/) and [BottomBorder](../bottomborder/). |
| Diagonal | `48` | Special combination of multiple borders for user's convenience for some APIs. Indicates diagonal borders of [DiagonalUp](../diagonalup/) and [DiagonalDown](../diagonaldown/). |
| DynamicStyleBorders | `192` | Indicates [Vertical](../vertical/) and [Horizontal](../horizontal/) of dynamic style. |
| None | `0` | No border has been specified. |
