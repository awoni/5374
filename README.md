# 徳島市版5374について
本家版に以下の機能を追加しています。

### 隔週、3週毎、4週毎、5週毎の収集及び年末・年始休業のずらしに対応
徳島市の場合、隔週及び4週毎の収集があるために隔週等の収集に対応させました。
area_days.csvに第3月曜日であれば「月3」と記載する代わりに、隔週の収集で収集日が2015年4月21日にあった場合には、「e2w20150421」と書けば、2週間毎に表示できるようにしています。e2wの2が2週間おきということで、4週毎であればe4w20150421と書きます。8週毎というようなのはあまリないと思いますが計算は可能です。

### ごみの出し方のルールを表示
徳島市でごみの分別について詳しく記載した「家庭ごみ分別ガイド」がすでにあるため、ごみの出し方のルールを表示するようにしました。

### 収集地区への対応
徳島市の場合、地区数は多いのですが、収集日は4つの収集地区しかないため、地区の収集スケジュールのファイル（area_days.csv）を地区名のファイル（area.csv）と収集日のファイル（area_days.csv）のファイルに分割して、データの作成作業を軽減できるようにしました。

### 先付けの日付でのテスト対応
年末・年始の処理を事前にテストできるように、日付をパラメータで渡せるように修正しています。

現在テスト中です。
