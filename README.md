# template-writing-with-gitlab ![Docker Cloud Automated build](https://img.shields.io/docker/cloud/automated/ricordanza/writing-with-gitlab-textlint) ![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/ricordanza/writing-with-gitlab-textlint)

GitLab で執筆する作用を行うためのテンプレートリポジトリ。  
GitLab CI を使って lint で校正して re:VIEW 経由で PDF にする。  

docs ディレクトリに md ファイル、画像ファイルを images ディレクトリには配置する。  
catalog.yml を自動生成するのでmdファイルをわけて管理する場合は、ファイルの命名を意識しないと意図したならびにならない。  
意図したならびにしたい場合は、.gitlab-ci.yml の catalog.yml の自動生成ではなく自分でファイルをメンテナンスする事。  

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/from-referrer/)

## image
[![dockeri.co](https://dockeri.co/image/ricordanza/writing-with-gitlab-textlint)](https://hub.docker.com/r/ricordanza/writing-with-gitlab-textlint)

## textlint
以下の内容をチェックします。
- aws-spellcheck
- preset-ja-technical-writing
- spellcheck-tech-word

## Gipod Workspace
以下の拡張機能を導入しています。
- [テキスト校正くん](https://marketplace.visualstudio.com/items?itemName=ICS.japanese-proofreading)
- [vscode-textlint](https://marketplace.visualstudio.com/items?itemName=taichi.vscode-textlint)
- [CharacterCount](https://marketplace.visualstudio.com/items?itemName=8amjp.charactercount)

ファイルの保存時にフォーマットをかけるようにしているのでlintで修正可能なものは自動修します。
