Hook可以在不编写class的情况下使用state以及其他React的特性

Hook是一些可以在函数组件里“钩入”React state及生命周期等特性的函数。Hook不能在class组件中使用 ——这能让你不使用class也能使用React

## 1. 组件之间复用状态逻辑很难

当组件之间需要共享一些状态时，就会在状态管理中出现很多相关的逻辑代码。一般会使用高阶组件或者renderPropos来处理这些逻辑的复用。但是这两种方法都有缺点（本处不再详细描述），所以使用Hook来处理这些逻辑。Hook相对以上两种方法有以下优点：

#### 写法简单

#### 组合简单

#### 容易扩展

#### 没有Wrapper hell

## 2. 复杂的组件可读性差

如果一个组件的逻辑很复杂，就有可能导致每个生命周期包含一些不相关的代码。而Hook可以讲组件中相互关联的部分拆的颗粒度更小，似的代码更简洁，结果也更加可预测。

## 3. Class组件现存的一些问题

class组件中this的复杂性以及生命周期函数的不确定性都使得class组件是一个难以使用的存在。想要使用函数组件却没有对应的状态管理，所以Hook就实现了一些和生命周期函数类似的功能，解决了以上问题。

class组件存在一些问题

hook实现了一些和生命周期函数类似的功能

this过于复杂

生命周期不稳定

复杂的组件可读性差

