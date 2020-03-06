# template-writing-with-gitlab
GitLab で執筆する作用を行うためのテンプレートリポジトリ。  
GitLab CI を使って lint で校正して re:VIEW 経由で PDF にする。  

docs ディレクトリに md ファイル、画像ファイルを images ディレクトリには配置する。  
catalog.yml を自動生成するのでmdファイルをわけて管理する場合は、ファイルの命名を意識しないと意図したならびにならない。  
意図したならびにしたい場合は、.gitlab-ci.yml の catalog.yml の自動生成ではなく自分でファイルをメンテナンスする事。  