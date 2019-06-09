# デバッグビルド

通常のビルドはリリースビルドと呼ばれ、
実行時に不要な情報を省いて最適化を行うことで高いパフォーマンスを実現しています。

コードにおけるファイルや行番号をはじめ、
デバッグで必要な情報の多くはリリースビルドでは省かれてしまうため、
デバッグを行うためにはデバッグビルドでビルドしたものを使用します。

デバッグビルドを行うためには `-g` を指定します。

<!-- TODO: -O0 のような最適化抑制も必要か確認する -->

```bash
$ g++ -std=c++11 -g main.cc
```