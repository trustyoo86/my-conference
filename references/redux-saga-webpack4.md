# webpack4 사용시 redux-saga middleware 적용 이슈

webpack4내에서 `redux-saga` 의 createSagaMiddleware가 error가 나는 관계로 적용이 어려움

```bash
exception: reduxSaga2.default is not function
```

해당 수정을 위해 js단에서 변경

```js
import createSagaMiddleware from 'redux-saga';

const sagaMiddleware = typeof createSagaMiddleware === 'function' ? createSagaMiddleware() : createSagaMiddleware.default();
```