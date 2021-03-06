# MicroFrontendsのコアアイディア

・ Be Technology Agnostic

　各チームは技術において他チームの影響を受けません。
　各チームは、他のチームと調整しなくても、スタックを選択してアップグレードできる必要があります。カスタム要素は、他のユーザーに中立的なインターフェイスを提供しながら、実装の詳細を隠すための優れた方法です。

・ Isolate Team Code

技術同様、実際のコードも共有しません。また、状態やグローバル変数、コーディングルールなども互いに依存しないよう独立して機能させます。

すべてのチームが同じフレームワークを使用している場合でも、ランタイムを共有しないでください。自己完結型の独立したアプリを構築します。共有状態またはグローバル変数に依存しないでください。

・ Establish Team Prefixes

　チームの Prefix を定める
　互いのコンフリクトを避けるため、チームの Prefix を定めて管理することが推奨されています。

　所有権を明確にするための名前空間CSS、イベント、ローカルストレージおよびCookie。

　本当にクロスチームAPIを構築する必要がある場合は、できるだけシンプルに保つようにしてください。

・ Build a Resilient Site　回復力があるサイトを構築する。

　 JavaScriptが失敗したり、まだ実行されていない場合でも、この機能は役立つはずです。

　　※詳しい情報
　　https://resilientwebdesign.com/


#　Web開発のトレンド

現在のWebのトレンドは多機能なSPAです。

SPAとはSPA(Single Page Application)の略です。

単一のWebページでアプリケーションを構成する設計構造の名称です。

特徴：

・単一のWebページでコンテンツ切り替えを行う	
			
・ページ遷移の必要がなくなり
				
・ブラウザの挙動に縛られないWeb表現を可能


# サンプル機能概要

トラクターストアの製品ページに下記の機能があります。

①3つ異なるトラクターモデルを切り替える。
②製品イメージを変更すると、名前、価格、推奨事項が更新されます。
③選択したモデルをバスケットに追加する。
購入ボタンを押すと、それに応じて更新される上部のミニバスケットもあります。

# Run Sample

    docker-compose up --build

http://127.0.0.1:3000/
