
## 教材タイトル
"Django REST frameworkでAPIを作る: ユーザー認証APIの構築"

## 教材概要
このセクションでは、Django REST frameworkを使ってユーザー認証APIを作成します。ユーザーの登録、ログイン、ログアウト機能をもつ基本的なAPIの設計と実装を通じて、Django REST frameworkの基本的な使用方法を学びます。

## 教材テキスト
```1. Djangoプロジェクトの作成   Djangoプロジェクトを新たに作成します。ターミナルで以下のコマンドを実行してください。   ```   $ django-admin startproject restapi   ```

## サンプルコード
```python# accounts/views.pyfrom django.contrib.auth.models import Userfrom rest_framework import statusfrom rest_framework.decorators import api_viewfrom rest_framework.response import Responsefrom .serializers import UserSerializer

## 作業手順
1. ターミナルを開き、新たにDjangoプロジェクトを作成します。2. 作成したプロジェクトの中で新たにDjangoアプリケーションを作成します。3. Djangoプロジェクトの設定ファイル(`restapi/settings.py`)を開き、`INSTALLED_APPS`に`'rest_framework'`と`'accounts'`を追加します。4. `accounts/views.py`ファイルにユーザー登録、ログイン、ログアウトのビューを作成し、`accounts/urls.py`ファイルにそれぞれのビューへのURLを設定します。5. ターミナルでサーバーを起動し、ブラウザから各APIにアクセスしてテストします。