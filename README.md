# Units

| Unit   | Description                                                                                  |
|--------|----------------------------------------------------------------------------------------------|
| `ch`   | The width of the character "0" in the current font, used for widths or spacing relative to the character size. |
| `rem`  | Relative to the root element's (`<html>`) font size, often used for scalable and consistent spacing and typography. |
| `fr`   | A fraction of the available space in CSS Grid layouts, useful for dividing space proportionally between grid items. |
| `em`   | Relative to the font size of the parent element, used for scalable sizing of text or other elements. |
| `px`   | An absolute unit representing pixels, used for fixed-size elements that do not scale with the layout. |
| `%`    | Relative to the size of the parent element, commonly used for setting widths, heights, margins, or padding. |
| `vw`   | Viewport width. 1 `vw` equals 1% of the width of the viewport (browser window). |
| `vh`   | Viewport height. 1 `vh` equals 1% of the height of the viewport. |
| `vmin` | The smaller value between `vw` and `vh`, useful for responsive design. |
| `vmax` | The larger value between `vw` and `vh`, used when you want an element to scale based on the larger dimension. |
| `cm`   | Centimeters, an absolute length unit, typically used for print media. |
| `mm`   | Millimeters, another absolute length unit, typically used for print media. |
| `in`   | Inches, an absolute unit, primarily used in print design (1 inch = 2.54 cm). |
| `pt`   | Points, an absolute unit where 1 point equals 1/72 of an inch, often used in print media. |
| `pc`   | Picas, another print-based unit where 1 pica equals 12 points or 1/6 of an inch. |

# CSS Unit Comparison

This section demonstrates various CSS units (`ch`, `rem`, `fr`, `em`, `px`, etc.) and how they behave in a browser.

## Unit Comparison Table

Here are some boxes with different CSS units applied for comparison:

<table>
  <thead>
    <tr>
      <th>Unit</th>
      <th>Box Example</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1rem</td>
      <td>
        <div style="width: 5rem; height: 2rem; background-color: lightblue; display: inline-block;">5rem width</div>
      </td>
      <td>Box with a width of 5 times the root element's font size.</td>
    </tr>
    <tr>
      <td>1em</td>
      <td>
        <div style="width: 5em; height: 2em; background-color: lightgreen; display: inline-block;">5em width</div>
      </td>
      <td>Box with a width relative to the parent element's font size.</td>
    </tr>
    <tr>
      <td>50px</td>
      <td>
        <div style="width: 50px; height: 50px; background-color: lightcoral; display: inline-block;">50px width</div>
      </td>
      <td>Fixed-size box of 50 pixels width.</td>
    </tr>
    <tr>
      <td>10ch</td>
      <td>
        <div style="width: 10ch; height: 2ch; background-color: lightyellow; display: inline-block;">10ch width</div>
      </td>
      <td>Box with a width equivalent to the width of 10 "0" characters in the current font.</td>
    </tr>
    <tr>
      <td>20vw</td>
      <td>
        <div style="width: 20vw; height: 10vh; background-color: lightgray; display: inline-block;">20vw width</div>
      </td>
      <td>Box with a width of 20% of the viewport's width.</td>
    </tr>
  </tbody>
</table>

## Grid with `fr` Example

To demonstrate the `fr` unit, here's a simple grid layout:

<div style="display: grid; grid-template-columns: 1fr 2fr 1fr; gap: 10px;">
  <div style="background-color: lightcoral; padding: 10px;">1fr</div>
  <div style="background-color: lightblue; padding: 10px;">2fr</div>
  <div style="background-color: lightgreen; padding: 10px;">1fr</div>
</div>

In the example above, the grid columns are distributed as 1 fraction for the first and third columns, and 2 fractions for the middle column.
