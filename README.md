# Bleak

An elegant AJAX driven theme for [Ghost](http://github.com/tryghost/ghost/) by [Peter Amende](http://zutrinken.com/).

## Demo

* [Blog](http://bleak.zutrinken.com)
* [Post](http://bleak.zutrinken.com/demo)
* [Tags](http://bleak.zutrinken.com/tag/general)
* [Author](http://bleak.zutrinken.com/author/zutrinken)

## Screenshots

<table>
<tr>
<td valign="top">
<img src="https://raw.githubusercontent.com/zutrinken/bleak/master/src/screenshot-desktop.jpg" />
</td>
<td valign="top">
<img src="https://raw.githubusercontent.com/zutrinken/bleak/master/src/screenshot-mobile.jpg" />
</td>
</tr>
</table>

## Features

* Responsive layout
* Blog navigation
* Post navigation
* Cover images for blog, tag and author archives
* Featured posts style
* Automatic code syntax highlight and line numbers
* Disqus/Gitalk support
* Subscribers support
* Sharing buttons

## Setup

To enable [Disqus](https://disqus.com/) comments go to your blogs code injection settings and add `<script>var disqus="YOUR_DISQUS_SHORTNAME";</script>` to your blog header. You can also try [Gitalk](https://github.com/gitalk/gitalk), a comment system based on Github Issue. Just need insert its dependencies and config to the blogs code injection.

```
<link rel="stylesheet" href="https://unpkg.com/gitalk/dist/gitalk.css">
<script src="https://cdnjs.cloudflare.com/ajax/libs/blueimp-md5/2.10.0/js/md5.min.js"></script>
<script src="https://unpkg.com/gitalk/dist/gitalk.min.js"></script>
<script>
var gitalkConf = {
  clientID: 'YOUR_GITHUB_APP_CLIENTID',
  clientSecret: 'YOUR_GITHUB_APP_CLIENTSECRET',
  repo: 'YOUR_GITHUB_REPO',
  owner: 'YOUR_GITHUB_ACCOUNT',
  admin: ['YOUR_GITHUB_ACCOUNT'],
  id: md5(location.pathname),
  // facebook-like distraction free mode
  distractionFreeMode: false
};
</script>
```

## Development

Install [Grunt](http://gruntjs.com/getting-started/):

	npm install -g grunt-cli

Install Grunt modules:

	npm install

Install [Bower](http://bower.io):

	npm install -g bower

Install Bower components:

	bower install

Build Grunt project:

	grunt

Distribute Grunt project:

	grunt build

## Copyright & License

Copyright (C) 2015-2018 Peter Amende - Released under the [MIT License](https://github.com/zutrinken/bleak/blob/master/LICENSE).
