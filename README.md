```css
@utility utilityName {
    color: green;
}

@utility utilityName small {
    color: blue;
}

@component ComponentName {
    color: cyan;

    @modifier modifierName {
        color: yellow;
    }

    @descendent descendentName {
        color: navy;
    }

    @when stateName {
        color: crimson;
    }
}

@component-namespace nmsp {
    @component ComponentName {
        color: red;
    }
}
```
```
.u-blockName {
    color: blue
}

.u--blockName {
    color: green
}

.elementName {
    color: brown
}

.elementName.is-sName {
    color: gainsboro
}

.elementName--mName {
    color: greenyellow
}

.elementName__dName {
    color: aqua
}

.nmsp-ComponentName {
    color: red
}
```
```
processors: [
  require('postcss-bem')(),
  require('postcss-nested')()
```
