# mocha-jsdom

## Usage

1\) mocha-jsdom 설치

```bash
npm install mocha-jsdom --save-dev
```

2\) test 파일 내에서 jsdom 호출

```javascript
describe('[test]', () => {
  before(() => {
    jsdom();
  });
});
```

## Issue

localStorage 이슈 발생하는 경우 강제로 url내 localhost 삽입

```javascript
jsdom({
  url: 'http://localhost',
})
```

