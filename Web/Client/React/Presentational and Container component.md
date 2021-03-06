# Presentational and Container components

## Sources
- [Presentational and Container Components](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0#.hwc2nicf5)
- [Usage with React](http://redux.js.org/docs/basics/UsageWithReact.html)

|               | Presentational           | Container  |
| ------------- |:-------------:| :-----:|
| Purpose       | How things look | How things work |
| Aware of Redux      | No      |   Yes |
| To read data | Read data from props      |   Subscribe to Redux state |
| To change data | Invoke callbacks from props | Dispatch Redux actions |
| Are written | By hand | Usually generated by React Redux |