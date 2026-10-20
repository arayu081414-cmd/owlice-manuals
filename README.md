# Owlice 配布マニュアル

受講者に URL で渡すマニュアルを置く場所。GitHub Pages で配信している。

| ページ | URL |
|---|---|
| Qoo10 入金設定マニュアル（ショップ情報ページ本文のコピー機能つき） | https://arayu081414-cmd.github.io/owlice-manuals/qoo10-payout.html |

## 更新のしかた

元データは `~/Desktop/Anthem資料/_src/qoo10-payout/`。

```sh
cd ~/Desktop/Anthem資料/_src/qoo10-payout
python3 web.py                                   # web/qoo10-payout-web.html を作り直す
cp web/qoo10-payout-web.html ~/owlice-manuals/qoo10-payout.html
cd ~/owlice-manuals && git add -A && git commit -m "update qoo10-payout" && git push
```

push の1〜2分後に反映される。

## 注意

- **公開ページ**。URLを知っていれば誰でも見られる。機密を含むものは置かない。
- 各HTMLは画像を埋め込んだ自己完結ファイル。外部参照は無い。
