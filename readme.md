## React Native Base

A react native styles sheet with inspiration from Mapbox Base. *A work in progress, there is still a lot to do*.

Example:

```js
var React = require('react-native');
var b = require('react-native-base');

var {
  AppRegistry,
  sheet,
  Text,
  View,
} = React;

var base = React.createClass({
  render: function() {
    return (
      <View style={[b.container, b.fillCyan, b.textAlingCenter, b.alignItemsCenter, b.justifyContentCenter]}>
        <Text style={b.h2}>
          Welcome to React Native!
        </Text>
        <Text style={[b.textAlingCenter, b.pad1, b.keylineAll, b.round]}>
          To get started, edit index.iob.js
        </Text>
        <Text style={b.textAlingCenter}>
          Press Cmd+R to reload,{'\n'}
          Cmd+D or shake for dev menu
        </Text>
      </View>
    );
  }
});

AppRegistry.registerComponent('base', () => base);
```
