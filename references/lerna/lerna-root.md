# lerna root에서 각 Packages 제어하기

## Usage

1) lerna init
```bash
lerna init -i
```

2) package 만들기
```bash
cd ./packages && mkdir test
```

3) test npm init
```bash
npm init
```

4) lerna link convert
```bash
# 1. lerna bootstrap
lerna bootstrap
# 2. lerna link convert
lerna link convert
# 3. lerna re-bootstrap
lerna bootstrap
```

5) file 확인
```js
{
  "dependencies": {
    "test": "file:packages/test"
  }
}
```