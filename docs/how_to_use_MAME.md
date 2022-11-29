# 変換には関係ないこと。

romsへデータを配置する。zipはそのまま、chdはディレクトリを作成

```
mkdir $ZIP_NAME
mv $CHD $ZIP_NAME
```

tree だとこんな感じ

```sh
# e.g. beatmania THE FINAL

cd ./mame/0.249
tree
...
├── roms
│   ├── bmfinal
│   │   └── c01jaa11.chd
│   ├── bmfinal.zip
│   └── dir.txt
...
```
