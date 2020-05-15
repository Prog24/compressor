# compressor
引数で与えられたファイルを gzip（bzip2）圧縮を行うプログラム．

## 依存ライブラリ
```
- args4j-2.33.jar
  - コマンドライン引数の解析に利用．
- annotations-19.0.0.jar
  - @NotNull を利用．
- commons-compress-1.20.jar
  - bzip2 圧縮に利用．
```

## build
```bash
./gradlew build
```

## 使用方法
```
java -jar compressor-all.jar [OPTIONS] <FILES...>
OPTIONS
    -c, --compress <ALGORITHM>    specifies compress algorithm. Default is "gzip".
                                  Available: gzip, and bzip2.
    -d, --delete-original         Delete original files after compression.
    -v, --version                 print version.
    -h, --help                    print this message.
```
