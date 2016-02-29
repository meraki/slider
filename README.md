# meraki-slider
---

meraki's fork of rc-slider, a react slider component 

[![NPM version][npm-image]][npm-url]
[![node version][node-image]][node-url]
[![npm download][download-image]][download-url]

[npm-image]: http://img.shields.io/npm/v/meraki-slider.svg?style=flat-square
[npm-url]: http://npmjs.org/package/meraki-slider
[node-image]: https://img.shields.io/badge/node.js-%3E=_0.10-green.svg?style=flat-square
[node-url]: http://nodejs.org/download/
[download-image]: https://img.shields.io/npm/dm/meraki-slider.svg?style=flat-square
[download-url]: https://npmjs.org/package/meraki-slider

## Feature

* support ie8,ie8+,chrome,firefox,safari

### Keyboard

## install

[![meraki-slider](https://nodei.co/npm/meraki-slider.png)](https://npmjs.org/package/meraki-slider)

## Usage

```js
var React = require('react');
var ReactDOM = require('react-dom');
var Merakislider = require('meraki-slider');
ReactDOM.render(<Merakislider />, container);
```

### props

<table class="table table-bordered table-striped">
    <thead>
    <tr>
        <th style="width: 100px;">name</th>
        <th style="width: 50px;">type</th>
        <th style="width: 50px;">default</th>
        <th>description</th>
    </tr>
    </thead>
    <tbody>
        <tr>
          <td>className</td>
          <td>String</td>
          <td>rc-slider</td>
          <td>Additional css class for the root dom node</td>
        </tr>
        <tr>
          <td>min</td>
          <td>number</td>
          <td>0</td>
          <td>The minimum value of the slider</td>
        </tr>
        <tr>
          <td>max</td>
          <td>number</td>
          <td>100</td>
          <td>The maximum value of the slider</td>
        </tr>
        <tr>
          <td>marks</td>
          <td>object {number: string}</td>
          <td>{}</td>
          <td>Mark on the slider. The key determines the position, and the value determines what will show.</td>
        </tr>
        <tr>
          <td>step</td>
          <td>number or `null`</td>
          <td>1</td>
          <td>Value to be added or subtracted on each step the slider makes. Must be greater than zero. max - min should be evenly divisible by the step value. When `marks` is not an empty object, `step` can be set to `null`, to make marks as steps.</td>
        </tr>
        <tr>
          <td>range</td>
          <td>boolean</td>
          <td>false</td>
          <td>Determines the type of slider. If range is `true`, two handles will be rendered in order to select a range.</td>
        </tr>
        <tr>
          <td>allowCross</td>
          <td>boolean</td>
          <td>true</td>
          <td>When `range` is `true`, `allowCross` could be set as `true` to allow those two handles cross.</td>
        </tr>
        <tr>
          <td>defaultValue</td>
          <td>number or [number, number]</td>
          <td>0 or [0, 0]</td>
          <td>Set initial positions of handles. If range is `false`, the type of `defaultValue` should be `number`. Otherwise, `[number, number]`</td>
        </tr>
        <tr>
          <td>value</td>
          <td>number or [number, number]</td>
          <td></td>
          <td>Set current positions of handles. If range is `false`, the type of `defaultValue` should be `number`. Otherwise, `[number, number]`</td>
        </tr>
        <tr>
          <td>included</td>
          <td>boolean</td>
          <td>true</td>
          <td>If the value is `true`, it means a continuous value interval, otherwise, it is a independent value.</td>
        </tr>
        <tr>
          <td>disabled</td>
          <td>boolean</td>
          <td>false</td>
          <td>If `true`, handles can't be moved.</td>
        </tr>
        <tr>
          <td>tipTransitionName</td>
          <td>string</td>
          <td>''</td>
          <td>Set the animation for tooltip if it shows.</td>
        </tr>
        <tr>
          <td>tipFormatter</td>
          <td>function or `null`</td>
          <td></td>
          <td>Format the value of the tooltip if it shows. If `null` the tooltip will always be hidden.</td>
        </tr>
        <tr>
          <td>dots</td>
          <td>bool</td>
          <td>false</td>
          <td>When the `step` value is greater than 1, you can set the `dots` to  `true` if you want to render the slider with dots.</td>
        </tr>
        <tr>
          <td>onChange</td>
          <td>function</td>
          <td>NOOP</td>
          <td>`onChange` will be triggered while the value of Slider changing.</td>
        </tr>
        <tr>
          <td>onAfterChange</td>
          <td>function</td>
          <td>NOOP</td>
          <td>`onAfterChange` will be triggered when `ontouchend` or `onmouseup` is triggered.</td>
        </tr>
        <tr>
          <td>reverseSlide</td>
          <td>function</td>
          <td>NOOP</td>
          <td>reverseSlide with tether a slider with a range on the right</td>
        </tr>
    </tbody>
</table>
## Development

```
npm install
npm start
```

## Example

http://localhost:8005/examples/

online example: http://react-component.github.io/slider/

## Test Case

http://localhost:8005/tests/runner.html?coverage

## Coverage

http://localhost:8005/node_modules/rc-server/node_modules/node-jscover/lib/front-end/jscoverage.html?w=http://localhost:8088/tests/runner.html?coverage

## License

meraki-slider is released under the MIT license.
