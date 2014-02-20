*This repository is a mirror of the [component](http://component.io) module [gamtiq/return-function](http://github.com/gamtiq/return-function). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/gamtiq-return-function`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# return-function

Set of functions that simply return a value.
Can be used for stubs.


## Installation

### Node

    npm install return-function

### Component

Install component:

    npm install -g component

Then:

    component install gamtiq/return-function

## Usage

### Node, Component

    var ret = require("return-function");
    ...
    
### AMD

    define(["dist/return-function"], function(ret) {
        ...
    });

### Browser

    <script type="text/javascript" src="dist/return-function.js"></script>
    <script type="text/javascript">
        var ret = returnFunction;
        ...
    </script>

## Examples

    var global = ret.returnGlobal();   // window in browser
    var first = ret.returnFirstArg(1, 2, 3);   // 1
    var second = ret.returnSecondArg(1, 2, 3);   // 2
    var list = ret.returnArgList(1, 2, 3);   // [1, 2, 3]

## API

### .emptyFunction()

Empty function that does nothing and returns `undefined`.

### .returnUndefined()

Empty function that does nothing and returns `undefined`.

### .returnNull()

Return `null`.

### .returnTrue()

Return `true`.

### .returnFalse()

Return `false`.

### .returnEmptyStr()

Return empty string.

### .returnNaN()

Return `NaN`.

### .returnZero()

Return `0`.

### .returnOne()

Return `1`.

### .returnEmptyObject()

Return `{}`.

### .returnEmptyArray()

Return `[]`.

### .returnEmptyFunction()

Return `function () {}`.

### .returnDate()

Return `new Date()`.

### .returnThis()

Return `this`.

### .returnGlobal()

Return global object (`window` in browser).

### .returnFirstArg()

Return the first argument.

### .returnSecondArg()

Return the second argument.

### .returnArgList()

Return array of arguments.

