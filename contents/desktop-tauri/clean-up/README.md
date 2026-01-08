# クリーンアップ方法

数 GB の容量を削減できることも。  


## キャッシュ・クリアー

（パワーシェルではなく）コマンドプロンプトを使う。  

```shell
# フロントエンド
pnpm store prune

# （pnpm ではなく npm が悪さをしてるなら）
#npm cache clean --force
```

```shell
# バックエンド
cd src-tauri
cargo clean
```

（ソースから生成できるので）削除してもいいフォルダーとファイル：  

```plaintext
# Tauriの場合：

📁 /
├─ 📁 node_modules 削除
├─ ( 📁 src-tauri )
│   ├─ 📁 target 削除
│   └─ 📄 Cargo.lock 削除
└─ 📄 pnpm-lock.yaml 削除
```
