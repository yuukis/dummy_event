# "現実をつなぐゲームサーバーの設計と実装"

## 教材概要
この教材では、自分だけのRPGゲームサーバーを設計し、PythonのDjango REST frameworkを使用して実装を行います。Django REST frameworkの基本的な機能を学びつつ、自らの想像を形にするプロセスを体験します。サーバーがどのように動作し、クライアントとどのように連携を取るかを学びます。

## 教材テキスト
1. **ゲームサーバーの設計**<br>
まずはゲームサーバーの設計から始めましょう。ゲームの世界観、キャラクター、物語の流れなどを考え、それをどのようにサーバーで実現するかを考えます。

## サンプルコード
```python
from django.shortcuts import render
from rest_framework import viewsets
from .models import Character
from .serializers import CharacterSerializer