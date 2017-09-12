# Angular4 + Systemjs module loader
[![Build Status][travis-badge]][travis-badge-url]

This repo is forked from [angular.io quickstart], then added a third party library cornerstone to do window leveling on image.

1. Before run the application, install:

- node: 6.11.3
- yarn: 0.24.5

2. Use command `yarn install` to install `node_modules`

3. Run command `yarn run start` to run the application

4. Because of CORS issue during access the cloud image (see details: http://rawgit.com/chafey/cornerstoneWebImageLoader/master/examples/index.html), open a new terminal and do the following steps to fix it:
   4.1 run `mkdir /tmp/chrome_dev_session` to create chrome_dev_session folder under tmp
   4.2 run `open -n -a /Applications/Google\ Chrome.app --args --user-data-dir="/tmp/chrome_dev_session" --disable-web-security` to start a Chrome without security check.

5. Visit `http://localhost:3000/` in new started Chrome.

6. Click "window leveling" button multiple times, the time cost of for loop from cornerstone library will output in the console. The performance is pretty good.

<a href="https://imgur.com/J33noLt"><img src="https://i.imgur.com/J33noLt.png" title="source: imgur.com" width="400" /></a>


