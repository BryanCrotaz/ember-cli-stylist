# [ember-cli-stylist](https://github.com/lifegadget/ember-cli-stylist) ![ ](https://travis-ci.org/lifegadget/ember-cli-stylist.svg) [![npm version](https://badge.fury.io/js/ember-cli-stylist.svg)](http://badge.fury.io/js/ember-cli-stylist) [![Code Climate](https://codeclimate.com/github/lifegadget/ember-cli-stylist/badges/gpa.svg)
> Input controls for ambitious Ember applications.

## Install ##
- Modern CLI versions
    ````bash
    ember install ui-knob
    ````

## Usage ##
This addon those seaking to have their component  proxy through HTML **style** attributes (such as `height`, `width`, `color`, `fontSize`, etc.) but do not want force a containing object to be required to open up their content-security-policy to include the **'unsafe-inline'** property.

To use this just install and then in your component mixin the `shared-stylist` mixin like so:

    import SharedStylist as 'ember-cli-stylist/mixins/shared-stylist';
    export default Ember.Component.extend(SharedStylist,{
      // your code here
    }

You can optionally include a property in your component `_styleWhitelist` which will limit the styles that are proxied only to those you specify. 

## Dependencies

None.

## Version Compatibility

This may very well work with older version of Ember and Ember-CLI but it was intended for:

- Ember 1.13.7+
- Ember-CLI 1.13.7+

You can see the CI results at: [Travis Reporting](https://travis-ci.org/lifegadget/ember-cli-stylist)

## Repo Contribution

We're open to your creative suggestions but please move past the "idea" stage
and send us a PR so we can incorporate your ideas without killing ourselves. :)

## Licensing

This component is free to use under the MIT license:

Copyright (c) 2015 LifeGadget Ltd

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do
so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
