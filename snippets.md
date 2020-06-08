#### taro
- page
```js
import { ComponentClass } from 'react'
import Taro, { Component, Config } from '@tarojs/taro'
import { View } from '@tarojs/components'

type PageStateProps = {}

type PageDispatchProps = {}

type PageOwnProps = {
}

type PageState = {}

type IProps = PageStateProps & PageDispatchProps & PageOwnProps

interface Index {
  props: IProps;
}

class Index extends Component {

  config: Config = {
    navigationBarTitleText: ''
  }

  componentWillReceiveProps (nextProps) {
    console.log(this.props, nextProps)
  }

  componentWillUnmount () { }

  componentDidShow () { }

  componentDidHide () { }

  render () {
    return (
      <View>
      </View>
    )
  }
}

export default Index as ComponentClass<PageOwnProps, PageState>
```

- components

```js
import { ComponentClass } from 'react'
import Taro, { Component } from '@tarojs/taro'
import { View } from '@tarojs/components'

type PageStateProps = {}

type PageDispatchProps = {}

type PageOwnProps = {
}

type PageState = {}

type IProps = PageStateProps & PageDispatchProps & PageOwnProps

interface Index {
  props: IProps;
}

class Index extends Component {
  componentWillReceiveProps (nextProps) {
    console.log(this.props, nextProps)
  }
  render () {
    return (
      <View>
      </View>
    )
  }
}

export default Index as ComponentClass<PageOwnProps, PageState>

```
