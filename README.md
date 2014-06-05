# Heroku Static Provider

Static site provider for Heroku.


## Installation

You need sign-in or sign-up to Heroku.

    $ git clone https://github.com/nulltask/heroku-static-provider.git my-site
    $ cd my-site
    $ heroku create
    $ git push -u heroku master
    $ heroku open

## Deployment

Add or update files in `/public`.

    $ git add .
    $ git commit -a -m 'some commit message'
    $ git push heroku master
    $ heroku open


1. まずHerokuでアプリを作る。

2. リポジトリをクローンする。
$ git clone git@heroku.com:webgl-video-imageprocessing.git -o heroku

3. 別のディレクトリでひな形サイトを取得する。
$ git clone git@github.com:DaisukeHirata/StaticSiteForHeroku.git

4. 3のファイルを２のリポジトリにコピーする。3は消して構わない。

5. 開発物（htmlとかjsとか）をpublic以下に加える。git commit する。

6. push先をherokuに。
$ git push -u heroku master

7. ブラウザでopen 
$ heroku open

## Notes

### Adding Basic Auth

	$ heroku config:set USER=username
	$ heroku config:set PASS=password

### Screencast

  * https://vimeo.com/71315109

## License

MIT
