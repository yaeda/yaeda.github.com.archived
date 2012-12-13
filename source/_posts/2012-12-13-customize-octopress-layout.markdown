---
layout: post
title: "Customize Octopress Layout"
date: 2012-12-13 00:14
comments: true
categories: octopress
---

タイトルが長く，iPhoneのブラウザで表示するとはみ出してしまうのが気になったので，レイアウトを修正してみた．

OctopressのレイアウトはSassで書かれている．`sass/custom/_style.scss`が最後にimportされるので，ここに書けばスタイルを上書きすることができる．

iPhone用にこんな感じにしてみた．

``` css
@media only screen and (max-device-width: 480px) {
    body > header { font-size: .85em; }
}

```

こんな感じになった．

BEFORE <--> AFTER

<a href="http://www.flickr.com/photos/22927952@N03/8267422765/" title="Untitled by yaeda, on Flickr"><img src="http://farm9.staticflickr.com/8349/8267422765_a6927e6feb.jpg" width="333" height="500" alt="Untitled"></a>
<a href="http://www.flickr.com/photos/22927952@N03/8268493392/" title="Untitled by yaeda, on Flickr"><img src="http://farm9.staticflickr.com/8216/8268493392_4184af3096.jpg" width="333" height="500" alt="Untitled"></a>

とはいうものの (この画像のレイアウトもそうだけど）デフォルトテーマはちょっと微妙ですね．次はThemeでも変えてみるかな．