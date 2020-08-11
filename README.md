## Installation
```
npm install react-native-prototype-to-scrollview
```

## Usage

```
support to lib `react-native-scroll-lazy`
```

```js
import PrototypeToScrollview from 'react-native-prototype-to-scrollview'

class App extends React.Component {

  render() {
    return (
      <Animated.ScrollView
                ref={ele => this._scrollResponder = ele}
                {...this.props}
            />
    );
  }

  getScrollResponder = () => this._scrollResponder;

  handleScrollTo = (x, y) => this.scrollTo(x, y)
}

Object.assign(App.prototype, PrototypeToScrollview);
```