# lorem-ipsum-demo-master Heroku.
Finished link:
<br>https://lorem-ipsum-demo-3.herokuapp.com/
## 1.insstall herokou from the link below:
<br>Heroku on mac
<br>https://github.com/GlennOu66304/Udacity-Data-Scientist/blob/master/2.%E5%AE%9E%E6%88%98%E9%A1%B9%E7%9B%AE:%20%E7%81%BE%E5%AE%B3%E5%BA%94%E5%AF%B9%E7%AE%A1%E9%81%93/Heroku%20on%20mac.md

## 2. download the code from link below:( I will list the Code fold under project too)
pg0408 /lorem-ipsum-demo
<br>https://github.com/pg0408/lorem-ipsum-demo

## 3. git inial project
```
Last login: Sun May 10 00:13:47 on ttys000
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % cd /Users/zhanghuiqiao/Downloads/((((b(((b((b(b(b(b((b(((((((base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro lorem-ipsum-demo-master % git init  
Initialized empty Git repository in /Users/zhanghuiqiao/Downloads/lorem-ipsum-demo-master/.git/
```
## 4. heroku login
```
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro lorem-ipsum-demo-master % heroku login 
heroku: Press any key to open up the browser to login or q to exit: 
Opening browser to https://cli-auth.heroku.com/auth/cli/browser/9b08b8c2-0e63-431c-85ce-640c919e3209
Logging in... done
Logged in as 1564468177glen@gmail.com
```
### 5. Hero create a project
```
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro lorem-ipsum-demo-master % heroku create lorem-ipsum-demo-2 
Creating ⬢ lorem-ipsum-demo-2... !
 ▸    Name lorem-ipsum-demo-2 is already taken
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro lorem-ipsum-demo-master % heroku create lorem-ipsum-demo-3 
Creating ⬢ lorem-ipsum-demo-3... done
````
### 6. deploy the project to herku
```
https://lorem-ipsum-demo-3.herokuapp.com/ | https://git.heroku.com/lorem-ipsum-demo-3.git
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro lorem-ipsum-demo-master % git add .  
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro lorem-ipsum-demo-master % git commit -m "ready to deploy" 
[master (root-commit) 9e0459f] ready to deploy
 336 files changed, 53931 insertions(+)
 create mode 100644 .DS_Store
 create mode 100644 Procfile
 create mode 100644 README.md
 create mode 100644 app.js
 create mode 120000 node_modules/.bin/mime
 create mode 100644 node_modules/accepts/HISTORY.md
 create mode 100644 node_modules/accepts/LICENSE
 create mode 100644 node_modules/accepts/README.md
 create mode 100644 node_modules/accepts/index.js
 create mode 100644 node_modules/accepts/package.json
 create mode 100644 node_modules/array-flatten/LICENSE
 create mode 100644 node_modules/array-flatten/README.md
 create mode 100644 node_modules/array-flatten/array-flatten.js
 create mode 100644 node_modules/array-flatten/package.json
 create mode 100644 node_modules/body-parser/HISTORY.md
 create mode 100644 node_modules/body-parser/LICENSE
 create mode 100644 node_modules/body-parser/README.md
 create mode 100644 node_modules/body-parser/index.js
 create mode 100644 node_modules/body-parser/lib/read.js
 create mode 100644 node_modules/body-parser/lib/types/json.js
 create mode 100644 node_modules/body-parser/lib/types/raw.js
 create mode 100644 node_modules/body-parser/lib/types/text.js
 create mode 100644 node_modules/body-parser/lib/types/urlencoded.js
 create mode 100644 node_modules/body-parser/package.json
 create mode 100644 node_modules/bytes/History.md
 create mode 100644 node_modules/bytes/LICENSE
 create mode 100644 node_modules/bytes/Readme.md
 create mode 100644 node_modules/bytes/index.js
 create mode 100644 node_modules/bytes/package.json
 create mode 100644 node_modules/content-disposition/HISTORY.md
 create mode 100644 node_modules/content-disposition/LICENSE
 create mode 100644 node_modules/content-disposition/README.md
 create mode 100644 node_modules/content-disposition/index.js
 create mode 100644 node_modules/content-disposition/package.json
 create mode 100644 node_modules/content-type/HISTORY.md
 create mode 100644 node_modules/content-type/LICENSE
 create mode 100644 node_modules/content-type/README.md
 create mode 100644 node_modules/content-type/index.js
 create mode 100644 node_modules/content-type/package.json
 create mode 100644 node_modules/cookie-signature/.npmignore
 create mode 100644 node_modules/cookie-signature/History.md
 create mode 100644 node_modules/cookie-signature/Readme.md
 create mode 100644 node_modules/cookie-signature/index.js
 create mode 100644 node_modules/cookie-signature/package.json
 create mode 100644 node_modules/cookie/HISTORY.md
 create mode 100644 node_modules/cookie/LICENSE
 create mode 100644 node_modules/cookie/README.md
 create mode 100644 node_modules/cookie/index.js
 create mode 100644 node_modules/cookie/package.json
 create mode 100644 node_modules/debug/.coveralls.yml
 create mode 100644 node_modules/debug/.eslintrc
 create mode 100644 node_modules/debug/.npmignore
 create mode 100644 node_modules/debug/.travis.yml
 create mode 100644 node_modules/debug/CHANGELOG.md
 create mode 100644 node_modules/debug/LICENSE
 create mode 100644 node_modules/debug/Makefile
 create mode 100644 node_modules/debug/README.md
 create mode 100644 node_modules/debug/component.json
 create mode 100644 node_modules/debug/karma.conf.js
 create mode 100644 node_modules/debug/node.js
 create mode 100644 node_modules/debug/package.json
 create mode 100644 node_modules/debug/src/browser.js
 create mode 100644 node_modules/debug/src/debug.js
 create mode 100644 node_modules/debug/src/index.js
 create mode 100644 node_modules/debug/src/inspector-log.js
 create mode 100644 node_modules/debug/src/node.js
 create mode 100644 node_modules/depd/History.md
 create mode 100644 node_modules/depd/LICENSE
 create mode 100644 node_modules/depd/Readme.md
 create mode 100644 node_modules/depd/index.js
 create mode 100644 node_modules/depd/lib/browser/index.js
 create mode 100644 node_modules/depd/lib/compat/callsite-tostring.js
 create mode 100644 node_modules/depd/lib/compat/event-listener-count.js
 create mode 100644 node_modules/depd/lib/compat/index.js
 create mode 100644 node_modules/depd/package.json
 create mode 100644 node_modules/destroy/LICENSE
 create mode 100644 node_modules/destroy/README.md
 create mode 100644 node_modules/destroy/index.js
 create mode 100644 node_modules/destroy/package.json
 create mode 100644 node_modules/ee-first/LICENSE
 create mode 100644 node_modules/ee-first/README.md
 create mode 100644 node_modules/ee-first/index.js
 create mode 100644 node_modules/ee-first/package.json
 create mode 100644 node_modules/encodeurl/HISTORY.md
 create mode 100644 node_modules/encodeurl/LICENSE
 create mode 100644 node_modules/encodeurl/README.md
 create mode 100644 node_modules/encodeurl/index.js
 create mode 100644 node_modules/encodeurl/package.json
 create mode 100644 node_modules/escape-html/LICENSE
 create mode 100644 node_modules/escape-html/Readme.md
 create mode 100644 node_modules/escape-html/index.js
 create mode 100644 node_modules/escape-html/package.json
 create mode 100644 node_modules/etag/HISTORY.md
 create mode 100644 node_modules/etag/LICENSE
 create mode 100644 node_modules/etag/README.md
 create mode 100644 node_modules/etag/index.js
 create mode 100644 node_modules/etag/package.json
 create mode 100644 node_modules/express/History.md
 create mode 100644 node_modules/express/LICENSE
 create mode 100644 node_modules/express/Readme.md
 create mode 100644 node_modules/express/index.js
 create mode 100644 node_modules/express/lib/application.js
 create mode 100644 node_modules/express/lib/express.js
 create mode 100644 node_modules/express/lib/middleware/init.js
 create mode 100644 node_modules/express/lib/middleware/query.js
 create mode 100644 node_modules/express/lib/request.js
 create mode 100644 node_modules/express/lib/response.js
 create mode 100644 node_modules/express/lib/router/index.js
 create mode 100644 node_modules/express/lib/router/layer.js
 create mode 100644 node_modules/express/lib/router/route.js
 create mode 100644 node_modules/express/lib/utils.js
 create mode 100644 node_modules/express/lib/view.js
 create mode 100644 node_modules/express/package.json
 create mode 100644 node_modules/finalhandler/HISTORY.md
 create mode 100644 node_modules/finalhandler/LICENSE
 create mode 100644 node_modules/finalhandler/README.md
 create mode 100644 node_modules/finalhandler/index.js
 create mode 100644 node_modules/finalhandler/package.json
 create mode 100644 node_modules/forwarded/HISTORY.md
 create mode 100644 node_modules/forwarded/LICENSE
 create mode 100644 node_modules/forwarded/README.md
 create mode 100644 node_modules/forwarded/index.js
 create mode 100644 node_modules/forwarded/package.json
 create mode 100644 node_modules/fresh/HISTORY.md
 create mode 100644 node_modules/fresh/LICENSE
 create mode 100644 node_modules/fresh/README.md
 create mode 100644 node_modules/fresh/index.js
 create mode 100644 node_modules/fresh/package.json
 create mode 100644 node_modules/http-errors/HISTORY.md
 create mode 100644 node_modules/http-errors/LICENSE
 create mode 100644 node_modules/http-errors/README.md
 create mode 100644 node_modules/http-errors/index.js
 create mode 100644 node_modules/http-errors/package.json
 create mode 100644 node_modules/iconv-lite/Changelog.md
 create mode 100644 node_modules/iconv-lite/LICENSE
 create mode 100644 node_modules/iconv-lite/README.md
 create mode 100644 node_modules/iconv-lite/encodings/dbcs-codec.js
 create mode 100644 node_modules/iconv-lite/encodings/dbcs-data.js
 create mode 100644 node_modules/iconv-lite/encodings/index.js
 create mode 100644 node_modules/iconv-lite/encodings/internal.js
 create mode 100644 node_modules/iconv-lite/encodings/sbcs-codec.js
 create mode 100644 node_modules/iconv-lite/encodings/sbcs-data-generated.js
 create mode 100644 node_modules/iconv-lite/encodings/sbcs-data.js
 create mode 100644 node_modules/iconv-lite/encodings/tables/big5-added.json
 create mode 100644 node_modules/iconv-lite/encodings/tables/cp936.json
 create mode 100644 node_modules/iconv-lite/encodings/tables/cp949.json
 create mode 100644 node_modules/iconv-lite/encodings/tables/cp950.json
 create mode 100644 node_modules/iconv-lite/encodings/tables/eucjp.json
 create mode 100644 node_modules/iconv-lite/encodings/tables/gb18030-ranges.json
 create mode 100644 node_modules/iconv-lite/encodings/tables/gbk-added.json
 create mode 100644 node_modules/iconv-lite/encodings/tables/shiftjis.json
 create mode 100644 node_modules/iconv-lite/encodings/utf16.js
 create mode 100644 node_modules/iconv-lite/encodings/utf7.js
 create mode 100644 node_modules/iconv-lite/lib/bom-handling.js
 create mode 100644 node_modules/iconv-lite/lib/extend-node.js
 create mode 100644 node_modules/iconv-lite/lib/index.d.ts
 create mode 100644 node_modules/iconv-lite/lib/index.js
 create mode 100644 node_modules/iconv-lite/lib/streams.js
 create mode 100644 node_modules/iconv-lite/package.json
 create mode 100644 node_modules/inherits/LICENSE
 create mode 100644 node_modules/inherits/README.md
 create mode 100644 node_modules/inherits/inherits.js
 create mode 100644 node_modules/inherits/inherits_browser.js
 create mode 100644 node_modules/inherits/package.json
 create mode 100644 node_modules/ipaddr.js/LICENSE
 create mode 100644 node_modules/ipaddr.js/README.md
 create mode 100644 node_modules/ipaddr.js/ipaddr.min.js
 create mode 100644 node_modules/ipaddr.js/lib/ipaddr.js
 create mode 100644 node_modules/ipaddr.js/lib/ipaddr.js.d.ts
 create mode 100644 node_modules/ipaddr.js/package.json
 create mode 100644 node_modules/media-typer/HISTORY.md
 create mode 100644 node_modules/media-typer/LICENSE
 create mode 100644 node_modules/media-typer/README.md
 create mode 100644 node_modules/media-typer/index.js
 create mode 100644 node_modules/media-typer/package.json
 create mode 100644 node_modules/merge-descriptors/HISTORY.md
 create mode 100644 node_modules/merge-descriptors/LICENSE
 create mode 100644 node_modules/merge-descriptors/README.md
 create mode 100644 node_modules/merge-descriptors/index.js
 create mode 100644 node_modules/merge-descriptors/package.json
 create mode 100644 node_modules/methods/HISTORY.md
 create mode 100644 node_modules/methods/LICENSE
 create mode 100644 node_modules/methods/README.md
 create mode 100644 node_modules/methods/index.js
 create mode 100644 node_modules/methods/package.json
 create mode 100644 node_modules/mime-db/HISTORY.md
 create mode 100644 node_modules/mime-db/LICENSE
 create mode 100644 node_modules/mime-db/README.md
 create mode 100644 node_modules/mime-db/db.json
 create mode 100644 node_modules/mime-db/index.js
 create mode 100644 node_modules/mime-db/package.json
 create mode 100644 node_modules/mime-types/HISTORY.md
 create mode 100644 node_modules/mime-types/LICENSE
 create mode 100644 node_modules/mime-types/README.md
 create mode 100644 node_modules/mime-types/index.js
 create mode 100644 node_modules/mime-types/package.json
 create mode 100644 node_modules/mime/.npmignore
 create mode 100644 node_modules/mime/CHANGELOG.md
 create mode 100644 node_modules/mime/LICENSE
 create mode 100644 node_modules/mime/README.md
 create mode 100755 node_modules/mime/cli.js
 create mode 100644 node_modules/mime/mime.js
 create mode 100644 node_modules/mime/package.json
 create mode 100755 node_modules/mime/src/build.js
 create mode 100644 node_modules/mime/src/test.js
 create mode 100644 node_modules/mime/types.json
 create mode 100644 node_modules/ms/index.js
 create mode 100644 node_modules/ms/license.md
 create mode 100644 node_modules/ms/package.json
 create mode 100644 node_modules/ms/readme.md
 create mode 100644 node_modules/negotiator/HISTORY.md
 create mode 100644 node_modules/negotiator/LICENSE
 create mode 100644 node_modules/negotiator/README.md
 create mode 100644 node_modules/negotiator/index.js
 create mode 100644 node_modules/negotiator/lib/charset.js
 create mode 100644 node_modules/negotiator/lib/encoding.js
 create mode 100644 node_modules/negotiator/lib/language.js
 create mode 100644 node_modules/negotiator/lib/mediaType.js
 create mode 100644 node_modules/negotiator/package.json
 create mode 100644 node_modules/on-finished/HISTORY.md
 create mode 100644 node_modules/on-finished/LICENSE
 create mode 100644 node_modules/on-finished/README.md
 create mode 100644 node_modules/on-finished/index.js
 create mode 100644 node_modules/on-finished/package.json
 create mode 100644 node_modules/parseurl/HISTORY.md
 create mode 100644 node_modules/parseurl/LICENSE
 create mode 100644 node_modules/parseurl/README.md
 create mode 100644 node_modules/parseurl/index.js
 create mode 100644 node_modules/parseurl/package.json
 create mode 100644 node_modules/path-to-regexp/History.md
 create mode 100644 node_modules/path-to-regexp/LICENSE
 create mode 100644 node_modules/path-to-regexp/Readme.md
 create mode 100644 node_modules/path-to-regexp/index.js
 create mode 100644 node_modules/path-to-regexp/package.json
 create mode 100644 node_modules/proxy-addr/HISTORY.md
 create mode 100644 node_modules/proxy-addr/LICENSE
 create mode 100644 node_modules/proxy-addr/README.md
 create mode 100644 node_modules/proxy-addr/index.js
 create mode 100644 node_modules/proxy-addr/package.json
 create mode 100644 node_modules/qs/.editorconfig
 create mode 100644 node_modules/qs/.eslintignore
 create mode 100644 node_modules/qs/.eslintrc
 create mode 100644 node_modules/qs/CHANGELOG.md
 create mode 100644 node_modules/qs/LICENSE
 create mode 100644 node_modules/qs/README.md
 create mode 100644 node_modules/qs/dist/qs.js
 create mode 100644 node_modules/qs/lib/formats.js
 create mode 100644 node_modules/qs/lib/index.js
 create mode 100644 node_modules/qs/lib/parse.js
 create mode 100644 node_modules/qs/lib/stringify.js
 create mode 100644 node_modules/qs/lib/utils.js
 create mode 100644 node_modules/qs/package.json
 create mode 100644 node_modules/qs/test/.eslintrc
 create mode 100644 node_modules/qs/test/index.js
 create mode 100644 node_modules/qs/test/parse.js
 create mode 100644 node_modules/qs/test/stringify.js
 create mode 100644 node_modules/qs/test/utils.js
 create mode 100644 node_modules/range-parser/HISTORY.md
 create mode 100644 node_modules/range-parser/LICENSE
 create mode 100644 node_modules/range-parser/README.md
 create mode 100644 node_modules/range-parser/index.js
 create mode 100644 node_modules/range-parser/package.json
 create mode 100644 node_modules/raw-body/HISTORY.md
 create mode 100644 node_modules/raw-body/LICENSE
 create mode 100644 node_modules/raw-body/README.md
 create mode 100644 node_modules/raw-body/index.d.ts
 create mode 100644 node_modules/raw-body/index.js
 create mode 100644 node_modules/raw-body/package.json
 create mode 100644 node_modules/safe-buffer/LICENSE
 create mode 100644 node_modules/safe-buffer/README.md
 create mode 100644 node_modules/safe-buffer/index.d.ts
 create mode 100644 node_modules/safe-buffer/index.js
 create mode 100644 node_modules/safe-buffer/package.json
 create mode 100644 node_modules/safer-buffer/LICENSE
 create mode 100644 node_modules/safer-buffer/Porting-Buffer.md
 create mode 100644 node_modules/safer-buffer/Readme.md
 create mode 100644 node_modules/safer-buffer/dangerous.js
 create mode 100644 node_modules/safer-buffer/package.json
 create mode 100644 node_modules/safer-buffer/safer.js
 create mode 100644 node_modules/safer-buffer/tests.js
 create mode 100644 node_modules/send/HISTORY.md
 create mode 100644 node_modules/send/LICENSE
 create mode 100644 node_modules/send/README.md
 create mode 100644 node_modules/send/index.js
 create mode 100644 node_modules/send/node_modules/ms/index.js
 create mode 100644 node_modules/send/node_modules/ms/license.md
 create mode 100644 node_modules/send/node_modules/ms/package.json
 create mode 100644 node_modules/send/node_modules/ms/readme.md
 create mode 100644 node_modules/send/package.json
 create mode 100644 node_modules/serve-static/HISTORY.md
 create mode 100644 node_modules/serve-static/LICENSE
 create mode 100644 node_modules/serve-static/README.md
 create mode 100644 node_modules/serve-static/index.js
 create mode 100644 node_modules/serve-static/package.json
 create mode 100644 node_modules/setprototypeof/LICENSE
 create mode 100644 node_modules/setprototypeof/README.md
 create mode 100644 node_modules/setprototypeof/index.d.ts
 create mode 100644 node_modules/setprototypeof/index.js
 create mode 100644 node_modules/setprototypeof/package.json
 create mode 100644 node_modules/setprototypeof/test/index.js
 create mode 100644 node_modules/statuses/HISTORY.md
 create mode 100644 node_modules/statuses/LICENSE
 create mode 100644 node_modules/statuses/README.md
 create mode 100644 node_modules/statuses/codes.json
 create mode 100644 node_modules/statuses/index.js
 create mode 100644 node_modules/statuses/package.json
 create mode 100644 node_modules/toidentifier/LICENSE
 create mode 100644 node_modules/toidentifier/README.md
 create mode 100644 node_modules/toidentifier/index.js
 create mode 100644 node_modules/toidentifier/package.json
 create mode 100644 node_modules/type-is/HISTORY.md
 create mode 100644 node_modules/type-is/LICENSE
 create mode 100644 node_modules/type-is/README.md
 create mode 100644 node_modules/type-is/index.js
 create mode 100644 node_modules/type-is/package.json
 create mode 100644 node_modules/unpipe/HISTORY.md
 create mode 100644 node_modules/unpipe/LICENSE
 create mode 100644 node_modules/unpipe/README.md
 create mode 100644 node_modules/unpipe/index.js
 create mode 100644 node_modules/unpipe/package.json
 create mode 100644 node_modules/utils-merge/.npmignore
 create mode 100644 node_modules/utils-merge/LICENSE
 create mode 100644 node_modules/utils-merge/README.md
 create mode 100644 node_modules/utils-merge/index.js
 create mode 100644 node_modules/utils-merge/package.json
 create mode 100644 node_modules/vary/HISTORY.md
 create mode 100644 node_modules/vary/LICENSE
 create mode 100644 node_modules/vary/README.md
 create mode 100644 node_modules/vary/index.js
 create mode 100644 node_modules/vary/package.json
 create mode 100644 package-lock.json
 create mode 100644 package.json
 create mode 100644 public/index.html
 create mode 100644 public/lorem.json
 create mode 100644 public/script.js
 create mode 100644 public/styles.css
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro lorem-ipsum-demo-master % git push heroku master  
Enumerating objects: 401, done.
Counting objects: 100% (401/401), done.
Delta compression using up to 4 threads
Compressing objects: 100% (388/388), done.
Writing objects: 100% (401/401), 584.18 KiB | 4.29 MiB/s, done.
Total 401 (delta 74), reused 0 (delta 0)
remote: Compressing source files... done.
remote: Building source:
remote: 
remote: -----> Node.js app detected
remote:        
remote: -----> Creating runtime environment
remote:        
remote:        NPM_CONFIG_LOGLEVEL=error
remote:        NODE_ENV=production
remote:        NODE_MODULES_CACHE=true
remote:        NODE_VERBOSE=false
remote:        
remote: -----> Installing binaries
remote:        engines.node (package.json):  unspecified
remote:        engines.npm (package.json):   unspecified (use default)
remote:        
remote:        Resolving node version 12.x...
remote:        Downloading and installing node 12.16.3...
remote:        Using default npm version: 6.14.4
remote:        
remote: -----> Installing dependencies
remote:        Prebuild detected (node_modules already exists)
remote:        Rebuilding any native modules
remote:        express@4.17.1 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/express
remote:        accepts@1.3.7 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/accepts
remote:        mime-types@2.1.26 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/mime-types
remote:        mime-db@1.43.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/mime-db
remote:        negotiator@0.6.2 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/negotiator
remote:        array-flatten@1.1.1 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/array-flatten
remote:        body-parser@1.19.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/body-parser
remote:        bytes@3.1.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/bytes
remote:        content-type@1.0.4 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/content-type
remote:        debug@2.6.9 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/debug
remote:        ms@2.0.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/ms
remote:        depd@1.1.2 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/depd
remote:        http-errors@1.7.2 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/http-errors
remote:        inherits@2.0.3 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/inherits
remote:        setprototypeof@1.1.1 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/setprototypeof
remote:        statuses@1.5.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/statuses
remote:        toidentifier@1.0.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/toidentifier
remote:        iconv-lite@0.4.24 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/iconv-lite
remote:        safer-buffer@2.1.2 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/safer-buffer
remote:        on-finished@2.3.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/on-finished
remote:        ee-first@1.1.1 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/ee-first
remote:        qs@6.7.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/qs
remote:        raw-body@2.4.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/raw-body
remote:        unpipe@1.0.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/unpipe
remote:        type-is@1.6.18 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/type-is
remote:        media-typer@0.3.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/media-typer
remote:        content-disposition@0.5.3 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/content-disposition
remote:        safe-buffer@5.1.2 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/safe-buffer
remote:        cookie@0.4.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/cookie
remote:        cookie-signature@1.0.6 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/cookie-signature
remote:        encodeurl@1.0.2 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/encodeurl
remote:        escape-html@1.0.3 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/escape-html
remote:        etag@1.8.1 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/etag
remote:        finalhandler@1.1.2 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/finalhandler
remote:        parseurl@1.3.3 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/parseurl
remote:        fresh@0.5.2 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/fresh
remote:        merge-descriptors@1.0.1 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/merge-descriptors
remote:        methods@1.1.2 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/methods
remote:        path-to-regexp@0.1.7 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/path-to-regexp
remote:        proxy-addr@2.0.6 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/proxy-addr
remote:        forwarded@0.1.2 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/forwarded
remote:        ipaddr.js@1.9.1 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/ipaddr.js
remote:        range-parser@1.2.1 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/range-parser
remote:        send@0.17.1 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/send
remote:        destroy@1.0.4 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/destroy
remote:        mime@1.6.0 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/mime
remote:        ms@2.1.1 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/send/node_modules/ms
remote:        serve-static@1.14.1 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/serve-static
remote:        utils-merge@1.0.1 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/utils-merge
remote:        vary@1.1.2 /tmp/build_b1ae02cd487ad06f076d1094f6b19419/node_modules/vary
remote:        Installing any new modules (package.json)
remote:        audited 126 packages in 0.854s
remote:        found 0 vulnerabilities
remote:        
remote:        
remote: -----> Build
remote:        
remote: -----> Caching build
remote:        - node_modules
remote:        
remote: -----> Pruning devDependencies
remote:        audited 126 packages in 0.964s
remote:        found 0 vulnerabilities
remote:        
remote:        
remote: -----> Build succeeded!
remote: -----> Discovering process types
remote:        Procfile declares types -> web
remote: 
remote: -----> Compressing...
remote:        Done: 22.7M
remote: -----> Launching...
remote:        Released v3
remote:        https://lorem-ipsum-demo-3.herokuapp.com/ deployed to Heroku
remote: 
remote: Verifying deploy... done.
To https://git.heroku.com/lorem-ipsum-demo-3.git
 * [new branch]      master -> master
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro lorem-ipsum-demo-master % 
```
## 7. Run project in local, you can use http://localhost:3000/ to log into the webpage.
```
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % cd /Users/zhanghuiqiao/Downloads/lorem-ipsum-demo-master
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro lorem-ipsum-demo-master % node /Users/zhanghuiqiao/Downloads/lorem-ipsum-demo-master/app.js
Server is running...
```
## 8. Log of Heroku
```
Last login: Sun May 10 00:14:37 on ttys001
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro ~ % cd /Users/zhanghuiqiao/Downloads/lorem-ipsum-demo-master     
(base) zhanghuiqiao@zhanghuiqiaodeMacBook-Pro lorem-ipsum-demo-master % heroku logs --tail 
2020-05-09T16:17:28.352260+00:00 app[api]: Initial release by user 1564468177glen@gmail.com
2020-05-09T16:17:28.352260+00:00 app[api]: Release v1 created by user 1564468177glen@gmail.com
2020-05-09T16:17:28.505402+00:00 app[api]: Enable Logplex by user 1564468177glen@gmail.com
2020-05-09T16:17:28.505402+00:00 app[api]: Release v2 created by user 1564468177glen@gmail.com
2020-05-09T16:18:42.000000+00:00 app[api]: Build started by user 1564468177glen@gmail.com
2020-05-09T16:18:55.689710+00:00 app[api]: Deploy 9e0459f6 by user 1564468177glen@gmail.com
2020-05-09T16:18:55.689710+00:00 app[api]: Release v3 created by user 1564468177glen@gmail.com
2020-05-09T16:18:55.705337+00:00 app[api]: Scaled to web@1:Free by user 1564468177glen@gmail.com
2020-05-09T16:18:56.000000+00:00 app[api]: Build succeeded
2020-05-09T16:19:01.145516+00:00 app[web.1]: Server is running...
2020-05-09T16:19:02.487353+00:00 heroku[web.1]: State changed from starting to up
2020-05-09T16:19:09.010693+00:00 heroku[router]: at=info method=GET path="/" host=lorem-ipsum-demo-3.herokuapp.com request_id=8d328dc3-c614-4ac7-bf02-d3b46f14773c fwd="104.247.130.170" dyno=web.1 connect=1ms service=39ms status=200 bytes=915 protocol=https
2020-05-09T16:19:09.821479+00:00 heroku[router]: at=info method=GET path="/styles.css" host=lorem-ipsum-demo-3.herokuapp.com request_id=5cc9fa1c-8a05-40fb-8a0a-bb6370cc6959 fwd="104.247.130.170" dyno=web.1 connect=0ms service=13ms status=200 bytes=626 protocol=https
2020-05-09T16:19:10.590409+00:00 heroku[router]: at=info method=GET path="/script.js" host=lorem-ipsum-demo-3.herokuapp.com request_id=9e8a9b30-3073-44e7-81b3-95f0bfa53a8f fwd="104.247.130.170" dyno=web.1 connect=0ms service=5ms status=200 bytes=28635 protocol=https
2020-05-09T16:19:11.154422+00:00 heroku[router]: at=info method=GET path="/favicon.ico" host=lorem-ipsum-demo-3.herokuapp.com request_id=f7d943d8-5969-4efc-bfbf-d440205a7636 fwd="104.247.130.170" dyno=web.1 connect=1ms service=17ms status=404 bytes=394 protocol=https
```

## 9. Possible help page:
How to deploy your app to the web using Express.js and Heroku
<br>https://www.freecodecamp.org/news/how-to-deploy-your-site-using-express-and-heroku/
<br>http://localhost:3000/
<br>How do I read Medium articles for free?
<br>https://www.quora.com/How-do-I-read-Medium-articles-for-free
<br>Can't push to the heroku
<br>https://stackoverflow.com/questions/38841284/cant-push-to-the-heroku/50905814
<br>Why does my app "fail to detect" a buildpack?
<br>https://help.heroku.com/1MC2J0GF/why-does-my-app-fail-to-detect-a-buildpack
<br>Logging
<br>https://devcenter.heroku.com/articles/logging#view-logs
<br>How to fix npm ERR! missing script: start
<br>https://techoverflow.net/2019/04/01/how-to-fix-npm-err-missing-script-start/
<br>Start script missing error when running npm start
<br>https://stackoverflow.com/questions/31976722/start-script-missing-error-when-running-npm-start
<br>Staging Files with Git
<br>https://rubygarage.org/blog/most-basic-git-commands-with-examples#article_title_6
