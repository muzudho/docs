# クリーンアップ方法


## キャッシュ・クリアー

```shell
pnpm store prune
# （pnpm ではなく npm が悪さをしてるなら） npm cache clean --force
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
