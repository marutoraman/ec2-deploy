EC2デプロイ手順
====
既に基本的な初期構築作業は完了している前提とします。

# リポジトリClone
```
git clone <リポジトリのurl>
```

# venv環境を作成
```
cd <リポジトリ名>
python3 -m venv venv
. venv/bin/activate
pip install requirements.txt
```

# .envの作成
```sudo vi .env```で.envを開き、以下を追記して保存
DB_PATH='<接続用のDB_PATH>'


# 実行
python main/run.py "検索したいキーワード"
