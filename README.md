# react_pro_static
静态HTML文件使用react demo

	<!--仅用于开发-->
	<script crossorigin src="https://unpkg.com/react@16/umd/react.development.js"></script>
	<script crossorigin src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
	
	<!--用于生产-->
	<script crossorigin src="https://unpkg.com/react@16/umd/react.production.min.js"></script>
	<script crossorigin src="https://unpkg.com/react-dom@16/umd/react-dom.production.min.js"></script>

	<script src="https://unpkg.com/babel-standalone@6.26.0/babel.js"></script>


React - React顶级API

React DOM - 添加特定于DOM的方法

Babel - 一种JavaScript编译器，允许我们在旧浏览器中使用ES6 +


使用ES6类来创建一个名为的React组件App。

	class App extends React.Component {
	  //...
	}

添加render()方法，这是类组件中唯一需要的方法，用于呈现DOM节点。

	class App extends React.Component {
	  render() {
	      return (
	          //...
	      );
	  }
	}

我们不会在此处返回字符串，因此请勿在元素周围使用引号。这被称为JSX，可以去了解它。

	class App extends React.Component {
	  render() {
	    return <h1>Hello world!</h1>
	  }
	}

使用React DOM render()方法将App我们创建的类呈现到rootHTML中的div中。

ReactDOM.render(<App />, document.getElementById('root'))
