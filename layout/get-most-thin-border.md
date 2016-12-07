使用`borderWidth: 1 / PixelRatio.get()`来获取最新边框

```js
import React, { Component } from 'react'
import {
  AppRegistry,
  StyleSheet,
  Text,
  View
} from 'react-native'

class App extends Component {
  render() {
    return (
      <View>
        <View style={{ borderWidth: 1, borderColor: 'red', height: 40, marginBottom: 20 }}></View>
        <View style={{ borderWidth: 1 / PixelRatio.get(), borderColor: 'red', height: 40 }}></View>
      </View>
    )
  }
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    marginTop: 25
  }
})

AppRegistry.registerComponent('App', () => App);
```
