# \<klima-dashboard\>

The klima-dashboard element helps to build Dashboards by doing the positioning
for tiles. The dashboard can be responsive to adjust the size of the dashboard
and tiles. With the border-width attribute it's possible to adjust the border
between tiles. By adding a element with a header class a title can be added to
the dashboard. The content of a tile must be placed in a klima-dashboard-tile
elment. Every tile needs to declare a row. Tiles can overlap over rows. But for
every row the position must be declared. Optional a tile can have a width, the
value is percental to the dashboard width. If the dashboard is in reponsive mode
tiles should have a min width in pixels. If the dashboard has not enough place
to grant the min width of a tile, the tile will be faded out. The following is
a simple demo:

```
<klima-dashboard border-width="4" class="dashboards" responsive>
  <div class="header">Dashboard</div>
  <klima-dashboard-tile style="background-color: red;" row="1" overlap="1" positions="[1,1]" min-width="500">A</klima-dashboard-tile>
  <klima-dashboard-tile style="background-color: blue;" row="1" positions="[2]" min-width="250">B</klima-dashboard-tile>
  <klima-dashboard-tile style="background-color: green;" row="1" positions="[3]" min-width="250">C</klima-dashboard-tile>
  <klima-dashboard-tile style="background-color: yellow;" row="2" positions="[2]" min-width="500">D</klima-dashboard-tile>
  <klima-dashboard-tile style="background-color: orange;" row="3" positions="[1]" min-width="250">E</klima-dashboard-tile>
  <klima-dashboard-tile style="background-color: aqua;" row="3" positions="[2]" min-width="250">F</klima-dashboard-tile>
  <klima-dashboard-tile style="background-color: hotpink;" row="3" positions="[3]" min-width="250">G</klima-dashboard-tile>
</klima-dashboard>
```
For more demos and documentation serve the element and check the demos


## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your element locally.

## Viewing Your Element

```
$ polymer serve
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
