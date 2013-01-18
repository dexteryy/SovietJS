<!---
layout: intro
title: SovietJS 
-->

# SovietJS 

> * Standalone UI event delegate implementation
> * Provide multiple styles/modes: override, automatically preventDefault, partial matching, exact matching...

## AMD and OzJS

* SovietJS can either be viewed as an independent library, or as a part of [OzJS mirco-framework](http://ozjs.org/#framework).
* It's wrapped as an [AMD (Asynchronous Module Definition)](https://github.com/amdjs/amdjs-api/wiki/AMD) module. You should use it with [oz.js](http://ozjs.org/#start) (or require.js or [similar](http://wiki.commonjs.org/wiki/Implementations) for handling dependencies). 
* If you want to make it available for both other AMD code and traditional code based on global namespace. OzJS provides [a mini define/require implementation](http://ozjs.org/examples/adapter/) to transform AMD module into traditional [module pattern](http://www.adequatelygood.com/2010/3/JavaScript-Module-Pattern-In-Depth).
* See [http://ozjs.org](http://ozjs.org) for details.

## Dependencies

* [mo/lang/es5](https://github.com/dexteryy/mo/es5)
* [mo/lang/mix](https://github.com/dexteryy/mo/mix)
* [mo/lang/type](https://github.com/dexteryy/mo/type)
* [mo/lang/struct](https://github.com/dexteryy/mo/struct)
* [dollar](https://github.com/dexteryy/DollarJS) or other jQuery-compatible library

## Examples

Under construction...

## Get the code

* [View/download on Github](https://github.com/dexteryy/SovietJS/blob/master/soviet.js)
* Add/update to your project as new dependency:
    * via [istatic](https://github.com/mockee/istatic.git)
    * via [volo](https://github.com/volojs/volo)

## API and usage

```javascript 
var soviet = require('soviet');
```

* `soviet(elm/*, options */)` -- 
    * options:
        * `preventDefault` -- false
        * `matchesSelector` -- false
        * `autoOverride` -- false
        * `trace` -- false
        * `traceStack` -- null
    * API:
        * `on(event/*, selector */, handler)` -- 
        * `on(event, { 'selector': handler, ... })` -- 
        * `off(event, selector, handler)` -- 
        * `matches(event, selector)` -- 
        * `reset(event)` -- 
        * `disable(event, selector)` -- 
        * `enable(event, selector)` -- 
        * `trigger(ev)` -- 
* `soviet.Soviet` -- 

Under construction...

## More References

See [OzJS References](http://ozjs.org/#ref)

## Release History

See [OzJS Release History](http://ozjs.org/#release)

## License

Copyright (c) 2010 - 2013 dexteryy  
Licensed under the MIT license.


