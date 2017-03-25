# api-documentation for  [backbone (v1.3.3)](https://github.com/jashkenas/backbone#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-backbone.svg)](https://travis-ci.org/npmdoc/node-npmdoc-backbone)
#### Give your JS App some Backbone with Models, Views, Collections, and Events.

[![NPM](https://nodei.co/npm/backbone.png?downloads=true)](https://www.npmjs.com/package/backbone)

# html version

- [https://npmdoc.github.io/node-npmdoc-backbone/build..beta..travis-ci.org/apidoc.html](https://npmdoc.github.io/node-npmdoc-backbone/build..beta..travis-ci.org/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-backbone/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-backbone_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-backbone/build..beta..travis-ci.org/apidoc.html)

# package listing

![package-listing](https://npmdoc.github.io/node-npmdoc-backbone/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Jeremy Ashkenas"
    },
    "bugs": {
        "url": "https://github.com/jashkenas/backbone/issues"
    },
    "dependencies": {
        "underscore": ">=1.8.3"
    },
    "description": "Give your JS App some Backbone with Models, Views, Collections, and Events.",
    "devDependencies": {
        "coffee-script": "1.7.1",
        "docco": "0.7.0",
        "eslint": "1.10.x",
        "karma": "^0.13.13",
        "karma-phantomjs-launcher": "^0.1.4",
        "karma-qunit": "^0.1.5",
        "qunitjs": "^1.18.0",
        "uglify-js": "^2.4.17"
    },
    "directories": {},
    "dist": {
        "shasum": "4cc80ea7cb1631ac474889ce40f2f8bc683b2999",
        "tarball": "https://registry.npmjs.org/backbone/-/backbone-1.3.3.tgz"
    },
    "files": [
        "backbone.js",
        "backbone-min.js",
        "backbone-min.map",
        "LICENSE"
    ],
    "gitHead": "8ec88604732944f197b352a6be22c8216ea9d3a1",
    "homepage": "https://github.com/jashkenas/backbone#readme",
    "keywords": [
        "model",
        "view",
        "controller",
        "router",
        "server",
        "client",
        "browser"
    ],
    "license": "MIT",
    "main": "backbone.js",
    "maintainers": [
        {
            "name": "braddunbar",
            "email": "dunbarb2@gmail.com"
        },
        {
            "name": "jashkenas",
            "email": "jashkenas@gmail.com"
        },
        {
            "name": "jridgewell",
            "email": "justin+npm@ridgewell.name"
        }
    ],
    "name": "backbone",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/jashkenas/backbone.git"
    },
    "scripts": {
        "build": "uglifyjs backbone.js --mangle --source-map backbone-min.map -o backbone-min.js",
        "doc": "docco backbone.js && docco examples/todos/todos.js examples/backbone.localStorage.js",
        "lint": "eslint backbone.js test/*.js",
        "test": "karma start && coffee test/model.coffee && npm run lint"
    },
    "url": "http://backbonejs.org",
    "version": "1.3.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module backbone](#apidoc.module.backbone)
1.  boolean <span class="apidocSignatureSpan">backbone.</span>emulateHTTP
1.  boolean <span class="apidocSignatureSpan">backbone.</span>emulateJSON
1.  [function <span class="apidocSignatureSpan">backbone.</span>Collection (models, options)](#apidoc.element.backbone.Collection)
1.  [function <span class="apidocSignatureSpan">backbone.</span>History ()](#apidoc.element.backbone.History)
1.  [function <span class="apidocSignatureSpan">backbone.</span>Model (attributes, options)](#apidoc.element.backbone.Model)
1.  [function <span class="apidocSignatureSpan">backbone.</span>Router (options)](#apidoc.element.backbone.Router)
1.  [function <span class="apidocSignatureSpan">backbone.</span>View (options)](#apidoc.element.backbone.View)
1.  [function <span class="apidocSignatureSpan">backbone.</span>ajax ()](#apidoc.element.backbone.ajax)
1.  [function <span class="apidocSignatureSpan">backbone.</span>bind (name, callback, context)](#apidoc.element.backbone.bind)
1.  [function <span class="apidocSignatureSpan">backbone.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.listenTo)
1.  [function <span class="apidocSignatureSpan">backbone.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.listenToOnce)
1.  [function <span class="apidocSignatureSpan">backbone.</span>noConflict ()](#apidoc.element.backbone.noConflict)
1.  [function <span class="apidocSignatureSpan">backbone.</span>off (name, callback, context)](#apidoc.element.backbone.off)
1.  [function <span class="apidocSignatureSpan">backbone.</span>on (name, callback, context)](#apidoc.element.backbone.on)
1.  [function <span class="apidocSignatureSpan">backbone.</span>once (name, callback, context)](#apidoc.element.backbone.once)
1.  [function <span class="apidocSignatureSpan">backbone.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.stopListening)
1.  [function <span class="apidocSignatureSpan">backbone.</span>sync (method, model, options)](#apidoc.element.backbone.sync)
1.  [function <span class="apidocSignatureSpan">backbone.</span>trigger (name)](#apidoc.element.backbone.trigger)
1.  [function <span class="apidocSignatureSpan">backbone.</span>unbind (name, callback, context)](#apidoc.element.backbone.unbind)
1.  object <span class="apidocSignatureSpan">backbone.</span>Collection.prototype
1.  object <span class="apidocSignatureSpan">backbone.</span>Events
1.  object <span class="apidocSignatureSpan">backbone.</span>History.prototype
1.  object <span class="apidocSignatureSpan">backbone.</span>Model.prototype
1.  object <span class="apidocSignatureSpan">backbone.</span>Router.prototype
1.  object <span class="apidocSignatureSpan">backbone.</span>View.prototype
1.  object <span class="apidocSignatureSpan">backbone.</span>history
1.  string <span class="apidocSignatureSpan">backbone.</span>VERSION

#### [module backbone.Collection](#apidoc.module.backbone.Collection)
1.  [function <span class="apidocSignatureSpan">backbone.</span>Collection (models, options)](#apidoc.element.backbone.Collection.Collection)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.</span>extend (protoProps, staticProps)](#apidoc.element.backbone.Collection.extend)

#### [module backbone.Collection.prototype](#apidoc.module.backbone.Collection.prototype)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_addReference (model, options)](#apidoc.element.backbone.Collection.prototype._addReference)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_isModel (model)](#apidoc.element.backbone.Collection.prototype._isModel)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_onModelEvent (event, model, collection, options)](#apidoc.element.backbone.Collection.prototype._onModelEvent)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_prepareModel (attrs, options)](#apidoc.element.backbone.Collection.prototype._prepareModel)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_removeModels (models, options)](#apidoc.element.backbone.Collection.prototype._removeModels)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_removeReference (model, options)](#apidoc.element.backbone.Collection.prototype._removeReference)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_reset ()](#apidoc.element.backbone.Collection.prototype._reset)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>add (models, options)](#apidoc.element.backbone.Collection.prototype.add)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>all (iteratee, context)](#apidoc.element.backbone.Collection.prototype.all)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>any (iteratee, context)](#apidoc.element.backbone.Collection.prototype.any)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>at (index)](#apidoc.element.backbone.Collection.prototype.at)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>bind (name, callback, context)](#apidoc.element.backbone.Collection.prototype.bind)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>chain ()](#apidoc.element.backbone.Collection.prototype.chain)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>clone ()](#apidoc.element.backbone.Collection.prototype.clone)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>collect (iteratee, context)](#apidoc.element.backbone.Collection.prototype.collect)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>contains (iteratee, context)](#apidoc.element.backbone.Collection.prototype.contains)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>countBy (iteratee, context)](#apidoc.element.backbone.Collection.prototype.countBy)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>create (model, options)](#apidoc.element.backbone.Collection.prototype.create)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>detect (iteratee, context)](#apidoc.element.backbone.Collection.prototype.detect)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>difference ()](#apidoc.element.backbone.Collection.prototype.difference)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>drop (iteratee, context)](#apidoc.element.backbone.Collection.prototype.drop)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>each (iteratee, context)](#apidoc.element.backbone.Collection.prototype.each)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>every (iteratee, context)](#apidoc.element.backbone.Collection.prototype.every)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>fetch (options)](#apidoc.element.backbone.Collection.prototype.fetch)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>filter (iteratee, context)](#apidoc.element.backbone.Collection.prototype.filter)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>find (iteratee, context)](#apidoc.element.backbone.Collection.prototype.find)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>findIndex (iteratee, context)](#apidoc.element.backbone.Collection.prototype.findIndex)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>findLastIndex (iteratee, context)](#apidoc.element.backbone.Collection.prototype.findLastIndex)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>findWhere (attrs)](#apidoc.element.backbone.Collection.prototype.findWhere)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>first (iteratee, context)](#apidoc.element.backbone.Collection.prototype.first)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>foldl ()](#apidoc.element.backbone.Collection.prototype.foldl)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>foldr ()](#apidoc.element.backbone.Collection.prototype.foldr)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>forEach (iteratee, context)](#apidoc.element.backbone.Collection.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>get (obj)](#apidoc.element.backbone.Collection.prototype.get)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>groupBy (iteratee, context)](#apidoc.element.backbone.Collection.prototype.groupBy)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>has (obj)](#apidoc.element.backbone.Collection.prototype.has)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>head (iteratee, context)](#apidoc.element.backbone.Collection.prototype.head)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>include (iteratee, context)](#apidoc.element.backbone.Collection.prototype.include)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>includes (iteratee, context)](#apidoc.element.backbone.Collection.prototype.includes)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>indexBy (iteratee, context)](#apidoc.element.backbone.Collection.prototype.indexBy)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>indexOf (iteratee, context)](#apidoc.element.backbone.Collection.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>initial (iteratee, context)](#apidoc.element.backbone.Collection.prototype.initial)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>initialize ()](#apidoc.element.backbone.Collection.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>inject ()](#apidoc.element.backbone.Collection.prototype.inject)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>invoke ()](#apidoc.element.backbone.Collection.prototype.invoke)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>isEmpty ()](#apidoc.element.backbone.Collection.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>last (iteratee, context)](#apidoc.element.backbone.Collection.prototype.last)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>lastIndexOf (iteratee, context)](#apidoc.element.backbone.Collection.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.Collection.prototype.listenTo)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.Collection.prototype.listenToOnce)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>map (iteratee, context)](#apidoc.element.backbone.Collection.prototype.map)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>max (iteratee, context)](#apidoc.element.backbone.Collection.prototype.max)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>min (iteratee, context)](#apidoc.element.backbone.Collection.prototype.min)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>model (attributes, options)](#apidoc.element.backbone.Collection.prototype.model)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>modelId (attrs)](#apidoc.element.backbone.Collection.prototype.modelId)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>off (name, callback, context)](#apidoc.element.backbone.Collection.prototype.off)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>on (name, callback, context)](#apidoc.element.backbone.Collection.prototype.on)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>once (name, callback, context)](#apidoc.element.backbone.Collection.prototype.once)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>parse (resp, options)](#apidoc.element.backbone.Collection.prototype.parse)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>partition (iteratee, context)](#apidoc.element.backbone.Collection.prototype.partition)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>pluck (attr)](#apidoc.element.backbone.Collection.prototype.pluck)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>pop (options)](#apidoc.element.backbone.Collection.prototype.pop)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>push (model, options)](#apidoc.element.backbone.Collection.prototype.push)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>reduce ()](#apidoc.element.backbone.Collection.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>reduceRight ()](#apidoc.element.backbone.Collection.prototype.reduceRight)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>reject (iteratee, context)](#apidoc.element.backbone.Collection.prototype.reject)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>remove (models, options)](#apidoc.element.backbone.Collection.prototype.remove)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>reset (models, options)](#apidoc.element.backbone.Collection.prototype.reset)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>rest (iteratee, context)](#apidoc.element.backbone.Collection.prototype.rest)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>sample (iteratee, context)](#apidoc.element.backbone.Collection.prototype.sample)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>select (iteratee, context)](#apidoc.element.backbone.Collection.prototype.select)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>set (models, options)](#apidoc.element.backbone.Collection.prototype.set)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>shift (options)](#apidoc.element.backbone.Collection.prototype.shift)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>shuffle ()](#apidoc.element.backbone.Collection.prototype.shuffle)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>size ()](#apidoc.element.backbone.Collection.prototype.size)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>slice ()](#apidoc.element.backbone.Collection.prototype.slice)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>some (iteratee, context)](#apidoc.element.backbone.Collection.prototype.some)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>sort (options)](#apidoc.element.backbone.Collection.prototype.sort)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>sortBy (iteratee, context)](#apidoc.element.backbone.Collection.prototype.sortBy)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.Collection.prototype.stopListening)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>sync ()](#apidoc.element.backbone.Collection.prototype.sync)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>tail (iteratee, context)](#apidoc.element.backbone.Collection.prototype.tail)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>take (iteratee, context)](#apidoc.element.backbone.Collection.prototype.take)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>toArray ()](#apidoc.element.backbone.Collection.prototype.toArray)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>toJSON (options)](#apidoc.element.backbone.Collection.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>trigger (name)](#apidoc.element.backbone.Collection.prototype.trigger)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>unbind (name, callback, context)](#apidoc.element.backbone.Collection.prototype.unbind)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>unshift (model, options)](#apidoc.element.backbone.Collection.prototype.unshift)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>where (attrs, first)](#apidoc.element.backbone.Collection.prototype.where)
1.  [function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>without ()](#apidoc.element.backbone.Collection.prototype.without)

#### [module backbone.Events](#apidoc.module.backbone.Events)
1.  [function <span class="apidocSignatureSpan">backbone.Events.</span>bind (name, callback, context)](#apidoc.element.backbone.Events.bind)
1.  [function <span class="apidocSignatureSpan">backbone.Events.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.Events.listenTo)
1.  [function <span class="apidocSignatureSpan">backbone.Events.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.Events.listenToOnce)
1.  [function <span class="apidocSignatureSpan">backbone.Events.</span>off (name, callback, context)](#apidoc.element.backbone.Events.off)
1.  [function <span class="apidocSignatureSpan">backbone.Events.</span>on (name, callback, context)](#apidoc.element.backbone.Events.on)
1.  [function <span class="apidocSignatureSpan">backbone.Events.</span>once (name, callback, context)](#apidoc.element.backbone.Events.once)
1.  [function <span class="apidocSignatureSpan">backbone.Events.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.Events.stopListening)
1.  [function <span class="apidocSignatureSpan">backbone.Events.</span>trigger (name)](#apidoc.element.backbone.Events.trigger)
1.  [function <span class="apidocSignatureSpan">backbone.Events.</span>unbind (name, callback, context)](#apidoc.element.backbone.Events.unbind)

#### [module backbone.History](#apidoc.module.backbone.History)
1.  boolean <span class="apidocSignatureSpan">backbone.History.</span>started
1.  [function <span class="apidocSignatureSpan">backbone.</span>History ()](#apidoc.element.backbone.History.History)
1.  [function <span class="apidocSignatureSpan">backbone.History.</span>extend (protoProps, staticProps)](#apidoc.element.backbone.History.extend)

#### [module backbone.History.prototype](#apidoc.module.backbone.History.prototype)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>_updateHash (location, fragment, replace)](#apidoc.element.backbone.History.prototype._updateHash)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>atRoot ()](#apidoc.element.backbone.History.prototype.atRoot)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>bind (name, callback, context)](#apidoc.element.backbone.History.prototype.bind)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>checkUrl (e)](#apidoc.element.backbone.History.prototype.checkUrl)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>decodeFragment (fragment)](#apidoc.element.backbone.History.prototype.decodeFragment)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>getFragment (fragment)](#apidoc.element.backbone.History.prototype.getFragment)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>getHash (window)](#apidoc.element.backbone.History.prototype.getHash)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>getPath ()](#apidoc.element.backbone.History.prototype.getPath)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>getSearch ()](#apidoc.element.backbone.History.prototype.getSearch)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.History.prototype.listenTo)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.History.prototype.listenToOnce)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>loadUrl (fragment)](#apidoc.element.backbone.History.prototype.loadUrl)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>matchRoot ()](#apidoc.element.backbone.History.prototype.matchRoot)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>navigate (fragment, options)](#apidoc.element.backbone.History.prototype.navigate)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>off (name, callback, context)](#apidoc.element.backbone.History.prototype.off)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>on (name, callback, context)](#apidoc.element.backbone.History.prototype.on)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>once (name, callback, context)](#apidoc.element.backbone.History.prototype.once)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>route (route, callback)](#apidoc.element.backbone.History.prototype.route)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>start (options)](#apidoc.element.backbone.History.prototype.start)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>stop ()](#apidoc.element.backbone.History.prototype.stop)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.History.prototype.stopListening)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>trigger (name)](#apidoc.element.backbone.History.prototype.trigger)
1.  [function <span class="apidocSignatureSpan">backbone.History.prototype.</span>unbind (name, callback, context)](#apidoc.element.backbone.History.prototype.unbind)
1.  number <span class="apidocSignatureSpan">backbone.History.prototype.</span>interval

#### [module backbone.Model](#apidoc.module.backbone.Model)
1.  [function <span class="apidocSignatureSpan">backbone.</span>Model (attributes, options)](#apidoc.element.backbone.Model.Model)
1.  [function <span class="apidocSignatureSpan">backbone.Model.</span>extend (protoProps, staticProps)](#apidoc.element.backbone.Model.extend)

#### [module backbone.Model.prototype](#apidoc.module.backbone.Model.prototype)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>_validate (attrs, options)](#apidoc.element.backbone.Model.prototype._validate)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>bind (name, callback, context)](#apidoc.element.backbone.Model.prototype.bind)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>chain ()](#apidoc.element.backbone.Model.prototype.chain)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>changedAttributes (diff)](#apidoc.element.backbone.Model.prototype.changedAttributes)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>clear (options)](#apidoc.element.backbone.Model.prototype.clear)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>clone ()](#apidoc.element.backbone.Model.prototype.clone)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>destroy (options)](#apidoc.element.backbone.Model.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>escape (attr)](#apidoc.element.backbone.Model.prototype.escape)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>fetch (options)](#apidoc.element.backbone.Model.prototype.fetch)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>get (attr)](#apidoc.element.backbone.Model.prototype.get)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>has (attr)](#apidoc.element.backbone.Model.prototype.has)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>hasChanged (attr)](#apidoc.element.backbone.Model.prototype.hasChanged)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>initialize ()](#apidoc.element.backbone.Model.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>invert ()](#apidoc.element.backbone.Model.prototype.invert)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>isEmpty ()](#apidoc.element.backbone.Model.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>isNew ()](#apidoc.element.backbone.Model.prototype.isNew)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>isValid (options)](#apidoc.element.backbone.Model.prototype.isValid)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>keys ()](#apidoc.element.backbone.Model.prototype.keys)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.Model.prototype.listenTo)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.Model.prototype.listenToOnce)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>matches (attrs)](#apidoc.element.backbone.Model.prototype.matches)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>off (name, callback, context)](#apidoc.element.backbone.Model.prototype.off)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>omit ()](#apidoc.element.backbone.Model.prototype.omit)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>on (name, callback, context)](#apidoc.element.backbone.Model.prototype.on)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>once (name, callback, context)](#apidoc.element.backbone.Model.prototype.once)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>pairs ()](#apidoc.element.backbone.Model.prototype.pairs)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>parse (resp, options)](#apidoc.element.backbone.Model.prototype.parse)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>pick ()](#apidoc.element.backbone.Model.prototype.pick)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>previous (attr)](#apidoc.element.backbone.Model.prototype.previous)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>previousAttributes ()](#apidoc.element.backbone.Model.prototype.previousAttributes)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>save (key, val, options)](#apidoc.element.backbone.Model.prototype.save)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>set (key, val, options)](#apidoc.element.backbone.Model.prototype.set)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.Model.prototype.stopListening)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>sync ()](#apidoc.element.backbone.Model.prototype.sync)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>toJSON (options)](#apidoc.element.backbone.Model.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>trigger (name)](#apidoc.element.backbone.Model.prototype.trigger)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>unbind (name, callback, context)](#apidoc.element.backbone.Model.prototype.unbind)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>unset (attr, options)](#apidoc.element.backbone.Model.prototype.unset)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>url ()](#apidoc.element.backbone.Model.prototype.url)
1.  [function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>values ()](#apidoc.element.backbone.Model.prototype.values)
1.  object <span class="apidocSignatureSpan">backbone.Model.prototype.</span>changed
1.  object <span class="apidocSignatureSpan">backbone.Model.prototype.</span>validationError
1.  string <span class="apidocSignatureSpan">backbone.Model.prototype.</span>cidPrefix
1.  string <span class="apidocSignatureSpan">backbone.Model.prototype.</span>idAttribute

#### [module backbone.Router](#apidoc.module.backbone.Router)
1.  [function <span class="apidocSignatureSpan">backbone.</span>Router (options)](#apidoc.element.backbone.Router.Router)
1.  [function <span class="apidocSignatureSpan">backbone.Router.</span>extend (protoProps, staticProps)](#apidoc.element.backbone.Router.extend)

#### [module backbone.Router.prototype](#apidoc.module.backbone.Router.prototype)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>_bindRoutes ()](#apidoc.element.backbone.Router.prototype._bindRoutes)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>_extractParameters (route, fragment)](#apidoc.element.backbone.Router.prototype._extractParameters)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>_routeToRegExp (route)](#apidoc.element.backbone.Router.prototype._routeToRegExp)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>bind (name, callback, context)](#apidoc.element.backbone.Router.prototype.bind)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>execute (callback, args, name)](#apidoc.element.backbone.Router.prototype.execute)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>initialize ()](#apidoc.element.backbone.Router.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.Router.prototype.listenTo)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.Router.prototype.listenToOnce)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>navigate (fragment, options)](#apidoc.element.backbone.Router.prototype.navigate)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>off (name, callback, context)](#apidoc.element.backbone.Router.prototype.off)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>on (name, callback, context)](#apidoc.element.backbone.Router.prototype.on)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>once (name, callback, context)](#apidoc.element.backbone.Router.prototype.once)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>route (route, name, callback)](#apidoc.element.backbone.Router.prototype.route)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.Router.prototype.stopListening)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>trigger (name)](#apidoc.element.backbone.Router.prototype.trigger)
1.  [function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>unbind (name, callback, context)](#apidoc.element.backbone.Router.prototype.unbind)

#### [module backbone.View](#apidoc.module.backbone.View)
1.  [function <span class="apidocSignatureSpan">backbone.</span>View (options)](#apidoc.element.backbone.View.View)
1.  [function <span class="apidocSignatureSpan">backbone.View.</span>extend (protoProps, staticProps)](#apidoc.element.backbone.View.extend)

#### [module backbone.View.prototype](#apidoc.module.backbone.View.prototype)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>_createElement (tagName)](#apidoc.element.backbone.View.prototype._createElement)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>_ensureElement ()](#apidoc.element.backbone.View.prototype._ensureElement)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>_removeElement ()](#apidoc.element.backbone.View.prototype._removeElement)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>_setAttributes (attributes)](#apidoc.element.backbone.View.prototype._setAttributes)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>_setElement (el)](#apidoc.element.backbone.View.prototype._setElement)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>bind (name, callback, context)](#apidoc.element.backbone.View.prototype.bind)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>delegate (eventName, selector, listener)](#apidoc.element.backbone.View.prototype.delegate)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>delegateEvents (events)](#apidoc.element.backbone.View.prototype.delegateEvents)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>initialize ()](#apidoc.element.backbone.View.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.View.prototype.listenTo)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.View.prototype.listenToOnce)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>off (name, callback, context)](#apidoc.element.backbone.View.prototype.off)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>on (name, callback, context)](#apidoc.element.backbone.View.prototype.on)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>once (name, callback, context)](#apidoc.element.backbone.View.prototype.once)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>remove ()](#apidoc.element.backbone.View.prototype.remove)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>render ()](#apidoc.element.backbone.View.prototype.render)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>setElement (element)](#apidoc.element.backbone.View.prototype.setElement)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.View.prototype.stopListening)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>trigger (name)](#apidoc.element.backbone.View.prototype.trigger)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>unbind (name, callback, context)](#apidoc.element.backbone.View.prototype.unbind)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>undelegate (eventName, selector, listener)](#apidoc.element.backbone.View.prototype.undelegate)
1.  [function <span class="apidocSignatureSpan">backbone.View.prototype.</span>undelegateEvents ()](#apidoc.element.backbone.View.prototype.undelegateEvents)
1.  string <span class="apidocSignatureSpan">backbone.View.prototype.</span>tagName

#### [module backbone.history](#apidoc.module.backbone.history)
1.  [function <span class="apidocSignatureSpan">backbone.history.</span>checkUrl ()](#apidoc.element.backbone.history.checkUrl)
1.  object <span class="apidocSignatureSpan">backbone.history.</span>handlers



# <a name="apidoc.module.backbone"></a>[module backbone](#apidoc.module.backbone)

#### <a name="apidoc.element.backbone.Collection"></a>[function <span class="apidocSignatureSpan">backbone.</span>Collection (models, options)](#apidoc.element.backbone.Collection)
- description and source-code
```javascript
Collection = function (models, options) {
  options || (options = {});
  if (options.model) this.model = options.model;
  if (options.comparator !== void 0) this.comparator = options.comparator;
  this._reset();
  this.initialize.apply(this, arguments);
  if (models) this.reset(models, _.extend({silent: true}, options));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.History"></a>[function <span class="apidocSignatureSpan">backbone.</span>History ()](#apidoc.element.backbone.History)
- description and source-code
```javascript
History = function () {
  this.handlers = [];
  this.checkUrl = _.bind(this.checkUrl, this);

  // Ensure that 'History' can be used outside of the browser.
  if (typeof window !== 'undefined') {
    this.location = window.location;
    this.history = window.history;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model"></a>[function <span class="apidocSignatureSpan">backbone.</span>Model (attributes, options)](#apidoc.element.backbone.Model)
- description and source-code
```javascript
Model = function (attributes, options) {
  var attrs = attributes || {};
  options || (options = {});
  this.cid = _.uniqueId(this.cidPrefix);
  this.attributes = {};
  if (options.collection) this.collection = options.collection;
  if (options.parse) attrs = this.parse(attrs, options) || {};
  var defaults = _.result(this, 'defaults');
  attrs = _.defaults(_.extend({}, defaults, attrs), defaults);
  this.set(attrs, options);
  this.changed = {};
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Router"></a>[function <span class="apidocSignatureSpan">backbone.</span>Router (options)](#apidoc.element.backbone.Router)
- description and source-code
```javascript
Router = function (options) {
  options || (options = {});
  if (options.routes) this.routes = options.routes;
  this._bindRoutes();
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.View"></a>[function <span class="apidocSignatureSpan">backbone.</span>View (options)](#apidoc.element.backbone.View)
- description and source-code
```javascript
View = function (options) {
  this.cid = _.uniqueId('view');
  _.extend(this, _.pick(options, viewOptions));
  this._ensureElement();
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.ajax"></a>[function <span class="apidocSignatureSpan">backbone.</span>ajax ()](#apidoc.element.backbone.ajax)
- description and source-code
```javascript
ajax = function () {
  return Backbone.$.ajax.apply(Backbone.$, arguments);
}
```
- example usage
```shell
...
  options.error = function(xhr, textStatus, errorThrown) {
    options.textStatus = textStatus;
    options.errorThrown = errorThrown;
    if (error) error.call(options.context, xhr, textStatus, errorThrown);
  };

  // Make the request, allowing the user to override any Ajax options.
  var xhr = options.xhr = Backbone.ajax(_.extend(params, options));
  model.trigger('request', model, xhr, options);
  return xhr;
};

// Map from CRUD to HTTP for our default 'Backbone.sync' implementation.
var methodMap = {
  'create': 'POST',
...
```

#### <a name="apidoc.element.backbone.bind"></a>[function <span class="apidocSignatureSpan">backbone.</span>bind (name, callback, context)](#apidoc.element.backbone.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...

// Bind an event to only be triggered a single time. After the first time
// the callback is invoked, its listener will be removed. If multiple events
// are passed in using the space-separated syntax, the handler will fire
// once for each event, not once for a combination of all events.
Events.once = function(name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
...
```

#### <a name="apidoc.element.backbone.listenTo"></a>[function <span class="apidocSignatureSpan">backbone.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.listenTo)
- description and source-code
```javascript
listenTo = function (obj, name, callback) {
  if (!obj) return this;
  var id = obj._listenId || (obj._listenId = _.uniqueId('l'));
  var listeningTo = this._listeningTo || (this._listeningTo = {});
  var listening = listeningTo[id];

  // This object is not listening to any other events on 'obj' yet.
  // Setup the necessary references to track the listening callbacks.
  if (!listening) {
    var thisId = this._listenId || (this._listenId = _.uniqueId('l'));
    listening = listeningTo[id] = {obj: obj, objId: id, id: thisId, listeningTo: listeningTo, count: 0};
  }

  // Bind callbacks on obj, and keep track of them on listening.
  internalOn(obj, name, callback, this, listening);
  return this;
}
```
- example usage
```shell
...
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
...
```

#### <a name="apidoc.element.backbone.listenToOnce"></a>[function <span class="apidocSignatureSpan">backbone.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.listenToOnce)
- description and source-code
```javascript
listenToOnce = function (obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.noConflict"></a>[function <span class="apidocSignatureSpan">backbone.</span>noConflict ()](#apidoc.element.backbone.noConflict)
- description and source-code
```javascript
noConflict = function () {
  root.Backbone = previousBackbone;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.off"></a>[function <span class="apidocSignatureSpan">backbone.</span>off (name, callback, context)](#apidoc.element.backbone.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
...
  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
};

// The reducing API that removes a callback from the 'events' object.
var offApi = function(events, name, callback, options) {
...
```

#### <a name="apidoc.element.backbone.on"></a>[function <span class="apidocSignatureSpan">backbone.</span>on (name, callback, context)](#apidoc.element.backbone.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...
// A module that can be mixed in to *any object* in order to provide it with
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;
...
```

#### <a name="apidoc.element.backbone.once"></a>[function <span class="apidocSignatureSpan">backbone.</span>once (name, callback, context)](#apidoc.element.backbone.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
}
```
- example usage
```shell
...
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
      offer(name, once);
      callback.apply(this, arguments);
    });
    once._callback = callback;
  }
  return map;
};
...
```

#### <a name="apidoc.element.backbone.stopListening"></a>[function <span class="apidocSignatureSpan">backbone.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.stopListening)
- description and source-code
```javascript
stopListening = function (obj, name, callback) {
  var listeningTo = this._listeningTo;
  if (!listeningTo) return this;

  var ids = obj ? [obj._listenId] : _.keys(listeningTo);

  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
}
```
- example usage
```shell
...
    destroy: function(options) {
options = options ? _.clone(options) : {};
var model = this;
var success = options.success;
var wait = options.wait;

var destroy = function() {
  model.stopListening();
  model.trigger('destroy', model, model.collection, options);
};

options.success = function(resp) {
  if (wait) destroy();
  if (success) success.call(options.context, model, resp, options);
  if (!model.isNew()) model.trigger('sync', model, resp, options);
...
```

#### <a name="apidoc.element.backbone.sync"></a>[function <span class="apidocSignatureSpan">backbone.</span>sync (method, model, options)](#apidoc.element.backbone.sync)
- description and source-code
```javascript
sync = function (method, model, options) {
  var type = methodMap[method];

  // Default options, unless specified.
  _.defaults(options || (options = {}), {
    emulateHTTP: Backbone.emulateHTTP,
    emulateJSON: Backbone.emulateJSON
  });

  // Default JSON-request options.
  var params = {type: type, dataType: 'json'};

  // Ensure that we have a URL.
  if (!options.url) {
    params.url = _.result(model, 'url') || urlError();
  }

  // Ensure that we have the appropriate request data.
  if (options.data == null && model && (method === 'create' || method === 'update' || method === 'patch')) {
    params.contentType = 'application/json';
    params.data = JSON.stringify(options.attrs || model.toJSON(options));
  }

  // For older servers, emulate JSON by encoding the request into an HTML-form.
  if (options.emulateJSON) {
    params.contentType = 'application/x-www-form-urlencoded';
    params.data = params.data ? {model: params.data} : {};
  }

  // For older servers, emulate HTTP by mimicking the HTTP method with '_method'
  // And an 'X-HTTP-Method-Override' header.
  if (options.emulateHTTP && (type === 'PUT' || type === 'DELETE' || type === 'PATCH')) {
    params.type = 'POST';
    if (options.emulateJSON) params.data._method = type;
    var beforeSend = options.beforeSend;
    options.beforeSend = function(xhr) {
      xhr.setRequestHeader('X-HTTP-Method-Override', type);
      if (beforeSend) return beforeSend.apply(this, arguments);
    };
  }

  // Don't process data on a non-GET request.
  if (params.type !== 'GET' && !options.emulateJSON) {
    params.processData = false;
  }

  // Pass along 'textStatus' and 'errorThrown' from jQuery.
  var error = options.error;
  options.error = function(xhr, textStatus, errorThrown) {
    options.textStatus = textStatus;
    options.errorThrown = errorThrown;
    if (error) error.call(options.context, xhr, textStatus, errorThrown);
  };

  // Make the request, allowing the user to override any Ajax options.
  var xhr = options.xhr = Backbone.ajax(_.extend(params, options));
  model.trigger('request', model, xhr, options);
  return xhr;
}
```
- example usage
```shell
...
  options.success = function(resp) {
    var serverAttrs = options.parse ? model.parse(resp, options) : resp;
    if (!model.set(serverAttrs, options)) return false;
    if (success) success.call(options.context, model, resp, options);
    model.trigger('sync', model, resp, options);
  };
  wrapError(this, options);
  return this.sync('read', this, options);
},

// Set a hash of model attributes, and sync the model to the server.
// If the server returns an attributes hash that differs, the model's
// state will be 'set' again.
save: function(key, val, options) {
  // Handle both '"key", value' and '{key: value}' -style arguments.
...
```

#### <a name="apidoc.element.backbone.trigger"></a>[function <span class="apidocSignatureSpan">backbone.</span>trigger (name)](#apidoc.element.backbone.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;

  var length = Math.max(0, arguments.length - 1);
  var args = Array(length);
  for (var i = 0; i < length; i++) args[i] = arguments[i + 1];

  eventsApi(triggerApi, this._events, name, void 0, args);
  return this;
}
```
- example usage
```shell
...
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;

// Iterates over the standard 'event, callback' (as well as the fancy multiple
...
```

#### <a name="apidoc.element.backbone.unbind"></a>[function <span class="apidocSignatureSpan">backbone.</span>unbind (name, callback, context)](#apidoc.element.backbone.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.backbone.Collection"></a>[module backbone.Collection](#apidoc.module.backbone.Collection)

#### <a name="apidoc.element.backbone.Collection.Collection"></a>[function <span class="apidocSignatureSpan">backbone.</span>Collection (models, options)](#apidoc.element.backbone.Collection.Collection)
- description and source-code
```javascript
Collection = function (models, options) {
  options || (options = {});
  if (options.model) this.model = options.model;
  if (options.comparator !== void 0) this.comparator = options.comparator;
  this._reset();
  this.initialize.apply(this, arguments);
  if (models) this.reset(models, _.extend({silent: true}, options));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.extend"></a>[function <span class="apidocSignatureSpan">backbone.Collection.</span>extend (protoProps, staticProps)](#apidoc.element.backbone.Collection.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ return parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function and add the prototype properties.
  child.prototype = _.create(parent.prototype, protoProps);
  child.prototype.constructor = child;

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...

// A module that can be mixed in to *any object* in order to provide it with
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;
...
```



# <a name="apidoc.module.backbone.Collection.prototype"></a>[module backbone.Collection.prototype](#apidoc.module.backbone.Collection.prototype)

#### <a name="apidoc.element.backbone.Collection.prototype._addReference"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_addReference (model, options)](#apidoc.element.backbone.Collection.prototype._addReference)
- description and source-code
```javascript
_addReference = function (model, options) {
  this._byId[model.cid] = model;
  var id = this.modelId(model.attributes);
  if (id != null) this._byId[id] = model;
  model.on('all', this._onModelEvent, this);
}
```
- example usage
```shell
...
    models[i] = existing;

  // If this is a new, valid model, push it to the 'toAdd' list.
  } else if (add) {
    model = models[i] = this._prepareModel(model, options);
    if (model) {
      toAdd.push(model);
      this._addReference(model, options);
      modelMap[model.cid] = true;
      set.push(model);
    }
  }
}

// Remove stale models.
...
```

#### <a name="apidoc.element.backbone.Collection.prototype._isModel"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_isModel (model)](#apidoc.element.backbone.Collection.prototype._isModel)
- description and source-code
```javascript
_isModel = function (model) {
  return model instanceof Model;
}
```
- example usage
```shell
...
    if (_[method]) Class.prototype[method] = addMethod(length, method, attribute);
  });
};

// Support 'collection.sortBy('attr')' and 'collection.findWhere({id: 1})'.
var cb = function(iteratee, instance) {
  if (_.isFunction(iteratee)) return iteratee;
  if (_.isObject(iteratee) && !instance._isModel(iteratee)) return modelMatcher(iteratee);
  if (_.isString(iteratee)) return function(model) { return model.get(iteratee); };
  return iteratee;
};
var modelMatcher = function(attrs) {
  var matcher = _.matches(attrs);
  return function(model) {
    return matcher(model.attributes);
...
```

#### <a name="apidoc.element.backbone.Collection.prototype._onModelEvent"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_onModelEvent (event, model, collection, options)](#apidoc.element.backbone.Collection.prototype._onModelEvent)
- description and source-code
```javascript
_onModelEvent = function (event, model, collection, options) {
  if (model) {
    if ((event === 'add' || event === 'remove') && collection !== this) return;
    if (event === 'destroy') this.remove(model, options);
    if (event === 'change') {
      var prevId = this.modelId(model.previousAttributes());
      var id = this.modelId(model.attributes);
      if (prevId !== id) {
        if (prevId != null) delete this._byId[prevId];
        if (id != null) this._byId[id] = model;
      }
    }
  }
  this.trigger.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype._prepareModel"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_prepareModel (attrs, options)](#apidoc.element.backbone.Collection.prototype._prepareModel)
- description and source-code
```javascript
_prepareModel = function (attrs, options) {
  if (this._isModel(attrs)) {
    if (!attrs.collection) attrs.collection = this;
    return attrs;
  }
  options = options ? _.clone(options) : {};
  options.collection = this;
  var model = new this.model(attrs, options);
  if (!model.validationError) return model;
  this.trigger('invalid', this, model.validationError, options);
  return false;
}
```
- example usage
```shell
...
    modelMap[existing.cid] = true;
    set.push(existing);
  }
  models[i] = existing;

// If this is a new, valid model, push it to the 'toAdd' list.
} else if (add) {
  model = models[i] = this._prepareModel(model, options);
  if (model) {
    toAdd.push(model);
    this._addReference(model, options);
    modelMap[model.cid] = true;
    set.push(model);
  }
}
...
```

#### <a name="apidoc.element.backbone.Collection.prototype._removeModels"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_removeModels (models, options)](#apidoc.element.backbone.Collection.prototype._removeModels)
- description and source-code
```javascript
_removeModels = function (models, options) {
  var removed = [];
  for (var i = 0; i < models.length; i++) {
    var model = this.get(models[i]);
    if (!model) continue;

    var index = this.indexOf(model);
    this.models.splice(index, 1);
    this.length--;

    // Remove references before triggering 'remove' event to prevent an
    // infinite loop. #3693
    delete this._byId[model.cid];
    var id = this.modelId(model.attributes);
    if (id != null) delete this._byId[id];

    if (!options.silent) {
      options.index = index;
      model.trigger('remove', model, this, options);
    }

    removed.push(model);
    this._removeReference(model, options);
  }
  return removed;
}
```
- example usage
```shell
...
},

// Remove a model, or a list of models from the set.
remove: function(models, options) {
  options = _.extend({}, options);
  var singular = !_.isArray(models);
  models = singular ? [models] : models.slice();
  var removed = this._removeModels(models, options);
  if (!options.silent && removed.length) {
    options.changes = {added: [], merged: [], removed: removed};
    this.trigger('update', this, options);
  }
  return singular ? removed[0] : removed;
},
...
```

#### <a name="apidoc.element.backbone.Collection.prototype._removeReference"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_removeReference (model, options)](#apidoc.element.backbone.Collection.prototype._removeReference)
- description and source-code
```javascript
_removeReference = function (model, options) {
  delete this._byId[model.cid];
  var id = this.modelId(model.attributes);
  if (id != null) delete this._byId[id];
  if (this === model.collection) delete model.collection;
  model.off('all', this._onModelEvent, this);
}
```
- example usage
```shell
...
// When you have more items than you want to add or remove individually,
// you can reset the entire set with a new list of models, without firing
// any granular 'add' or 'remove' events. Fires 'reset' when finished.
// Useful for bulk operations and optimizations.
reset: function(models, options) {
  options = options ? _.clone(options) : {};
  for (var i = 0; i < this.models.length; i++) {
    this._removeReference(this.models[i], options);
  }
  options.previousModels = this.models;
  this._reset();
  models = this.add(models, _.extend({silent: true}, options));
  if (!options.silent) this.trigger('reset', this, options);
  return models;
},
...
```

#### <a name="apidoc.element.backbone.Collection.prototype._reset"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>_reset ()](#apidoc.element.backbone.Collection.prototype._reset)
- description and source-code
```javascript
_reset = function () {
  this.length = 0;
  this.models = [];
  this._byId  = {};
}
```
- example usage
```shell
...
// Create a new **Collection**, perhaps to contain a specific type of 'model'.
// If a 'comparator' is specified, the Collection will maintain
// its models in sort order, as they're added and removed.
var Collection = Backbone.Collection = function(models, options) {
  options || (options = {});
  if (options.model) this.model = options.model;
  if (options.comparator !== void 0) this.comparator = options.comparator;
  this._reset();
  this.initialize.apply(this, arguments);
  if (models) this.reset(models, _.extend({silent: true}, options));
};

// Default options for 'Collection#set'.
var setOptions = {add: true, remove: true, merge: true};
var addOptions = {add: true, remove: false};
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.add"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>add (models, options)](#apidoc.element.backbone.Collection.prototype.add)
- description and source-code
```javascript
add = function (models, options) {
  return this.set(models, _.extend({merge: false}, options, addOptions));
}
```
- example usage
```shell
...
reset: function(models, options) {
  options = options ? _.clone(options) : {};
  for (var i = 0; i < this.models.length; i++) {
    this._removeReference(this.models[i], options);
  }
  options.previousModels = this.models;
  this._reset();
  models = this.add(models, _.extend({silent: true}, options));
  if (!options.silent) this.trigger('reset', this, options);
  return models;
},

// Add a model to the end of the collection.
push: function(model, options) {
  return this.add(model, _.extend({at: this.length}, options));
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.all"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>all (iteratee, context)](#apidoc.element.backbone.Collection.prototype.all)
- description and source-code
```javascript
all = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.any"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>any (iteratee, context)](#apidoc.element.backbone.Collection.prototype.any)
- description and source-code
```javascript
any = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.at"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>at (index)](#apidoc.element.backbone.Collection.prototype.at)
- description and source-code
```javascript
at = function (index) {
  if (index < 0) index += this.length;
  return this.models[index];
}
```
- example usage
```shell
...
// Add a model to the end of the collection.
push: function(model, options) {
  return this.add(model, _.extend({at: this.length}, options));
},

// Remove a model from the end of the collection.
pop: function(options) {
  var model = this.at(this.length - 1);
  return this.remove(model, options);
},

// Add a model to the beginning of the collection.
unshift: function(model, options) {
  return this.add(model, _.extend({at: 0}, options));
},
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.bind"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>bind (name, callback, context)](#apidoc.element.backbone.Collection.prototype.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...

// Bind an event to only be triggered a single time. After the first time
// the callback is invoked, its listener will be removed. If multiple events
// are passed in using the space-separated syntax, the handler will fire
// once for each event, not once for a combination of all events.
Events.once = function(name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.chain"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>chain ()](#apidoc.element.backbone.Collection.prototype.chain)
- description and source-code
```javascript
chain = function () {
  return _[method](this[attribute]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.clone"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>clone ()](#apidoc.element.backbone.Collection.prototype.clone)
- description and source-code
```javascript
clone = function () {
  return new this.constructor(this.models, {
    model: this.model,
    comparator: this.comparator
  });
}
```
- example usage
```shell
...

// Initialize is an empty function by default. Override it with your own
// initialization logic.
initialize: function(){},

// Return a copy of the model's 'attributes' object.
toJSON: function(options) {
  return _.clone(this.attributes);
},

// Proxy 'Backbone.sync' by default -- but override this if you need
// custom syncing semantics for *this* particular model.
sync: function() {
  return Backbone.sync.apply(this, arguments);
},
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.collect"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>collect (iteratee, context)](#apidoc.element.backbone.Collection.prototype.collect)
- description and source-code
```javascript
collect = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.contains"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>contains (iteratee, context)](#apidoc.element.backbone.Collection.prototype.contains)
- description and source-code
```javascript
contains = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.countBy"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>countBy (iteratee, context)](#apidoc.element.backbone.Collection.prototype.countBy)
- description and source-code
```javascript
countBy = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.create"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>create (model, options)](#apidoc.element.backbone.Collection.prototype.create)
- description and source-code
```javascript
create = function (model, options) {
  options = options ? _.clone(options) : {};
  var wait = options.wait;
  model = this._prepareModel(model, options);
  if (!model) return false;
  if (!wait) this.add(model, options);
  var collection = this;
  var success = options.success;
  options.success = function(m, resp, callbackOpts) {
    if (wait) collection.add(m, callbackOpts);
    if (success) success.call(callbackOpts.context, m, resp, callbackOpts);
  };
  model.save(null, options);
  return model;
}
```
- example usage
```shell
...
}

// Add static properties to the constructor function, if supplied.
_.extend(child, parent, staticProps);

// Set the prototype chain to inherit from 'parent', without calling
// 'parent''s constructor function and add the prototype properties.
child.prototype = _.create(parent.prototype, protoProps);
child.prototype.constructor = child;

// Set a convenience property in case the parent's prototype is needed
// later.
child.__super__ = parent.prototype;

return child;
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.detect"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>detect (iteratee, context)](#apidoc.element.backbone.Collection.prototype.detect)
- description and source-code
```javascript
detect = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.difference"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>difference ()](#apidoc.element.backbone.Collection.prototype.difference)
- description and source-code
```javascript
difference = function () {
  var args = slice.call(arguments);
  args.unshift(this[attribute]);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.drop"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>drop (iteratee, context)](#apidoc.element.backbone.Collection.prototype.drop)
- description and source-code
```javascript
drop = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.each"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>each (iteratee, context)](#apidoc.element.backbone.Collection.prototype.each)
- description and source-code
```javascript
each = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
...
// form param named 'model'.
Backbone.emulateJSON = false;

// Proxy Backbone class methods to Underscore functions, wrapping the model's
// 'attributes' object or collection's 'models' array behind the scenes.
//
// collection.filter(function(model) { return model.get('age') > 10 });
// collection.each(this.addView);
//
// 'Function#apply' can be slow so we use the method's arg count, if we know it.
var addMethod = function(length, method, attribute) {
  switch (length) {
    case 1: return function() {
      return _[method](this[attribute]);
    };
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.every"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>every (iteratee, context)](#apidoc.element.backbone.Collection.prototype.every)
- description and source-code
```javascript
every = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.fetch"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>fetch (options)](#apidoc.element.backbone.Collection.prototype.fetch)
- description and source-code
```javascript
fetch = function (options) {
  options = _.extend({parse: true}, options);
  var success = options.success;
  var collection = this;
  options.success = function(resp) {
    var method = options.reset ? 'reset' : 'set';
    collection[method](resp, options);
    if (success) success.call(options.context, collection, resp, options);
    collection.trigger('sync', collection, resp, options);
  };
  wrapError(this, options);
  return this.sync('read', this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.filter"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>filter (iteratee, context)](#apidoc.element.backbone.Collection.prototype.filter)
- description and source-code
```javascript
filter = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
...
// 'application/x-www-form-urlencoded' instead and will send the model in a
// form param named 'model'.
Backbone.emulateJSON = false;

// Proxy Backbone class methods to Underscore functions, wrapping the model's
// 'attributes' object or collection's 'models' array behind the scenes.
//
// collection.filter(function(model) { return model.get('age') > 10 });
// collection.each(this.addView);
//
// 'Function#apply' can be slow so we use the method's arg count, if we know it.
var addMethod = function(length, method, attribute) {
  switch (length) {
    case 1: return function() {
      return _[method](this[attribute]);
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.find"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>find (iteratee, context)](#apidoc.element.backbone.Collection.prototype.find)
- description and source-code
```javascript
find = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
...

// The default 'tagName' of a View's element is '"div"'.
tagName: 'div',

// jQuery delegate for element lookup, scoped to DOM elements within the
// current view. This should be preferred to global lookups where possible.
$: function(selector) {
  return this.$el.find(selector);
},

// Initialize is an empty function by default. Override it with your own
// initialization logic.
initialize: function(){},

// **render** is the core function that your view should override, in order
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.findIndex"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>findIndex (iteratee, context)](#apidoc.element.backbone.Collection.prototype.findIndex)
- description and source-code
```javascript
findIndex = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.findLastIndex"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>findLastIndex (iteratee, context)](#apidoc.element.backbone.Collection.prototype.findLastIndex)
- description and source-code
```javascript
findLastIndex = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.findWhere"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>findWhere (attrs)](#apidoc.element.backbone.Collection.prototype.findWhere)
- description and source-code
```javascript
findWhere = function (attrs) {
  return this.where(attrs, true);
}
```
- example usage
```shell
...
};
var addUnderscoreMethods = function(Class, methods, attribute) {
  _.each(methods, function(length, method) {
    if (_[method]) Class.prototype[method] = addMethod(length, method, attribute);
  });
};

// Support 'collection.sortBy('attr')' and 'collection.findWhere({id: 1})'.
var cb = function(iteratee, instance) {
  if (_.isFunction(iteratee)) return iteratee;
  if (_.isObject(iteratee) && !instance._isModel(iteratee)) return modelMatcher(iteratee);
  if (_.isString(iteratee)) return function(model) { return model.get(iteratee); };
  return iteratee;
};
var modelMatcher = function(attrs) {
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.first"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>first (iteratee, context)](#apidoc.element.backbone.Collection.prototype.first)
- description and source-code
```javascript
first = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.foldl"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>foldl ()](#apidoc.element.backbone.Collection.prototype.foldl)
- description and source-code
```javascript
foldl = function () {
  var args = slice.call(arguments);
  args.unshift(this[attribute]);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.foldr"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>foldr ()](#apidoc.element.backbone.Collection.prototype.foldr)
- description and source-code
```javascript
foldr = function () {
  var args = slice.call(arguments);
  args.unshift(this[attribute]);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.forEach"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>forEach (iteratee, context)](#apidoc.element.backbone.Collection.prototype.forEach)
- description and source-code
```javascript
forEach = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.get"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>get (obj)](#apidoc.element.backbone.Collection.prototype.get)
- description and source-code
```javascript
get = function (obj) {
  if (obj == null) return void 0;
  return this._byId[obj] ||
    this._byId[this.modelId(obj.attributes || obj)] ||
    obj.cid && this._byId[obj.cid];
}
```
- example usage
```shell
...
// 'application/x-www-form-urlencoded' instead and will send the model in a
// form param named 'model'.
Backbone.emulateJSON = false;

// Proxy Backbone class methods to Underscore functions, wrapping the model's
// 'attributes' object or collection's 'models' array behind the scenes.
//
// collection.filter(function(model) { return model.get('age') > 10 });
// collection.each(this.addView);
//
// 'Function#apply' can be slow so we use the method's arg count, if we know it.
var addMethod = function(length, method, attribute) {
  switch (length) {
    case 1: return function() {
      return _[method](this[attribute]);
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.groupBy"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>groupBy (iteratee, context)](#apidoc.element.backbone.Collection.prototype.groupBy)
- description and source-code
```javascript
groupBy = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.has"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>has (obj)](#apidoc.element.backbone.Collection.prototype.has)
- description and source-code
```javascript
has = function (obj) {
  return this.get(obj) != null;
}
```
- example usage
```shell
...
  return this.set(attrs, _.extend({}, options, {unset: true}));
},

// Determine if the model has changed since the last '"change"' event.
// If you specify an attribute name, determine if that attribute has changed.
hasChanged: function(attr) {
  if (attr == null) return !_.isEmpty(this.changed);
  return _.has(this.changed, attr);
},

// Return an object containing all the attributes that have changed, or
// false if there are no changed attributes. Useful for determining what
// parts of a view need to be updated and/or what attributes need to be
// persisted to the server. Unset attributes will be set to undefined.
// You can also pass an attributes object to diff against the model,
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.head"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>head (iteratee, context)](#apidoc.element.backbone.Collection.prototype.head)
- description and source-code
```javascript
head = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.include"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>include (iteratee, context)](#apidoc.element.backbone.Collection.prototype.include)
- description and source-code
```javascript
include = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.includes"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>includes (iteratee, context)](#apidoc.element.backbone.Collection.prototype.includes)
- description and source-code
```javascript
includes = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.indexBy"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>indexBy (iteratee, context)](#apidoc.element.backbone.Collection.prototype.indexBy)
- description and source-code
```javascript
indexBy = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>indexOf (iteratee, context)](#apidoc.element.backbone.Collection.prototype.indexOf)
- description and source-code
```javascript
indexOf = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
...
    // Internal method called by both remove and set.
    _removeModels: function(models, options) {
      var removed = [];
      for (var i = 0; i < models.length; i++) {
var model = this.get(models[i]);
if (!model) continue;

var index = this.indexOf(model);
this.models.splice(index, 1);
this.length--;

// Remove references before triggering 'remove' event to prevent an
// infinite loop. #3693
delete this._byId[model.cid];
var id = this.modelId(model.attributes);
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.initial"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>initial (iteratee, context)](#apidoc.element.backbone.Collection.prototype.initial)
- description and source-code
```javascript
initial = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.initialize"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>initialize ()](#apidoc.element.backbone.Collection.prototype.initialize)
- description and source-code
```javascript
initialize = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.inject"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>inject ()](#apidoc.element.backbone.Collection.prototype.inject)
- description and source-code
```javascript
inject = function () {
  var args = slice.call(arguments);
  args.unshift(this[attribute]);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.invoke"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>invoke ()](#apidoc.element.backbone.Collection.prototype.invoke)
- description and source-code
```javascript
invoke = function () {
  var args = slice.call(arguments);
  args.unshift(this[attribute]);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>isEmpty ()](#apidoc.element.backbone.Collection.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  return _[method](this[attribute]);
}
```
- example usage
```shell
...
  for (var key in this.attributes) attrs[key] = void 0;
  return this.set(attrs, _.extend({}, options, {unset: true}));
},

// Determine if the model has changed since the last '"change"' event.
// If you specify an attribute name, determine if that attribute has changed.
hasChanged: function(attr) {
  if (attr == null) return !_.isEmpty(this.changed);
  return _.has(this.changed, attr);
},

// Return an object containing all the attributes that have changed, or
// false if there are no changed attributes. Useful for determining what
// parts of a view need to be updated and/or what attributes need to be
// persisted to the server. Unset attributes will be set to undefined.
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.last"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>last (iteratee, context)](#apidoc.element.backbone.Collection.prototype.last)
- description and source-code
```javascript
last = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>lastIndexOf (iteratee, context)](#apidoc.element.backbone.Collection.prototype.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.listenTo"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.Collection.prototype.listenTo)
- description and source-code
```javascript
listenTo = function (obj, name, callback) {
  if (!obj) return this;
  var id = obj._listenId || (obj._listenId = _.uniqueId('l'));
  var listeningTo = this._listeningTo || (this._listeningTo = {});
  var listening = listeningTo[id];

  // This object is not listening to any other events on 'obj' yet.
  // Setup the necessary references to track the listening callbacks.
  if (!listening) {
    var thisId = this._listenId || (this._listenId = _.uniqueId('l'));
    listening = listeningTo[id] = {obj: obj, objId: id, id: thisId, listeningTo: listeningTo, count: 0};
  }

  // Bind callbacks on obj, and keep track of them on listening.
  internalOn(obj, name, callback, this, listening);
  return this;
}
```
- example usage
```shell
...
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.listenToOnce"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.Collection.prototype.listenToOnce)
- description and source-code
```javascript
listenToOnce = function (obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.map"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>map (iteratee, context)](#apidoc.element.backbone.Collection.prototype.map)
- description and source-code
```javascript
map = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
...
// Initialize is an empty function by default. Override it with your own
// initialization logic.
initialize: function(){},

// The JSON representation of a Collection is an array of the
// models' attributes.
toJSON: function(options) {
  return this.map(function(model) { return model.toJSON(options); });
},

// Proxy 'Backbone.sync' by default.
sync: function() {
  return Backbone.sync.apply(this, arguments);
},
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.max"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>max (iteratee, context)](#apidoc.element.backbone.Collection.prototype.max)
- description and source-code
```javascript
max = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
...
// Trigger one or many events, firing all bound callbacks. Callbacks are
// passed the same arguments as 'trigger' is, apart from the event name
// (unless you're listening on '"all"', which will cause your callback to
// receive the true name of the event as the first argument).
Events.trigger = function(name) {
  if (!this._events) return this;

  var length = Math.max(0, arguments.length - 1);
  var args = Array(length);
  for (var i = 0; i < length; i++) args[i] = arguments[i + 1];

  eventsApi(triggerApi, this._events, name, void 0, args);
  return this;
};
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.min"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>min (iteratee, context)](#apidoc.element.backbone.Collection.prototype.min)
- description and source-code
```javascript
min = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
...

// Default options for 'Collection#set'.
var setOptions = {add: true, remove: true, merge: true};
var addOptions = {add: true, remove: false};

// Splices 'insert' into 'array' at index 'at'.
var splice = function(array, insert, at) {
  at = Math.min(Math.max(at, 0), array.length);
  var tail = Array(array.length - at);
  var length = insert.length;
  var i;
  for (i = 0; i < tail.length; i++) tail[i] = array[i + at];
  for (i = 0; i < length; i++) array[i + at] = insert[i];
  for (i = 0; i < tail.length; i++) array[i + length + at] = tail[i];
};
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.model"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>model (attributes, options)](#apidoc.element.backbone.Collection.prototype.model)
- description and source-code
```javascript
model = function (attributes, options) {
  var attrs = attributes || {};
  options || (options = {});
  this.cid = _.uniqueId(this.cidPrefix);
  this.attributes = {};
  if (options.collection) this.collection = options.collection;
  if (options.parse) attrs = this.parse(attrs, options) || {};
  var defaults = _.result(this, 'defaults');
  attrs = _.defaults(_.extend({}, defaults, attrs), defaults);
  this.set(attrs, options);
  this.changed = {};
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
...
_prepareModel: function(attrs, options) {
  if (this._isModel(attrs)) {
    if (!attrs.collection) attrs.collection = this;
    return attrs;
  }
  options = options ? _.clone(options) : {};
  options.collection = this;
  var model = new this.model(attrs, options);
  if (!model.validationError) return model;
  this.trigger('invalid', this, model.validationError, options);
  return false;
},

// Internal method called by both remove and set.
_removeModels: function(models, options) {
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.modelId"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>modelId (attrs)](#apidoc.element.backbone.Collection.prototype.modelId)
- description and source-code
```javascript
modelId = function (attrs) {
  return attrs[this.model.prototype.idAttribute || 'id'];
}
```
- example usage
```shell
...
},

// Get a model from the set by id, cid, model object with id or cid
// properties, or an attributes object that is transformed through modelId.
get: function(obj) {
  if (obj == null) return void 0;
  return this._byId[obj] ||
    this._byId[this.modelId(obj.attributes || obj)] ||
    obj.cid && this._byId[obj.cid];
},

// Returns 'true' if the model is in the collection.
has: function(obj) {
  return this.get(obj) != null;
},
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.off"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>off (name, callback, context)](#apidoc.element.backbone.Collection.prototype.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
...
  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
};

// The reducing API that removes a callback from the 'events' object.
var offApi = function(events, name, callback, options) {
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.on"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>on (name, callback, context)](#apidoc.element.backbone.Collection.prototype.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...
// A module that can be mixed in to *any object* in order to provide it with
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.once"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>once (name, callback, context)](#apidoc.element.backbone.Collection.prototype.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
}
```
- example usage
```shell
...
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
      offer(name, once);
      callback.apply(this, arguments);
    });
    once._callback = callback;
  }
  return map;
};
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.parse"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>parse (resp, options)](#apidoc.element.backbone.Collection.prototype.parse)
- description and source-code
```javascript
parse = function (resp, options) {
  return resp;
}
```
- example usage
```shell
...
// is automatically generated and assigned for you.
var Model = Backbone.Model = function(attributes, options) {
  var attrs = attributes || {};
  options || (options = {});
  this.cid = _.uniqueId(this.cidPrefix);
  this.attributes = {};
  if (options.collection) this.collection = options.collection;
  if (options.parse) attrs = this.parse(attrs, options) || {};
  var defaults = _.result(this, 'defaults');
  attrs = _.defaults(_.extend({}, defaults, attrs), defaults);
  this.set(attrs, options);
  this.changed = {};
  this.initialize.apply(this, arguments);
};
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.partition"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>partition (iteratee, context)](#apidoc.element.backbone.Collection.prototype.partition)
- description and source-code
```javascript
partition = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.pluck"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>pluck (attr)](#apidoc.element.backbone.Collection.prototype.pluck)
- description and source-code
```javascript
pluck = function (attr) {
  return this.map(attr + '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.pop"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>pop (options)](#apidoc.element.backbone.Collection.prototype.pop)
- description and source-code
```javascript
pop = function (options) {
  var model = this.at(this.length - 1);
  return this.remove(model, options);
}
```
- example usage
```shell
...
// Bind all defined routes to 'Backbone.history'. We have to reverse the
// order of the routes here to support behavior where the most general
// routes can be defined at the bottom of the route map.
_bindRoutes: function() {
  if (!this.routes) return;
  this.routes = _.result(this, 'routes');
  var route, routes = _.keys(this.routes);
  while ((route = routes.pop()) != null) {
    this.route(route, this.routes[route]);
  }
},

// Convert a route string into a regular expression, suitable for matching
// against the current location hash.
_routeToRegExp: function(route) {
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.push"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>push (model, options)](#apidoc.element.backbone.Collection.prototype.push)
- description and source-code
```javascript
push = function (model, options) {
  return this.add(model, _.extend({at: this.length}, options));
}
```
- example usage
```shell
...
// The reducing API that adds a callback to the 'events' object.
var onApi = function(events, name, callback, options) {
  if (callback) {
    var handlers = events[name] || (events[name] = []);
    var context = options.context, ctx = options.ctx, listening = options.listening;
    if (listening) listening.count++;

    handlers.push({callback: callback, context: context, ctx: context || ctx, listening: listening});
  }
  return events;
};

// Remove one or many callbacks. If 'context' is null, removes all
// callbacks with that function. If 'callback' is null, removes all
// callbacks for the event. If 'name' is null, removes all bound
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.reduce"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>reduce ()](#apidoc.element.backbone.Collection.prototype.reduce)
- description and source-code
```javascript
reduce = function () {
  var args = slice.call(arguments);
  args.unshift(this[attribute]);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.reduceRight"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>reduceRight ()](#apidoc.element.backbone.Collection.prototype.reduceRight)
- description and source-code
```javascript
reduceRight = function () {
  var args = slice.call(arguments);
  args.unshift(this[attribute]);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.reject"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>reject (iteratee, context)](#apidoc.element.backbone.Collection.prototype.reject)
- description and source-code
```javascript
reject = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.remove"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>remove (models, options)](#apidoc.element.backbone.Collection.prototype.remove)
- description and source-code
```javascript
remove = function (models, options) {
  options = _.extend({}, options);
  var singular = !_.isArray(models);
  models = singular ? [models] : models.slice();
  var removed = this._removeModels(models, options);
  if (!options.silent && removed.length) {
    options.changes = {added: [], merged: [], removed: removed};
    this.trigger('update', this, options);
  }
  return singular ? removed[0] : removed;
}
```
- example usage
```shell
...
push: function(model, options) {
  return this.add(model, _.extend({at: this.length}, options));
},

// Remove a model from the end of the collection.
pop: function(options) {
  var model = this.at(this.length - 1);
  return this.remove(model, options);
},

// Add a model to the beginning of the collection.
unshift: function(model, options) {
  return this.add(model, _.extend({at: 0}, options));
},
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.reset"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>reset (models, options)](#apidoc.element.backbone.Collection.prototype.reset)
- description and source-code
```javascript
reset = function (models, options) {
  options = options ? _.clone(options) : {};
  for (var i = 0; i < this.models.length; i++) {
    this._removeReference(this.models[i], options);
  }
  options.previousModels = this.models;
  this._reset();
  models = this.add(models, _.extend({silent: true}, options));
  if (!options.silent) this.trigger('reset', this, options);
  return models;
}
```
- example usage
```shell
...
// its models in sort order, as they're added and removed.
var Collection = Backbone.Collection = function(models, options) {
  options || (options = {});
  if (options.model) this.model = options.model;
  if (options.comparator !== void 0) this.comparator = options.comparator;
  this._reset();
  this.initialize.apply(this, arguments);
  if (models) this.reset(models, _.extend({silent: true}, options));
};

// Default options for 'Collection#set'.
var setOptions = {add: true, remove: true, merge: true};
var addOptions = {add: true, remove: false};

// Splices 'insert' into 'array' at index 'at'.
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.rest"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>rest (iteratee, context)](#apidoc.element.backbone.Collection.prototype.rest)
- description and source-code
```javascript
rest = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.sample"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>sample (iteratee, context)](#apidoc.element.backbone.Collection.prototype.sample)
- description and source-code
```javascript
sample = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.select"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>select (iteratee, context)](#apidoc.element.backbone.Collection.prototype.select)
- description and source-code
```javascript
select = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.set"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>set (models, options)](#apidoc.element.backbone.Collection.prototype.set)
- description and source-code
```javascript
set = function (models, options) {
  if (models == null) return;

  options = _.extend({}, setOptions, options);
  if (options.parse && !this._isModel(models)) {
    models = this.parse(models, options) || [];
  }

  var singular = !_.isArray(models);
  models = singular ? [models] : models.slice();

  var at = options.at;
  if (at != null) at = +at;
  if (at > this.length) at = this.length;
  if (at < 0) at += this.length + 1;

  var set = [];
  var toAdd = [];
  var toMerge = [];
  var toRemove = [];
  var modelMap = {};

  var add = options.add;
  var merge = options.merge;
  var remove = options.remove;

  var sort = false;
  var sortable = this.comparator && at == null && options.sort !== false;
  var sortAttr = _.isString(this.comparator) ? this.comparator : null;

  // Turn bare objects into model references, and prevent invalid models
  // from being added.
  var model, i;
  for (i = 0; i < models.length; i++) {
    model = models[i];

    // If a duplicate is found, prevent it from being added and
    // optionally merge it into the existing model.
    var existing = this.get(model);
    if (existing) {
      if (merge && model !== existing) {
        var attrs = this._isModel(model) ? model.attributes : model;
        if (options.parse) attrs = existing.parse(attrs, options);
        existing.set(attrs, options);
        toMerge.push(existing);
        if (sortable && !sort) sort = existing.hasChanged(sortAttr);
      }
      if (!modelMap[existing.cid]) {
        modelMap[existing.cid] = true;
        set.push(existing);
      }
      models[i] = existing;

    // If this is a new, valid model, push it to the 'toAdd' list.
    } else if (add) {
      model = models[i] = this._prepareModel(model, options);
      if (model) {
        toAdd.push(model);
        this._addReference(model, options);
        modelMap[model.cid] = true;
        set.push(model);
      }
    }
  }

  // Remove stale models.
  if (remove) {
    for (i = 0; i < this.length; i++) {
      model = this.models[i];
      if (!modelMap[model.cid]) toRemove.push(model);
    }
    if (toRemove.length) this._removeModels(toRemove, options);
  }

  // See if sorting is needed, update 'length' and splice in new models.
  var orderChanged = false;
  var replace = !sortable && add && remove;
  if (set.length && replace) {
    orderChanged = this.length !== set.length || _.some(this.models, function(m, index) {
      return m !== set[index];
    });
    this.models.length = 0;
    splice(this.models, set, 0);
    this.length = this.models.length;
  } else if (toAdd.length) {
    if (sortable) sort = true;
    splice(this.models, toAdd, at == null ? this.length : at);
    this.length = this.models.length;
  }

  // Silently sort the collection if appropriate.
  if (sort) this.sort({silent: true});

  // Unless silenced, it's time to fire all appropriate add/sort/update events.
  if (!options.silent) {
    for (i = 0; i < toAdd.length; i++) {
      if (at != null) options.index = at + i;
      model = toAdd[i];
      model.trigger('add', model, this, options);
    }
    if (sort || orderChanged) this.trigger('sort', this, options);
    if (toAdd.length || toRemove.length || toMerge.length) {
      options.changes = {
        added: toAdd,
        removed: toRemove,
        merged: toMerge
      };
      this.trigger('update', this, options);
    }
  }

  // Return the added (or merged) model (or models).
  return singular ? models[0] : models;
}
```
- example usage
```shell
...
  options || (options = {});
  this.cid = _.uniqueId(this.cidPrefix);
  this.attributes = {};
  if (options.collection) this.collection = options.collection;
  if (options.parse) attrs = this.parse(attrs, options) || {};
  var defaults = _.result(this, 'defaults');
  attrs = _.defaults(_.extend({}, defaults, attrs), defaults);
  this.set(attrs, options);
  this.changed = {};
  this.initialize.apply(this, arguments);
};

// Attach all inheritable methods to the Model prototype.
_.extend(Model.prototype, Events, {
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.shift"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>shift (options)](#apidoc.element.backbone.Collection.prototype.shift)
- description and source-code
```javascript
shift = function (options) {
  var model = this.at(0);
  return this.remove(model, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.shuffle"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>shuffle ()](#apidoc.element.backbone.Collection.prototype.shuffle)
- description and source-code
```javascript
shuffle = function () {
  return _[method](this[attribute]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.size"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>size ()](#apidoc.element.backbone.Collection.prototype.size)
- description and source-code
```javascript
size = function () {
  return _[method](this[attribute]);
}
```
- example usage
```shell
...
  var old = this._changing ? this._previousAttributes : this.attributes;
  var changed = {};
  for (var attr in diff) {
    var val = diff[attr];
    if (_.isEqual(old[attr], val)) continue;
    changed[attr] = val;
  }
  return _.size(changed) ? changed : false;
},

// Get the previous value of an attribute, recorded at the time the last
// '"change"' event was fired.
previous: function(attr) {
  if (attr == null || !this._previousAttributes) return null;
  return this._previousAttributes[attr];
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.slice"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>slice ()](#apidoc.element.backbone.Collection.prototype.slice)
- description and source-code
```javascript
slice = function () {
  return slice.apply(this.models, arguments);
}
```
- example usage
```shell
...
};

// Handles triggering the appropriate event callbacks.
var triggerApi = function(objEvents, name, callback, args) {
  if (objEvents) {
    var events = objEvents[name];
    var allEvents = objEvents.all;
    if (events && allEvents) allEvents = allEvents.slice();
    if (events) triggerEvents(events, args);
    if (allEvents) triggerEvents(allEvents, [name].concat(args));
  }
  return objEvents;
};

// A difficult-to-believe, but optimized internal dispatch function for
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.some"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>some (iteratee, context)](#apidoc.element.backbone.Collection.prototype.some)
- description and source-code
```javascript
some = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
...
  if (toRemove.length) this._removeModels(toRemove, options);
}

// See if sorting is needed, update 'length' and splice in new models.
var orderChanged = false;
var replace = !sortable && add && remove;
if (set.length && replace) {
  orderChanged = this.length !== set.length || _.some(this.models, function(m, index) {
    return m !== set[index];
  });
  this.models.length = 0;
  splice(this.models, set, 0);
  this.length = this.models.length;
} else if (toAdd.length) {
  if (sortable) sort = true;
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.sort"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>sort (options)](#apidoc.element.backbone.Collection.prototype.sort)
- description and source-code
```javascript
sort = function (options) {
  var comparator = this.comparator;
  if (!comparator) throw new Error('Cannot sort a set without a comparator');
  options || (options = {});

  var length = comparator.length;
  if (_.isFunction(comparator)) comparator = _.bind(comparator, this);

  // Run sort based on type of 'comparator'.
  if (length === 1 || _.isString(comparator)) {
    this.models = this.sortBy(comparator);
  } else {
    this.models.sort(comparator);
  }
  if (!options.silent) this.trigger('sort', this, options);
  return this;
}
```
- example usage
```shell
...
} else if (toAdd.length) {
  if (sortable) sort = true;
  splice(this.models, toAdd, at == null ? this.length : at);
  this.length = this.models.length;
}

// Silently sort the collection if appropriate.
if (sort) this.sort({silent: true});

// Unless silenced, it's time to fire all appropriate add/sort/update events.
if (!options.silent) {
  for (i = 0; i < toAdd.length; i++) {
    if (at != null) options.index = at + i;
    model = toAdd[i];
    model.trigger('add', model, this, options);
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.sortBy"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>sortBy (iteratee, context)](#apidoc.element.backbone.Collection.prototype.sortBy)
- description and source-code
```javascript
sortBy = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
...
};
var addUnderscoreMethods = function(Class, methods, attribute) {
  _.each(methods, function(length, method) {
    if (_[method]) Class.prototype[method] = addMethod(length, method, attribute);
  });
};

// Support 'collection.sortBy('attr')' and 'collection.findWhere({id: 1})'.
var cb = function(iteratee, instance) {
  if (_.isFunction(iteratee)) return iteratee;
  if (_.isObject(iteratee) && !instance._isModel(iteratee)) return modelMatcher(iteratee);
  if (_.isString(iteratee)) return function(model) { return model.get(iteratee); };
  return iteratee;
};
var modelMatcher = function(attrs) {
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.stopListening"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.Collection.prototype.stopListening)
- description and source-code
```javascript
stopListening = function (obj, name, callback) {
  var listeningTo = this._listeningTo;
  if (!listeningTo) return this;

  var ids = obj ? [obj._listenId] : _.keys(listeningTo);

  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
}
```
- example usage
```shell
...
    destroy: function(options) {
options = options ? _.clone(options) : {};
var model = this;
var success = options.success;
var wait = options.wait;

var destroy = function() {
  model.stopListening();
  model.trigger('destroy', model, model.collection, options);
};

options.success = function(resp) {
  if (wait) destroy();
  if (success) success.call(options.context, model, resp, options);
  if (!model.isNew()) model.trigger('sync', model, resp, options);
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.sync"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>sync ()](#apidoc.element.backbone.Collection.prototype.sync)
- description and source-code
```javascript
sync = function () {
  return Backbone.sync.apply(this, arguments);
}
```
- example usage
```shell
...
  options.success = function(resp) {
    var serverAttrs = options.parse ? model.parse(resp, options) : resp;
    if (!model.set(serverAttrs, options)) return false;
    if (success) success.call(options.context, model, resp, options);
    model.trigger('sync', model, resp, options);
  };
  wrapError(this, options);
  return this.sync('read', this, options);
},

// Set a hash of model attributes, and sync the model to the server.
// If the server returns an attributes hash that differs, the model's
// state will be 'set' again.
save: function(key, val, options) {
  // Handle both '"key", value' and '{key: value}' -style arguments.
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.tail"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>tail (iteratee, context)](#apidoc.element.backbone.Collection.prototype.tail)
- description and source-code
```javascript
tail = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.take"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>take (iteratee, context)](#apidoc.element.backbone.Collection.prototype.take)
- description and source-code
```javascript
take = function (iteratee, context) {
  return _[method](this[attribute], cb(iteratee, this), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.toArray"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>toArray ()](#apidoc.element.backbone.Collection.prototype.toArray)
- description and source-code
```javascript
toArray = function () {
  return _[method](this[attribute]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>toJSON (options)](#apidoc.element.backbone.Collection.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (options) {
  return this.map(function(model) { return model.toJSON(options); });
}
```
- example usage
```shell
...
// Initialize is an empty function by default. Override it with your own
// initialization logic.
initialize: function(){},

// The JSON representation of a Collection is an array of the
// models' attributes.
toJSON: function(options) {
  return this.map(function(model) { return model.toJSON(options); });
},

// Proxy 'Backbone.sync' by default.
sync: function() {
  return Backbone.sync.apply(this, arguments);
},
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.trigger"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>trigger (name)](#apidoc.element.backbone.Collection.prototype.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;

  var length = Math.max(0, arguments.length - 1);
  var args = Array(length);
  for (var i = 0; i < length; i++) args[i] = arguments[i + 1];

  eventsApi(triggerApi, this._events, name, void 0, args);
  return this;
}
```
- example usage
```shell
...
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;

// Iterates over the standard 'event, callback' (as well as the fancy multiple
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.unbind"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>unbind (name, callback, context)](#apidoc.element.backbone.Collection.prototype.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Collection.prototype.unshift"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>unshift (model, options)](#apidoc.element.backbone.Collection.prototype.unshift)
- description and source-code
```javascript
unshift = function (model, options) {
  return this.add(model, _.extend({at: 0}, options));
}
```
- example usage
```shell
...
      return _[method](this[attribute], cb(iteratee, this), context);
    };
    case 4: return function(iteratee, defaultVal, context) {
      return _[method](this[attribute], cb(iteratee, this), defaultVal, context);
    };
    default: return function() {
      var args = slice.call(arguments);
      args.unshift(this[attribute]);
      return _[method].apply(_, args);
    };
  }
};
var addUnderscoreMethods = function(Class, methods, attribute) {
  _.each(methods, function(length, method) {
    if (_[method]) Class.prototype[method] = addMethod(length, method, attribute);
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.where"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>where (attrs, first)](#apidoc.element.backbone.Collection.prototype.where)
- description and source-code
```javascript
where = function (attrs, first) {
  return this[first ? 'find' : 'filter'](attrs);
}
```
- example usage
```shell
...
where: function(attrs, first) {
  return this[first ? 'find' : 'filter'](attrs);
},

// Return the first model with matching attributes. Useful for simple cases
// of 'find'.
findWhere: function(attrs) {
  return this.where(attrs, true);
},

// Force the collection to re-sort itself. You don't need to call this under
// normal circumstances, as the set will maintain sort order as each item
// is added.
sort: function(options) {
  var comparator = this.comparator;
...
```

#### <a name="apidoc.element.backbone.Collection.prototype.without"></a>[function <span class="apidocSignatureSpan">backbone.Collection.prototype.</span>without ()](#apidoc.element.backbone.Collection.prototype.without)
- description and source-code
```javascript
without = function () {
  var args = slice.call(arguments);
  args.unshift(this[attribute]);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.backbone.Events"></a>[module backbone.Events](#apidoc.module.backbone.Events)

#### <a name="apidoc.element.backbone.Events.bind"></a>[function <span class="apidocSignatureSpan">backbone.Events.</span>bind (name, callback, context)](#apidoc.element.backbone.Events.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...

// Bind an event to only be triggered a single time. After the first time
// the callback is invoked, its listener will be removed. If multiple events
// are passed in using the space-separated syntax, the handler will fire
// once for each event, not once for a combination of all events.
Events.once = function(name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
...
```

#### <a name="apidoc.element.backbone.Events.listenTo"></a>[function <span class="apidocSignatureSpan">backbone.Events.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.Events.listenTo)
- description and source-code
```javascript
listenTo = function (obj, name, callback) {
  if (!obj) return this;
  var id = obj._listenId || (obj._listenId = _.uniqueId('l'));
  var listeningTo = this._listeningTo || (this._listeningTo = {});
  var listening = listeningTo[id];

  // This object is not listening to any other events on 'obj' yet.
  // Setup the necessary references to track the listening callbacks.
  if (!listening) {
    var thisId = this._listenId || (this._listenId = _.uniqueId('l'));
    listening = listeningTo[id] = {obj: obj, objId: id, id: thisId, listeningTo: listeningTo, count: 0};
  }

  // Bind callbacks on obj, and keep track of them on listening.
  internalOn(obj, name, callback, this, listening);
  return this;
}
```
- example usage
```shell
...
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
...
```

#### <a name="apidoc.element.backbone.Events.listenToOnce"></a>[function <span class="apidocSignatureSpan">backbone.Events.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.Events.listenToOnce)
- description and source-code
```javascript
listenToOnce = function (obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Events.off"></a>[function <span class="apidocSignatureSpan">backbone.Events.</span>off (name, callback, context)](#apidoc.element.backbone.Events.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
...
  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
};

// The reducing API that removes a callback from the 'events' object.
var offApi = function(events, name, callback, options) {
...
```

#### <a name="apidoc.element.backbone.Events.on"></a>[function <span class="apidocSignatureSpan">backbone.Events.</span>on (name, callback, context)](#apidoc.element.backbone.Events.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...
// A module that can be mixed in to *any object* in order to provide it with
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;
...
```

#### <a name="apidoc.element.backbone.Events.once"></a>[function <span class="apidocSignatureSpan">backbone.Events.</span>once (name, callback, context)](#apidoc.element.backbone.Events.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
}
```
- example usage
```shell
...
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
      offer(name, once);
      callback.apply(this, arguments);
    });
    once._callback = callback;
  }
  return map;
};
...
```

#### <a name="apidoc.element.backbone.Events.stopListening"></a>[function <span class="apidocSignatureSpan">backbone.Events.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.Events.stopListening)
- description and source-code
```javascript
stopListening = function (obj, name, callback) {
  var listeningTo = this._listeningTo;
  if (!listeningTo) return this;

  var ids = obj ? [obj._listenId] : _.keys(listeningTo);

  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
}
```
- example usage
```shell
...
    destroy: function(options) {
options = options ? _.clone(options) : {};
var model = this;
var success = options.success;
var wait = options.wait;

var destroy = function() {
  model.stopListening();
  model.trigger('destroy', model, model.collection, options);
};

options.success = function(resp) {
  if (wait) destroy();
  if (success) success.call(options.context, model, resp, options);
  if (!model.isNew()) model.trigger('sync', model, resp, options);
...
```

#### <a name="apidoc.element.backbone.Events.trigger"></a>[function <span class="apidocSignatureSpan">backbone.Events.</span>trigger (name)](#apidoc.element.backbone.Events.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;

  var length = Math.max(0, arguments.length - 1);
  var args = Array(length);
  for (var i = 0; i < length; i++) args[i] = arguments[i + 1];

  eventsApi(triggerApi, this._events, name, void 0, args);
  return this;
}
```
- example usage
```shell
...
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;

// Iterates over the standard 'event, callback' (as well as the fancy multiple
...
```

#### <a name="apidoc.element.backbone.Events.unbind"></a>[function <span class="apidocSignatureSpan">backbone.Events.</span>unbind (name, callback, context)](#apidoc.element.backbone.Events.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.backbone.History"></a>[module backbone.History](#apidoc.module.backbone.History)

#### <a name="apidoc.element.backbone.History.History"></a>[function <span class="apidocSignatureSpan">backbone.</span>History ()](#apidoc.element.backbone.History.History)
- description and source-code
```javascript
History = function () {
  this.handlers = [];
  this.checkUrl = _.bind(this.checkUrl, this);

  // Ensure that 'History' can be used outside of the browser.
  if (typeof window !== 'undefined') {
    this.location = window.location;
    this.history = window.history;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.History.extend"></a>[function <span class="apidocSignatureSpan">backbone.History.</span>extend (protoProps, staticProps)](#apidoc.element.backbone.History.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ return parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function and add the prototype properties.
  child.prototype = _.create(parent.prototype, protoProps);
  child.prototype.constructor = child;

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...

// A module that can be mixed in to *any object* in order to provide it with
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;
...
```



# <a name="apidoc.module.backbone.History.prototype"></a>[module backbone.History.prototype](#apidoc.module.backbone.History.prototype)

#### <a name="apidoc.element.backbone.History.prototype._updateHash"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>_updateHash (location, fragment, replace)](#apidoc.element.backbone.History.prototype._updateHash)
- description and source-code
```javascript
_updateHash = function (location, fragment, replace) {
  if (replace) {
    var href = location.href.replace(/(javascript:|#).*$/, '');
    location.replace(href + '#' + fragment);
  } else {
    // Some browsers require that 'hash' contains a leading #.
    location.hash = '#' + fragment;
  }
}
```
- example usage
```shell
...
      // If pushState is available, we use it to set the fragment as a real URL.
      if (this._usePushState) {
        this.history[options.replace ? 'replaceState' : 'pushState']({}, document.title, url);

      // If hash changes haven't been explicitly disabled, update the hash
      // fragment to store history.
      } else if (this._wantsHashChange) {
        this._updateHash(this.location, fragment, options.replace);
        if (this.iframe && fragment !== this.getHash(this.iframe.contentWindow)) {
var iWindow = this.iframe.contentWindow;

// Opening and closing the iframe tricks IE7 and earlier to push a
// history entry on hash-tag change.  When replace is true, we don't
// want this.
if (!options.replace) {
...
```

#### <a name="apidoc.element.backbone.History.prototype.atRoot"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>atRoot ()](#apidoc.element.backbone.History.prototype.atRoot)
- description and source-code
```javascript
atRoot = function () {
  var path = this.location.pathname.replace(/[^\/]$/, '$&/');
  return path === this.root && !this.getSearch();
}
```
- example usage
```shell
...

      // Transition from hashChange to pushState or vice versa if both are
      // requested.
      if (this._wantsHashChange && this._wantsPushState) {

// If we've started off with a route from a 'pushState'-enabled
// browser, but we're currently in a browser that doesn't support it...
if (!this._hasPushState && !this.atRoot()) {
  var rootPath = this.root.slice(0, -1) || '/';
  this.location.replace(rootPath + '#' + this.getPath());
  // Return immediately as browser will do redirect to new url
  return true;

// Or if we've started out with a hash-based route, but we're currently
// in a browser where it could be 'pushState'-based instead...
...
```

#### <a name="apidoc.element.backbone.History.prototype.bind"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>bind (name, callback, context)](#apidoc.element.backbone.History.prototype.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...

// Bind an event to only be triggered a single time. After the first time
// the callback is invoked, its listener will be removed. If multiple events
// are passed in using the space-separated syntax, the handler will fire
// once for each event, not once for a combination of all events.
Events.once = function(name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
...
```

#### <a name="apidoc.element.backbone.History.prototype.checkUrl"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>checkUrl (e)](#apidoc.element.backbone.History.prototype.checkUrl)
- description and source-code
```javascript
checkUrl = function (e) {
  var current = this.getFragment();

  // If the user pressed the back button, the iframe's hash will have
  // changed and we should use that for comparison.
  if (current === this.fragment && this.iframe) {
    current = this.getHash(this.iframe.contentWindow);
  }

  if (current === this.fragment) return false;
  if (this.iframe) this.navigate(current);
  this.loadUrl();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.History.prototype.decodeFragment"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>decodeFragment (fragment)](#apidoc.element.backbone.History.prototype.decodeFragment)
- description and source-code
```javascript
decodeFragment = function (fragment) {
  return decodeURI(fragment.replace(/%25/g, '%2525'));
}
```
- example usage
```shell
...
atRoot: function() {
  var path = this.location.pathname.replace(/[^\/]$/, '$&/');
  return path === this.root && !this.getSearch();
},

// Does the pathname match the root?
matchRoot: function() {
  var path = this.decodeFragment(this.location.pathname);
  var rootPath = path.slice(0, this.root.length - 1) + '/';
  return rootPath === this.root;
},

// Unicode characters in 'location.pathname' are percent encoded so they're
// decoded for comparison. '%25' should not be decoded since it may be part
// of an encoded parameter.
...
```

#### <a name="apidoc.element.backbone.History.prototype.getFragment"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>getFragment (fragment)](#apidoc.element.backbone.History.prototype.getFragment)
- description and source-code
```javascript
getFragment = function (fragment) {
  if (fragment == null) {
    if (this._usePushState || !this._wantsHashChange) {
      fragment = this.getPath();
    } else {
      fragment = this.getHash();
    }
  }
  return fragment.replace(routeStripper, '');
}
```
- example usage
```shell
...
this.root             = this.options.root;
this._wantsHashChange = this.options.hashChange !== false;
this._hasHashChange   = 'onhashchange' in window && (document.documentMode === void 0 || document.documentMode > 7);
this._useHashChange   = this._wantsHashChange && this._hasHashChange;
this._wantsPushState  = !!this.options.pushState;
this._hasPushState    = !!(this.history && this.history.pushState);
this._usePushState    = this._wantsPushState && this._hasPushState;
this.fragment         = this.getFragment();

// Normalize root to always include a leading and trailing slash.
this.root = ('/' + this.root + '/').replace(rootStripper, '/');

// Transition from hashChange to pushState or vice versa if both are
// requested.
if (this._wantsHashChange && this._wantsPushState) {
...
```

#### <a name="apidoc.element.backbone.History.prototype.getHash"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>getHash (window)](#apidoc.element.backbone.History.prototype.getHash)
- description and source-code
```javascript
getHash = function (window) {
  var match = (window || this).location.href.match(/#(.*)$/);
  return match ? match[1] : '';
}
```
- example usage
```shell
...

// Get the cross-browser normalized URL fragment from the path or hash.
getFragment: function(fragment) {
  if (fragment == null) {
    if (this._usePushState || !this._wantsHashChange) {
      fragment = this.getPath();
    } else {
      fragment = this.getHash();
    }
  }
  return fragment.replace(routeStripper, '');
},

// Start the hash change handling, returning 'true' if the current URL matches
// an existing route, and 'false' otherwise.
...
```

#### <a name="apidoc.element.backbone.History.prototype.getPath"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>getPath ()](#apidoc.element.backbone.History.prototype.getPath)
- description and source-code
```javascript
getPath = function () {
  var path = this.decodeFragment(
    this.location.pathname + this.getSearch()
  ).slice(this.root.length - 1);
  return path.charAt(0) === '/' ? path.slice(1) : path;
}
```
- example usage
```shell
...
  return path.charAt(0) === '/' ? path.slice(1) : path;
},

// Get the cross-browser normalized URL fragment from the path or hash.
getFragment: function(fragment) {
  if (fragment == null) {
    if (this._usePushState || !this._wantsHashChange) {
      fragment = this.getPath();
    } else {
      fragment = this.getHash();
    }
  }
  return fragment.replace(routeStripper, '');
},
...
```

#### <a name="apidoc.element.backbone.History.prototype.getSearch"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>getSearch ()](#apidoc.element.backbone.History.prototype.getSearch)
- description and source-code
```javascript
getSearch = function () {
  var match = this.location.href.replace(/#.*/, '').match(/\?.+/);
  return match ? match[0] : '';
}
```
- example usage
```shell
...
// The default interval to poll for hash changes, if necessary, is
// twenty times a second.
interval: 50,

// Are we at the app root?
atRoot: function() {
  var path = this.location.pathname.replace(/[^\/]$/, '$&/');
  return path === this.root && !this.getSearch();
},

// Does the pathname match the root?
matchRoot: function() {
  var path = this.decodeFragment(this.location.pathname);
  var rootPath = path.slice(0, this.root.length - 1) + '/';
  return rootPath === this.root;
...
```

#### <a name="apidoc.element.backbone.History.prototype.listenTo"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.History.prototype.listenTo)
- description and source-code
```javascript
listenTo = function (obj, name, callback) {
  if (!obj) return this;
  var id = obj._listenId || (obj._listenId = _.uniqueId('l'));
  var listeningTo = this._listeningTo || (this._listeningTo = {});
  var listening = listeningTo[id];

  // This object is not listening to any other events on 'obj' yet.
  // Setup the necessary references to track the listening callbacks.
  if (!listening) {
    var thisId = this._listenId || (this._listenId = _.uniqueId('l'));
    listening = listeningTo[id] = {obj: obj, objId: id, id: thisId, listeningTo: listeningTo, count: 0};
  }

  // Bind callbacks on obj, and keep track of them on listening.
  internalOn(obj, name, callback, this, listening);
  return this;
}
```
- example usage
```shell
...
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
...
```

#### <a name="apidoc.element.backbone.History.prototype.listenToOnce"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.History.prototype.listenToOnce)
- description and source-code
```javascript
listenToOnce = function (obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.History.prototype.loadUrl"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>loadUrl (fragment)](#apidoc.element.backbone.History.prototype.loadUrl)
- description and source-code
```javascript
loadUrl = function (fragment) {
  // If the root doesn't match, no routes can match either.
  if (!this.matchRoot()) return false;
  fragment = this.fragment = this.getFragment(fragment);
  return _.some(this.handlers, function(handler) {
    if (handler.route.test(fragment)) {
      handler.callback(fragment);
      return true;
    }
  });
}
```
- example usage
```shell
...
    addEventListener('popstate', this.checkUrl, false);
  } else if (this._useHashChange && !this.iframe) {
    addEventListener('hashchange', this.checkUrl, false);
  } else if (this._wantsHashChange) {
    this._checkUrlInterval = setInterval(this.checkUrl, this.interval);
  }

  if (!this.options.silent) return this.loadUrl();
},

// Disable Backbone.history, perhaps temporarily. Not useful in a real app,
// but possibly useful for unit testing Routers.
stop: function() {
  // Add a cross-platform 'removeEventListener' shim for older browsers.
  var removeEventListener = window.removeEventListener || function(eventName, listener) {
...
```

#### <a name="apidoc.element.backbone.History.prototype.matchRoot"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>matchRoot ()](#apidoc.element.backbone.History.prototype.matchRoot)
- description and source-code
```javascript
matchRoot = function () {
  var path = this.decodeFragment(this.location.pathname);
  var rootPath = path.slice(0, this.root.length - 1) + '/';
  return rootPath === this.root;
}
```
- example usage
```shell
...
},

// Attempt to load the current URL fragment. If a route succeeds with a
// match, returns 'true'. If no defined routes matches the fragment,
// returns 'false'.
loadUrl: function(fragment) {
  // If the root doesn't match, no routes can match either.
  if (!this.matchRoot()) return false;
  fragment = this.fragment = this.getFragment(fragment);
  return _.some(this.handlers, function(handler) {
    if (handler.route.test(fragment)) {
      handler.callback(fragment);
      return true;
    }
  });
...
```

#### <a name="apidoc.element.backbone.History.prototype.navigate"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>navigate (fragment, options)](#apidoc.element.backbone.History.prototype.navigate)
- description and source-code
```javascript
navigate = function (fragment, options) {
  if (!History.started) return false;
  if (!options || options === true) options = {trigger: !!options};

  // Normalize the fragment.
  fragment = this.getFragment(fragment || '');

  // Don't include a trailing slash on the root.
  var rootPath = this.root;
  if (fragment === '' || fragment.charAt(0) === '?') {
    rootPath = rootPath.slice(0, -1) || '/';
  }
  var url = rootPath + fragment;

  // Strip the hash and decode for matching.
  fragment = this.decodeFragment(fragment.replace(pathStripper, ''));

  if (this.fragment === fragment) return;
  this.fragment = fragment;

  // If pushState is available, we use it to set the fragment as a real URL.
  if (this._usePushState) {
    this.history[options.replace ? 'replaceState' : 'pushState']({}, document.title, url);

  // If hash changes haven't been explicitly disabled, update the hash
  // fragment to store history.
  } else if (this._wantsHashChange) {
    this._updateHash(this.location, fragment, options.replace);
    if (this.iframe && fragment !== this.getHash(this.iframe.contentWindow)) {
      var iWindow = this.iframe.contentWindow;

      // Opening and closing the iframe tricks IE7 and earlier to push a
      // history entry on hash-tag change.  When replace is true, we don't
      // want this.
      if (!options.replace) {
        iWindow.document.open();
        iWindow.document.close();
      }

      this._updateHash(iWindow.location, fragment, options.replace);
    }

  // If you've told us that you explicitly don't want fallback hashchange-
  // based history, then 'navigate' becomes a page refresh.
  } else {
    return this.location.assign(url);
  }
  if (options.trigger) return this.loadUrl(fragment);
}
```
- example usage
```shell
...
// excellent place to do pre-route setup or post-route cleanup.
execute: function(callback, args, name) {
  if (callback) callback.apply(this, args);
},

// Simple proxy to 'Backbone.history' to save a fragment into the history.
navigate: function(fragment, options) {
  Backbone.history.navigate(fragment, options);
  return this;
},

// Bind all defined routes to 'Backbone.history'. We have to reverse the
// order of the routes here to support behavior where the most general
// routes can be defined at the bottom of the route map.
_bindRoutes: function() {
...
```

#### <a name="apidoc.element.backbone.History.prototype.off"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>off (name, callback, context)](#apidoc.element.backbone.History.prototype.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
...
  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
};

// The reducing API that removes a callback from the 'events' object.
var offApi = function(events, name, callback, options) {
...
```

#### <a name="apidoc.element.backbone.History.prototype.on"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>on (name, callback, context)](#apidoc.element.backbone.History.prototype.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...
// A module that can be mixed in to *any object* in order to provide it with
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;
...
```

#### <a name="apidoc.element.backbone.History.prototype.once"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>once (name, callback, context)](#apidoc.element.backbone.History.prototype.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
}
```
- example usage
```shell
...
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
      offer(name, once);
      callback.apply(this, arguments);
    });
    once._callback = callback;
  }
  return map;
};
...
```

#### <a name="apidoc.element.backbone.History.prototype.route"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>route (route, callback)](#apidoc.element.backbone.History.prototype.route)
- description and source-code
```javascript
route = function (route, callback) {
  this.handlers.unshift({route: route, callback: callback});
}
```
- example usage
```shell
...

// Initialize is an empty function by default. Override it with your own
// initialization logic.
initialize: function(){},

// Manually bind a single named route to a callback. For example:
//
//     this.route('search/:query/p:num', 'search', function(query, num) {
//       ...
//     });
//
route: function(route, name, callback) {
  if (!_.isRegExp(route)) route = this._routeToRegExp(route);
  if (_.isFunction(name)) {
    callback = name;
...
```

#### <a name="apidoc.element.backbone.History.prototype.start"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>start (options)](#apidoc.element.backbone.History.prototype.start)
- description and source-code
```javascript
start = function (options) {
  if (History.started) throw new Error('Backbone.history has already been started');
  History.started = true;

  // Figure out the initial configuration. Do we need an iframe?
  // Is pushState desired ... is it available?
  this.options          = _.extend({root: '/'}, this.options, options);
  this.root             = this.options.root;
  this._wantsHashChange = this.options.hashChange !== false;
  this._hasHashChange   = 'onhashchange' in window && (document.documentMode === void 0 || document.documentMode > 7);
  this._useHashChange   = this._wantsHashChange && this._hasHashChange;
  this._wantsPushState  = !!this.options.pushState;
  this._hasPushState    = !!(this.history && this.history.pushState);
  this._usePushState    = this._wantsPushState && this._hasPushState;
  this.fragment         = this.getFragment();

  // Normalize root to always include a leading and trailing slash.
  this.root = ('/' + this.root + '/').replace(rootStripper, '/');

  // Transition from hashChange to pushState or vice versa if both are
  // requested.
  if (this._wantsHashChange && this._wantsPushState) {

    // If we've started off with a route from a 'pushState'-enabled
    // browser, but we're currently in a browser that doesn't support it...
    if (!this._hasPushState && !this.atRoot()) {
      var rootPath = this.root.slice(0, -1) || '/';
      this.location.replace(rootPath + '#' + this.getPath());
      // Return immediately as browser will do redirect to new url
      return true;

    // Or if we've started out with a hash-based route, but we're currently
    // in a browser where it could be 'pushState'-based instead...
    } else if (this._hasPushState && this.atRoot()) {
      this.navigate(this.getHash(), {replace: true});
    }

  }

  // Proxy an iframe to handle location events if the browser doesn't
  // support the 'hashchange' event, HTML5 history, or the user wants
  // 'hashChange' but not 'pushState'.
  if (!this._hasHashChange && this._wantsHashChange && !this._usePushState) {
    this.iframe = document.createElement('iframe');
    this.iframe.src = 'javascript:0';
    this.iframe.style.display = 'none';
    this.iframe.tabIndex = -1;
    var body = document.body;
    // Using 'appendChild' will throw on IE < 9 if the document is not ready.
    var iWindow = body.insertBefore(this.iframe, body.firstChild).contentWindow;
    iWindow.document.open();
    iWindow.document.close();
    iWindow.location.hash = '#' + this.fragment;
  }

  // Add a cross-platform 'addEventListener' shim for older browsers.
  var addEventListener = window.addEventListener || function(eventName, listener) {
    return attachEvent('on' + eventName, listener);
  };

  // Depending on whether we're using pushState or hashes, and whether
  // 'onhashchange' is supported, determine how we check the URL state.
  if (this._usePushState) {
    addEventListener('popstate', this.checkUrl, false);
  } else if (this._useHashChange && !this.iframe) {
    addEventListener('hashchange', this.checkUrl, false);
  } else if (this._wantsHashChange) {
    this._checkUrlInterval = setInterval(this.checkUrl, this.interval);
  }

  if (!this.options.silent) return this.loadUrl();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.History.prototype.stop"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>stop ()](#apidoc.element.backbone.History.prototype.stop)
- description and source-code
```javascript
stop = function () {
  // Add a cross-platform 'removeEventListener' shim for older browsers.
  var removeEventListener = window.removeEventListener || function(eventName, listener) {
    return detachEvent('on' + eventName, listener);
  };

  // Remove window listeners.
  if (this._usePushState) {
    removeEventListener('popstate', this.checkUrl, false);
  } else if (this._useHashChange && !this.iframe) {
    removeEventListener('hashchange', this.checkUrl, false);
  }

  // Clean up the iframe if necessary.
  if (this.iframe) {
    document.body.removeChild(this.iframe);
    this.iframe = null;
  }

  // Some environments will throw when clearing an undefined interval.
  if (this._checkUrlInterval) clearInterval(this._checkUrlInterval);
  History.started = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.History.prototype.stopListening"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.History.prototype.stopListening)
- description and source-code
```javascript
stopListening = function (obj, name, callback) {
  var listeningTo = this._listeningTo;
  if (!listeningTo) return this;

  var ids = obj ? [obj._listenId] : _.keys(listeningTo);

  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
}
```
- example usage
```shell
...
    destroy: function(options) {
options = options ? _.clone(options) : {};
var model = this;
var success = options.success;
var wait = options.wait;

var destroy = function() {
  model.stopListening();
  model.trigger('destroy', model, model.collection, options);
};

options.success = function(resp) {
  if (wait) destroy();
  if (success) success.call(options.context, model, resp, options);
  if (!model.isNew()) model.trigger('sync', model, resp, options);
...
```

#### <a name="apidoc.element.backbone.History.prototype.trigger"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>trigger (name)](#apidoc.element.backbone.History.prototype.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;

  var length = Math.max(0, arguments.length - 1);
  var args = Array(length);
  for (var i = 0; i < length; i++) args[i] = arguments[i + 1];

  eventsApi(triggerApi, this._events, name, void 0, args);
  return this;
}
```
- example usage
```shell
...
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;

// Iterates over the standard 'event, callback' (as well as the fancy multiple
...
```

#### <a name="apidoc.element.backbone.History.prototype.unbind"></a>[function <span class="apidocSignatureSpan">backbone.History.prototype.</span>unbind (name, callback, context)](#apidoc.element.backbone.History.prototype.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.backbone.Model"></a>[module backbone.Model](#apidoc.module.backbone.Model)

#### <a name="apidoc.element.backbone.Model.Model"></a>[function <span class="apidocSignatureSpan">backbone.</span>Model (attributes, options)](#apidoc.element.backbone.Model.Model)
- description and source-code
```javascript
Model = function (attributes, options) {
  var attrs = attributes || {};
  options || (options = {});
  this.cid = _.uniqueId(this.cidPrefix);
  this.attributes = {};
  if (options.collection) this.collection = options.collection;
  if (options.parse) attrs = this.parse(attrs, options) || {};
  var defaults = _.result(this, 'defaults');
  attrs = _.defaults(_.extend({}, defaults, attrs), defaults);
  this.set(attrs, options);
  this.changed = {};
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.extend"></a>[function <span class="apidocSignatureSpan">backbone.Model.</span>extend (protoProps, staticProps)](#apidoc.element.backbone.Model.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ return parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function and add the prototype properties.
  child.prototype = _.create(parent.prototype, protoProps);
  child.prototype.constructor = child;

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...

// A module that can be mixed in to *any object* in order to provide it with
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;
...
```



# <a name="apidoc.module.backbone.Model.prototype"></a>[module backbone.Model.prototype](#apidoc.module.backbone.Model.prototype)

#### <a name="apidoc.element.backbone.Model.prototype._validate"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>_validate (attrs, options)](#apidoc.element.backbone.Model.prototype._validate)
- description and source-code
```javascript
_validate = function (attrs, options) {
  if (!options.validate || !this.validate) return true;
  attrs = _.extend({}, this.attributes, attrs);
  var error = this.validationError = this.validate(attrs, options) || null;
  if (!error) return true;
  this.trigger('invalid', this, error, _.extend(options, {validationError: error}));
  return false;
}
```
- example usage
```shell
...
} else {
  (attrs = {})[key] = val;
}

options || (options = {});

// Run validation.
if (!this._validate(attrs, options)) return false;

// Extract attributes and options.
var unset      = options.unset;
var silent     = options.silent;
var changes    = [];
var changing   = this._changing;
this._changing = true;
...
```

#### <a name="apidoc.element.backbone.Model.prototype.bind"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>bind (name, callback, context)](#apidoc.element.backbone.Model.prototype.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...

// Bind an event to only be triggered a single time. After the first time
// the callback is invoked, its listener will be removed. If multiple events
// are passed in using the space-separated syntax, the handler will fire
// once for each event, not once for a combination of all events.
Events.once = function(name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
...
```

#### <a name="apidoc.element.backbone.Model.prototype.chain"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>chain ()](#apidoc.element.backbone.Model.prototype.chain)
- description and source-code
```javascript
chain = function () {
  return _[method](this[attribute]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.changedAttributes"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>changedAttributes (diff)](#apidoc.element.backbone.Model.prototype.changedAttributes)
- description and source-code
```javascript
changedAttributes = function (diff) {
  if (!diff) return this.hasChanged() ? _.clone(this.changed) : false;
  var old = this._changing ? this._previousAttributes : this.attributes;
  var changed = {};
  for (var attr in diff) {
    var val = diff[attr];
    if (_.isEqual(old[attr], val)) continue;
    changed[attr] = val;
  }
  return _.size(changed) ? changed : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.clear"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>clear (options)](#apidoc.element.backbone.Model.prototype.clear)
- description and source-code
```javascript
clear = function (options) {
  var attrs = {};
  for (var key in this.attributes) attrs[key] = void 0;
  return this.set(attrs, _.extend({}, options, {unset: true}));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.clone"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>clone ()](#apidoc.element.backbone.Model.prototype.clone)
- description and source-code
```javascript
clone = function () {
  return new this.constructor(this.attributes);
}
```
- example usage
```shell
...

// Initialize is an empty function by default. Override it with your own
// initialization logic.
initialize: function(){},

// Return a copy of the model's 'attributes' object.
toJSON: function(options) {
  return _.clone(this.attributes);
},

// Proxy 'Backbone.sync' by default -- but override this if you need
// custom syncing semantics for *this* particular model.
sync: function() {
  return Backbone.sync.apply(this, arguments);
},
...
```

#### <a name="apidoc.element.backbone.Model.prototype.destroy"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>destroy (options)](#apidoc.element.backbone.Model.prototype.destroy)
- description and source-code
```javascript
destroy = function (options) {
  options = options ? _.clone(options) : {};
  var model = this;
  var success = options.success;
  var wait = options.wait;

  var destroy = function() {
    model.stopListening();
    model.trigger('destroy', model, model.collection, options);
  };

  options.success = function(resp) {
    if (wait) destroy();
    if (success) success.call(options.context, model, resp, options);
    if (!model.isNew()) model.trigger('sync', model, resp, options);
  };

  var xhr = false;
  if (this.isNew()) {
    _.defer(options.success);
  } else {
    wrapError(this, options);
    xhr = this.sync('delete', this, options);
  }
  if (!wait) destroy();
  return xhr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.escape"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>escape (attr)](#apidoc.element.backbone.Model.prototype.escape)
- description and source-code
```javascript
escape = function (attr) {
  return _.escape(this.get(attr));
}
```
- example usage
```shell
...
// Get the value of an attribute.
get: function(attr) {
  return this.attributes[attr];
},

// Get the HTML-escaped value of an attribute.
escape: function(attr) {
  return _.escape(this.get(attr));
},

// Returns 'true' if the attribute contains a value that is not null
// or undefined.
has: function(attr) {
  return this.get(attr) != null;
},
...
```

#### <a name="apidoc.element.backbone.Model.prototype.fetch"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>fetch (options)](#apidoc.element.backbone.Model.prototype.fetch)
- description and source-code
```javascript
fetch = function (options) {
  options = _.extend({parse: true}, options);
  var model = this;
  var success = options.success;
  options.success = function(resp) {
    var serverAttrs = options.parse ? model.parse(resp, options) : resp;
    if (!model.set(serverAttrs, options)) return false;
    if (success) success.call(options.context, model, resp, options);
    model.trigger('sync', model, resp, options);
  };
  wrapError(this, options);
  return this.sync('read', this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.get"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>get (attr)](#apidoc.element.backbone.Model.prototype.get)
- description and source-code
```javascript
get = function (attr) {
  return this.attributes[attr];
}
```
- example usage
```shell
...
// 'application/x-www-form-urlencoded' instead and will send the model in a
// form param named 'model'.
Backbone.emulateJSON = false;

// Proxy Backbone class methods to Underscore functions, wrapping the model's
// 'attributes' object or collection's 'models' array behind the scenes.
//
// collection.filter(function(model) { return model.get('age') > 10 });
// collection.each(this.addView);
//
// 'Function#apply' can be slow so we use the method's arg count, if we know it.
var addMethod = function(length, method, attribute) {
  switch (length) {
    case 1: return function() {
      return _[method](this[attribute]);
...
```

#### <a name="apidoc.element.backbone.Model.prototype.has"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>has (attr)](#apidoc.element.backbone.Model.prototype.has)
- description and source-code
```javascript
has = function (attr) {
  return this.get(attr) != null;
}
```
- example usage
```shell
...
  return this.set(attrs, _.extend({}, options, {unset: true}));
},

// Determine if the model has changed since the last '"change"' event.
// If you specify an attribute name, determine if that attribute has changed.
hasChanged: function(attr) {
  if (attr == null) return !_.isEmpty(this.changed);
  return _.has(this.changed, attr);
},

// Return an object containing all the attributes that have changed, or
// false if there are no changed attributes. Useful for determining what
// parts of a view need to be updated and/or what attributes need to be
// persisted to the server. Unset attributes will be set to undefined.
// You can also pass an attributes object to diff against the model,
...
```

#### <a name="apidoc.element.backbone.Model.prototype.hasChanged"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>hasChanged (attr)](#apidoc.element.backbone.Model.prototype.hasChanged)
- description and source-code
```javascript
hasChanged = function (attr) {
  if (attr == null) return !_.isEmpty(this.changed);
  return _.has(this.changed, attr);
}
```
- example usage
```shell
...
// Return an object containing all the attributes that have changed, or
// false if there are no changed attributes. Useful for determining what
// parts of a view need to be updated and/or what attributes need to be
// persisted to the server. Unset attributes will be set to undefined.
// You can also pass an attributes object to diff against the model,
// determining if there *would be* a change.
changedAttributes: function(diff) {
  if (!diff) return this.hasChanged() ? _.clone(this.changed) : false;
  var old = this._changing ? this._previousAttributes : this.attributes;
  var changed = {};
  for (var attr in diff) {
    var val = diff[attr];
    if (_.isEqual(old[attr], val)) continue;
    changed[attr] = val;
  }
...
```

#### <a name="apidoc.element.backbone.Model.prototype.initialize"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>initialize ()](#apidoc.element.backbone.Model.prototype.initialize)
- description and source-code
```javascript
initialize = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.invert"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>invert ()](#apidoc.element.backbone.Model.prototype.invert)
- description and source-code
```javascript
invert = function () {
  return _[method](this[attribute]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>isEmpty ()](#apidoc.element.backbone.Model.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  return _[method](this[attribute]);
}
```
- example usage
```shell
...
  for (var key in this.attributes) attrs[key] = void 0;
  return this.set(attrs, _.extend({}, options, {unset: true}));
},

// Determine if the model has changed since the last '"change"' event.
// If you specify an attribute name, determine if that attribute has changed.
hasChanged: function(attr) {
  if (attr == null) return !_.isEmpty(this.changed);
  return _.has(this.changed, attr);
},

// Return an object containing all the attributes that have changed, or
// false if there are no changed attributes. Useful for determining what
// parts of a view need to be updated and/or what attributes need to be
// persisted to the server. Unset attributes will be set to undefined.
...
```

#### <a name="apidoc.element.backbone.Model.prototype.isNew"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>isNew ()](#apidoc.element.backbone.Model.prototype.isNew)
- description and source-code
```javascript
isNew = function () {
  return !this.has(this.idAttribute);
}
```
- example usage
```shell
...
  model.trigger('sync', model, resp, options);
};
wrapError(this, options);

// Set temporary attributes if '{wait: true}' to properly find new ids.
if (attrs && wait) this.attributes = _.extend({}, attributes, attrs);

var method = this.isNew() ? 'create' : (options.patch ? 'patch' : 'update');
if (method === 'patch' && !options.attrs) options.attrs = attrs;
var xhr = this.sync(method, this, options);

// Restore attributes.
this.attributes = attributes;

return xhr;
...
```

#### <a name="apidoc.element.backbone.Model.prototype.isValid"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>isValid (options)](#apidoc.element.backbone.Model.prototype.isValid)
- description and source-code
```javascript
isValid = function (options) {
  return this._validate({}, _.extend({}, options, {validate: true}));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.keys"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>keys ()](#apidoc.element.backbone.Model.prototype.keys)
- description and source-code
```javascript
keys = function () {
  return _[method](this[attribute]);
}
```
- example usage
```shell
...
// space-separated events '"change blur", callback' and jQuery-style event
// maps '{event: callback}').
var eventsApi = function(iteratee, events, name, callback, opts) {
  var i = 0, names;
  if (name && typeof name === 'object') {
    // Handle event maps.
    if (callback !== void 0 && 'context' in opts && opts.context === void 0) opts.context = callback;
    for (names = _.keys(name); i < names.length ; i++) {
      events = eventsApi(iteratee, events, names[i], name[names[i]], opts);
    }
  } else if (name && eventSplitter.test(name)) {
    // Handle space-separated event names by delegating them individually.
    for (names = name.split(eventSplitter); i < names.length; i++) {
      events = iteratee(events, names[i], callback, opts);
    }
...
```

#### <a name="apidoc.element.backbone.Model.prototype.listenTo"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.Model.prototype.listenTo)
- description and source-code
```javascript
listenTo = function (obj, name, callback) {
  if (!obj) return this;
  var id = obj._listenId || (obj._listenId = _.uniqueId('l'));
  var listeningTo = this._listeningTo || (this._listeningTo = {});
  var listening = listeningTo[id];

  // This object is not listening to any other events on 'obj' yet.
  // Setup the necessary references to track the listening callbacks.
  if (!listening) {
    var thisId = this._listenId || (this._listenId = _.uniqueId('l'));
    listening = listeningTo[id] = {obj: obj, objId: id, id: thisId, listeningTo: listeningTo, count: 0};
  }

  // Bind callbacks on obj, and keep track of them on listening.
  internalOn(obj, name, callback, this, listening);
  return this;
}
```
- example usage
```shell
...
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
...
```

#### <a name="apidoc.element.backbone.Model.prototype.listenToOnce"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.Model.prototype.listenToOnce)
- description and source-code
```javascript
listenToOnce = function (obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.matches"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>matches (attrs)](#apidoc.element.backbone.Model.prototype.matches)
- description and source-code
```javascript
matches = function (attrs) {
  return !!_.iteratee(attrs, this)(this.attributes);
}
```
- example usage
```shell
...
var cb = function(iteratee, instance) {
  if (_.isFunction(iteratee)) return iteratee;
  if (_.isObject(iteratee) && !instance._isModel(iteratee)) return modelMatcher(iteratee);
  if (_.isString(iteratee)) return function(model) { return model.get(iteratee); };
  return iteratee;
};
var modelMatcher = function(attrs) {
  var matcher = _.matches(attrs);
  return function(model) {
    return matcher(model.attributes);
  };
};

// Backbone.Events
// ---------------
...
```

#### <a name="apidoc.element.backbone.Model.prototype.off"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>off (name, callback, context)](#apidoc.element.backbone.Model.prototype.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
...
  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
};

// The reducing API that removes a callback from the 'events' object.
var offApi = function(events, name, callback, options) {
...
```

#### <a name="apidoc.element.backbone.Model.prototype.omit"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>omit ()](#apidoc.element.backbone.Model.prototype.omit)
- description and source-code
```javascript
omit = function () {
  var args = slice.call(arguments);
  args.unshift(this[attribute]);
  return _[method].apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.on"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>on (name, callback, context)](#apidoc.element.backbone.Model.prototype.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...
// A module that can be mixed in to *any object* in order to provide it with
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;
...
```

#### <a name="apidoc.element.backbone.Model.prototype.once"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>once (name, callback, context)](#apidoc.element.backbone.Model.prototype.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
}
```
- example usage
```shell
...
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
      offer(name, once);
      callback.apply(this, arguments);
    });
    once._callback = callback;
  }
  return map;
};
...
```

#### <a name="apidoc.element.backbone.Model.prototype.pairs"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>pairs ()](#apidoc.element.backbone.Model.prototype.pairs)
- description and source-code
```javascript
pairs = function () {
  return _[method](this[attribute]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.parse"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>parse (resp, options)](#apidoc.element.backbone.Model.prototype.parse)
- description and source-code
```javascript
parse = function (resp, options) {
  return resp;
}
```
- example usage
```shell
...
// is automatically generated and assigned for you.
var Model = Backbone.Model = function(attributes, options) {
  var attrs = attributes || {};
  options || (options = {});
  this.cid = _.uniqueId(this.cidPrefix);
  this.attributes = {};
  if (options.collection) this.collection = options.collection;
  if (options.parse) attrs = this.parse(attrs, options) || {};
  var defaults = _.result(this, 'defaults');
  attrs = _.defaults(_.extend({}, defaults, attrs), defaults);
  this.set(attrs, options);
  this.changed = {};
  this.initialize.apply(this, arguments);
};
...
```

#### <a name="apidoc.element.backbone.Model.prototype.pick"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>pick ()](#apidoc.element.backbone.Model.prototype.pick)
- description and source-code
```javascript
pick = function () {
  var args = slice.call(arguments);
  args.unshift(this[attribute]);
  return _[method].apply(_, args);
}
```
- example usage
```shell
...
// having to worry about render order ... and makes it easy for the view to
// react to specific changes in the state of your models.

// Creating a Backbone.View creates its initial element outside of the DOM,
// if an existing element is not provided...
var View = Backbone.View = function(options) {
  this.cid = _.uniqueId('view');
  _.extend(this, _.pick(options, viewOptions));
  this._ensureElement();
  this.initialize.apply(this, arguments);
};

// Cached regex to split keys for 'delegate'.
var delegateEventSplitter = /^(\S+)\s*(.*)$/;
...
```

#### <a name="apidoc.element.backbone.Model.prototype.previous"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>previous (attr)](#apidoc.element.backbone.Model.prototype.previous)
- description and source-code
```javascript
previous = function (attr) {
  if (attr == null || !this._previousAttributes) return null;
  return this._previousAttributes[attr];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.previousAttributes"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>previousAttributes ()](#apidoc.element.backbone.Model.prototype.previousAttributes)
- description and source-code
```javascript
previousAttributes = function () {
  return _.clone(this._previousAttributes);
}
```
- example usage
```shell
...
// events simply proxy through. "add" and "remove" events that originate
// in other collections are ignored.
_onModelEvent: function(event, model, collection, options) {
  if (model) {
    if ((event === 'add' || event === 'remove') && collection !== this) return;
    if (event === 'destroy') this.remove(model, options);
    if (event === 'change') {
      var prevId = this.modelId(model.previousAttributes());
      var id = this.modelId(model.attributes);
      if (prevId !== id) {
        if (prevId != null) delete this._byId[prevId];
        if (id != null) this._byId[id] = model;
      }
    }
  }
...
```

#### <a name="apidoc.element.backbone.Model.prototype.save"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>save (key, val, options)](#apidoc.element.backbone.Model.prototype.save)
- description and source-code
```javascript
save = function (key, val, options) {
  // Handle both '"key", value' and '{key: value}' -style arguments.
  var attrs;
  if (key == null || typeof key === 'object') {
    attrs = key;
    options = val;
  } else {
    (attrs = {})[key] = val;
  }

  options = _.extend({validate: true, parse: true}, options);
  var wait = options.wait;

  // If we're not waiting and attributes exist, save acts as
  // 'set(attr).save(null, opts)' with validation. Otherwise, check if
  // the model will be valid when the attributes, if any, are set.
  if (attrs && !wait) {
    if (!this.set(attrs, options)) return false;
  } else if (!this._validate(attrs, options)) {
    return false;
  }

  // After a successful server-side save, the client is (optionally)
  // updated with the server-side state.
  var model = this;
  var success = options.success;
  var attributes = this.attributes;
  options.success = function(resp) {
    // Ensure attributes are restored during synchronous saves.
    model.attributes = attributes;
    var serverAttrs = options.parse ? model.parse(resp, options) : resp;
    if (wait) serverAttrs = _.extend({}, attrs, serverAttrs);
    if (serverAttrs && !model.set(serverAttrs, options)) return false;
    if (success) success.call(options.context, model, resp, options);
    model.trigger('sync', model, resp, options);
  };
  wrapError(this, options);

  // Set temporary attributes if '{wait: true}' to properly find new ids.
  if (attrs && wait) this.attributes = _.extend({}, attributes, attrs);

  var method = this.isNew() ? 'create' : (options.patch ? 'patch' : 'update');
  if (method === 'patch' && !options.attrs) options.attrs = attrs;
  var xhr = this.sync(method, this, options);

  // Restore attributes.
  this.attributes = attributes;

  return xhr;
}
```
- example usage
```shell
...
  (attrs = {})[key] = val;
}

options = _.extend({validate: true, parse: true}, options);
var wait = options.wait;

// If we're not waiting and attributes exist, save acts as
// 'set(attr).save(null, opts)' with validation. Otherwise, check if
// the model will be valid when the attributes, if any, are set.
if (attrs && !wait) {
  if (!this.set(attrs, options)) return false;
} else if (!this._validate(attrs, options)) {
  return false;
}
...
```

#### <a name="apidoc.element.backbone.Model.prototype.set"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>set (key, val, options)](#apidoc.element.backbone.Model.prototype.set)
- description and source-code
```javascript
set = function (key, val, options) {
  if (key == null) return this;

  // Handle both '"key", value' and '{key: value}' -style arguments.
  var attrs;
  if (typeof key === 'object') {
    attrs = key;
    options = val;
  } else {
    (attrs = {})[key] = val;
  }

  options || (options = {});

  // Run validation.
  if (!this._validate(attrs, options)) return false;

  // Extract attributes and options.
  var unset      = options.unset;
  var silent     = options.silent;
  var changes    = [];
  var changing   = this._changing;
  this._changing = true;

  if (!changing) {
    this._previousAttributes = _.clone(this.attributes);
    this.changed = {};
  }

  var current = this.attributes;
  var changed = this.changed;
  var prev    = this._previousAttributes;

  // For each 'set' attribute, update or delete the current value.
  for (var attr in attrs) {
    val = attrs[attr];
    if (!_.isEqual(current[attr], val)) changes.push(attr);
    if (!_.isEqual(prev[attr], val)) {
      changed[attr] = val;
    } else {
      delete changed[attr];
    }
    unset ? delete current[attr] : current[attr] = val;
  }

  // Update the 'id'.
  if (this.idAttribute in attrs) this.id = this.get(this.idAttribute);

  // Trigger all relevant attribute changes.
  if (!silent) {
    if (changes.length) this._pending = options;
    for (var i = 0; i < changes.length; i++) {
      this.trigger('change:' + changes[i], this, current[changes[i]], options);
    }
  }

  // You might be wondering why there's a 'while' loop here. Changes can
  // be recursively nested within '"change"' events.
  if (changing) return this;
  if (!silent) {
    while (this._pending) {
      options = this._pending;
      this._pending = false;
      this.trigger('change', this, options);
    }
  }
  this._pending = false;
  this._changing = false;
  return this;
}
```
- example usage
```shell
...
  options || (options = {});
  this.cid = _.uniqueId(this.cidPrefix);
  this.attributes = {};
  if (options.collection) this.collection = options.collection;
  if (options.parse) attrs = this.parse(attrs, options) || {};
  var defaults = _.result(this, 'defaults');
  attrs = _.defaults(_.extend({}, defaults, attrs), defaults);
  this.set(attrs, options);
  this.changed = {};
  this.initialize.apply(this, arguments);
};

// Attach all inheritable methods to the Model prototype.
_.extend(Model.prototype, Events, {
...
```

#### <a name="apidoc.element.backbone.Model.prototype.stopListening"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.Model.prototype.stopListening)
- description and source-code
```javascript
stopListening = function (obj, name, callback) {
  var listeningTo = this._listeningTo;
  if (!listeningTo) return this;

  var ids = obj ? [obj._listenId] : _.keys(listeningTo);

  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
}
```
- example usage
```shell
...
    destroy: function(options) {
options = options ? _.clone(options) : {};
var model = this;
var success = options.success;
var wait = options.wait;

var destroy = function() {
  model.stopListening();
  model.trigger('destroy', model, model.collection, options);
};

options.success = function(resp) {
  if (wait) destroy();
  if (success) success.call(options.context, model, resp, options);
  if (!model.isNew()) model.trigger('sync', model, resp, options);
...
```

#### <a name="apidoc.element.backbone.Model.prototype.sync"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>sync ()](#apidoc.element.backbone.Model.prototype.sync)
- description and source-code
```javascript
sync = function () {
  return Backbone.sync.apply(this, arguments);
}
```
- example usage
```shell
...
  options.success = function(resp) {
    var serverAttrs = options.parse ? model.parse(resp, options) : resp;
    if (!model.set(serverAttrs, options)) return false;
    if (success) success.call(options.context, model, resp, options);
    model.trigger('sync', model, resp, options);
  };
  wrapError(this, options);
  return this.sync('read', this, options);
},

// Set a hash of model attributes, and sync the model to the server.
// If the server returns an attributes hash that differs, the model's
// state will be 'set' again.
save: function(key, val, options) {
  // Handle both '"key", value' and '{key: value}' -style arguments.
...
```

#### <a name="apidoc.element.backbone.Model.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>toJSON (options)](#apidoc.element.backbone.Model.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (options) {
  return _.clone(this.attributes);
}
```
- example usage
```shell
...
// Initialize is an empty function by default. Override it with your own
// initialization logic.
initialize: function(){},

// The JSON representation of a Collection is an array of the
// models' attributes.
toJSON: function(options) {
  return this.map(function(model) { return model.toJSON(options); });
},

// Proxy 'Backbone.sync' by default.
sync: function() {
  return Backbone.sync.apply(this, arguments);
},
...
```

#### <a name="apidoc.element.backbone.Model.prototype.trigger"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>trigger (name)](#apidoc.element.backbone.Model.prototype.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;

  var length = Math.max(0, arguments.length - 1);
  var args = Array(length);
  for (var i = 0; i < length; i++) args[i] = arguments[i + 1];

  eventsApi(triggerApi, this._events, name, void 0, args);
  return this;
}
```
- example usage
```shell
...
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;

// Iterates over the standard 'event, callback' (as well as the fancy multiple
...
```

#### <a name="apidoc.element.backbone.Model.prototype.unbind"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>unbind (name, callback, context)](#apidoc.element.backbone.Model.prototype.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.unset"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>unset (attr, options)](#apidoc.element.backbone.Model.prototype.unset)
- description and source-code
```javascript
unset = function (attr, options) {
  return this.set(attr, void 0, _.extend({}, options, {unset: true}));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.url"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>url ()](#apidoc.element.backbone.Model.prototype.url)
- description and source-code
```javascript
url = function () {
  var base =
    _.result(this, 'urlRoot') ||
    _.result(this.collection, 'url') ||
    urlError();
  if (this.isNew()) return base;
  var id = this.get(this.idAttribute);
  return base.replace(/[^\/]$/, '$&/') + encodeURIComponent(id);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Model.prototype.values"></a>[function <span class="apidocSignatureSpan">backbone.Model.prototype.</span>values ()](#apidoc.element.backbone.Model.prototype.values)
- description and source-code
```javascript
values = function () {
  return _[method](this[attribute]);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.backbone.Router"></a>[module backbone.Router](#apidoc.module.backbone.Router)

#### <a name="apidoc.element.backbone.Router.Router"></a>[function <span class="apidocSignatureSpan">backbone.</span>Router (options)](#apidoc.element.backbone.Router.Router)
- description and source-code
```javascript
Router = function (options) {
  options || (options = {});
  if (options.routes) this.routes = options.routes;
  this._bindRoutes();
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Router.extend"></a>[function <span class="apidocSignatureSpan">backbone.Router.</span>extend (protoProps, staticProps)](#apidoc.element.backbone.Router.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ return parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function and add the prototype properties.
  child.prototype = _.create(parent.prototype, protoProps);
  child.prototype.constructor = child;

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...

// A module that can be mixed in to *any object* in order to provide it with
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;
...
```



# <a name="apidoc.module.backbone.Router.prototype"></a>[module backbone.Router.prototype](#apidoc.module.backbone.Router.prototype)

#### <a name="apidoc.element.backbone.Router.prototype._bindRoutes"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>_bindRoutes ()](#apidoc.element.backbone.Router.prototype._bindRoutes)
- description and source-code
```javascript
_bindRoutes = function () {
  if (!this.routes) return;
  this.routes = _.result(this, 'routes');
  var route, routes = _.keys(this.routes);
  while ((route = routes.pop()) != null) {
    this.route(route, this.routes[route]);
  }
}
```
- example usage
```shell
...
// ---------------

// Routers map faux-URLs to actions, and fire events when routes are
// matched. Creating a new one sets its 'routes' hash, if not set statically.
var Router = Backbone.Router = function(options) {
  options || (options = {});
  if (options.routes) this.routes = options.routes;
  this._bindRoutes();
  this.initialize.apply(this, arguments);
};

// Cached regular expressions for matching named param parts and splatted
// parts of route strings.
var optionalParam = /\((.*?)\)/g;
var namedParam    = /(\(\?)?:\w+/g;
...
```

#### <a name="apidoc.element.backbone.Router.prototype._extractParameters"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>_extractParameters (route, fragment)](#apidoc.element.backbone.Router.prototype._extractParameters)
- description and source-code
```javascript
_extractParameters = function (route, fragment) {
  var params = route.exec(fragment).slice(1);
  return _.map(params, function(param, i) {
    // Don't decode the search params.
    if (i === params.length - 1) return param || null;
    return param ? decodeURIComponent(param) : null;
  });
}
```
- example usage
```shell
...
if (_.isFunction(name)) {
  callback = name;
  name = '';
}
if (!callback) callback = this[name];
var router = this;
Backbone.history.route(route, function(fragment) {
  var args = router._extractParameters(route, fragment);
  if (router.execute(callback, args, name) !== false) {
    router.trigger.apply(router, ['route:' + name].concat(args));
    router.trigger('route', name, args);
    Backbone.history.trigger('route', router, name, args);
  }
});
return this;
...
```

#### <a name="apidoc.element.backbone.Router.prototype._routeToRegExp"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>_routeToRegExp (route)](#apidoc.element.backbone.Router.prototype._routeToRegExp)
- description and source-code
```javascript
_routeToRegExp = function (route) {
  route = route.replace(escapeRegExp, '\\$&')
               .replace(optionalParam, '(?:$1)?')
               .replace(namedParam, function(match, optional) {
                 return optional ? match : '([^/?]+)';
               })
               .replace(splatParam, '([^?]*?)');
  return new RegExp('^' + route + '(?:\\?([\\s\\S]*))?$');
}
```
- example usage
```shell
...
// Manually bind a single named route to a callback. For example:
//
//     this.route('search/:query/p:num', 'search', function(query, num) {
//       ...
//     });
//
route: function(route, name, callback) {
  if (!_.isRegExp(route)) route = this._routeToRegExp(route);
  if (_.isFunction(name)) {
    callback = name;
    name = '';
  }
  if (!callback) callback = this[name];
  var router = this;
  Backbone.history.route(route, function(fragment) {
...
```

#### <a name="apidoc.element.backbone.Router.prototype.bind"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>bind (name, callback, context)](#apidoc.element.backbone.Router.prototype.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...

// Bind an event to only be triggered a single time. After the first time
// the callback is invoked, its listener will be removed. If multiple events
// are passed in using the space-separated syntax, the handler will fire
// once for each event, not once for a combination of all events.
Events.once = function(name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
...
```

#### <a name="apidoc.element.backbone.Router.prototype.execute"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>execute (callback, args, name)](#apidoc.element.backbone.Router.prototype.execute)
- description and source-code
```javascript
execute = function (callback, args, name) {
  if (callback) callback.apply(this, args);
}
```
- example usage
```shell
...
    callback = name;
    name = '';
  }
  if (!callback) callback = this[name];
  var router = this;
  Backbone.history.route(route, function(fragment) {
    var args = router._extractParameters(route, fragment);
    if (router.execute(callback, args, name) !== false) {
      router.trigger.apply(router, ['route:' + name].concat(args));
      router.trigger('route', name, args);
      Backbone.history.trigger('route', router, name, args);
    }
  });
  return this;
},
...
```

#### <a name="apidoc.element.backbone.Router.prototype.initialize"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>initialize ()](#apidoc.element.backbone.Router.prototype.initialize)
- description and source-code
```javascript
initialize = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Router.prototype.listenTo"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.Router.prototype.listenTo)
- description and source-code
```javascript
listenTo = function (obj, name, callback) {
  if (!obj) return this;
  var id = obj._listenId || (obj._listenId = _.uniqueId('l'));
  var listeningTo = this._listeningTo || (this._listeningTo = {});
  var listening = listeningTo[id];

  // This object is not listening to any other events on 'obj' yet.
  // Setup the necessary references to track the listening callbacks.
  if (!listening) {
    var thisId = this._listenId || (this._listenId = _.uniqueId('l'));
    listening = listeningTo[id] = {obj: obj, objId: id, id: thisId, listeningTo: listeningTo, count: 0};
  }

  // Bind callbacks on obj, and keep track of them on listening.
  internalOn(obj, name, callback, this, listening);
  return this;
}
```
- example usage
```shell
...
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
...
```

#### <a name="apidoc.element.backbone.Router.prototype.listenToOnce"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.Router.prototype.listenToOnce)
- description and source-code
```javascript
listenToOnce = function (obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.Router.prototype.navigate"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>navigate (fragment, options)](#apidoc.element.backbone.Router.prototype.navigate)
- description and source-code
```javascript
navigate = function (fragment, options) {
  Backbone.history.navigate(fragment, options);
  return this;
}
```
- example usage
```shell
...
// excellent place to do pre-route setup or post-route cleanup.
execute: function(callback, args, name) {
  if (callback) callback.apply(this, args);
},

// Simple proxy to 'Backbone.history' to save a fragment into the history.
navigate: function(fragment, options) {
  Backbone.history.navigate(fragment, options);
  return this;
},

// Bind all defined routes to 'Backbone.history'. We have to reverse the
// order of the routes here to support behavior where the most general
// routes can be defined at the bottom of the route map.
_bindRoutes: function() {
...
```

#### <a name="apidoc.element.backbone.Router.prototype.off"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>off (name, callback, context)](#apidoc.element.backbone.Router.prototype.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
...
  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
};

// The reducing API that removes a callback from the 'events' object.
var offApi = function(events, name, callback, options) {
...
```

#### <a name="apidoc.element.backbone.Router.prototype.on"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>on (name, callback, context)](#apidoc.element.backbone.Router.prototype.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...
// A module that can be mixed in to *any object* in order to provide it with
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;
...
```

#### <a name="apidoc.element.backbone.Router.prototype.once"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>once (name, callback, context)](#apidoc.element.backbone.Router.prototype.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
}
```
- example usage
```shell
...
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
      offer(name, once);
      callback.apply(this, arguments);
    });
    once._callback = callback;
  }
  return map;
};
...
```

#### <a name="apidoc.element.backbone.Router.prototype.route"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>route (route, name, callback)](#apidoc.element.backbone.Router.prototype.route)
- description and source-code
```javascript
route = function (route, name, callback) {
  if (!_.isRegExp(route)) route = this._routeToRegExp(route);
  if (_.isFunction(name)) {
    callback = name;
    name = '';
  }
  if (!callback) callback = this[name];
  var router = this;
  Backbone.history.route(route, function(fragment) {
    var args = router._extractParameters(route, fragment);
    if (router.execute(callback, args, name) !== false) {
      router.trigger.apply(router, ['route:' + name].concat(args));
      router.trigger('route', name, args);
      Backbone.history.trigger('route', router, name, args);
    }
  });
  return this;
}
```
- example usage
```shell
...

// Initialize is an empty function by default. Override it with your own
// initialization logic.
initialize: function(){},

// Manually bind a single named route to a callback. For example:
//
//     this.route('search/:query/p:num', 'search', function(query, num) {
//       ...
//     });
//
route: function(route, name, callback) {
  if (!_.isRegExp(route)) route = this._routeToRegExp(route);
  if (_.isFunction(name)) {
    callback = name;
...
```

#### <a name="apidoc.element.backbone.Router.prototype.stopListening"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.Router.prototype.stopListening)
- description and source-code
```javascript
stopListening = function (obj, name, callback) {
  var listeningTo = this._listeningTo;
  if (!listeningTo) return this;

  var ids = obj ? [obj._listenId] : _.keys(listeningTo);

  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
}
```
- example usage
```shell
...
    destroy: function(options) {
options = options ? _.clone(options) : {};
var model = this;
var success = options.success;
var wait = options.wait;

var destroy = function() {
  model.stopListening();
  model.trigger('destroy', model, model.collection, options);
};

options.success = function(resp) {
  if (wait) destroy();
  if (success) success.call(options.context, model, resp, options);
  if (!model.isNew()) model.trigger('sync', model, resp, options);
...
```

#### <a name="apidoc.element.backbone.Router.prototype.trigger"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>trigger (name)](#apidoc.element.backbone.Router.prototype.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;

  var length = Math.max(0, arguments.length - 1);
  var args = Array(length);
  for (var i = 0; i < length; i++) args[i] = arguments[i + 1];

  eventsApi(triggerApi, this._events, name, void 0, args);
  return this;
}
```
- example usage
```shell
...
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;

// Iterates over the standard 'event, callback' (as well as the fancy multiple
...
```

#### <a name="apidoc.element.backbone.Router.prototype.unbind"></a>[function <span class="apidocSignatureSpan">backbone.Router.prototype.</span>unbind (name, callback, context)](#apidoc.element.backbone.Router.prototype.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.backbone.View"></a>[module backbone.View](#apidoc.module.backbone.View)

#### <a name="apidoc.element.backbone.View.View"></a>[function <span class="apidocSignatureSpan">backbone.</span>View (options)](#apidoc.element.backbone.View.View)
- description and source-code
```javascript
View = function (options) {
  this.cid = _.uniqueId('view');
  _.extend(this, _.pick(options, viewOptions));
  this._ensureElement();
  this.initialize.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.View.extend"></a>[function <span class="apidocSignatureSpan">backbone.View.</span>extend (protoProps, staticProps)](#apidoc.element.backbone.View.extend)
- description and source-code
```javascript
extend = function (protoProps, staticProps) {
  var parent = this;
  var child;

  // The constructor function for the new subclass is either defined by you
  // (the "constructor" property in your 'extend' definition), or defaulted
  // by us to simply call the parent constructor.
  if (protoProps && _.has(protoProps, 'constructor')) {
    child = protoProps.constructor;
  } else {
    child = function(){ return parent.apply(this, arguments); };
  }

  // Add static properties to the constructor function, if supplied.
  _.extend(child, parent, staticProps);

  // Set the prototype chain to inherit from 'parent', without calling
  // 'parent''s constructor function and add the prototype properties.
  child.prototype = _.create(parent.prototype, protoProps);
  child.prototype.constructor = child;

  // Set a convenience property in case the parent's prototype is needed
  // later.
  child.__super__ = parent.prototype;

  return child;
}
```
- example usage
```shell
...

// A module that can be mixed in to *any object* in order to provide it with
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;
...
```



# <a name="apidoc.module.backbone.View.prototype"></a>[module backbone.View.prototype](#apidoc.module.backbone.View.prototype)

#### <a name="apidoc.element.backbone.View.prototype._createElement"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>_createElement (tagName)](#apidoc.element.backbone.View.prototype._createElement)
- description and source-code
```javascript
_createElement = function (tagName) {
  return document.createElement(tagName);
}
```
- example usage
```shell
...
// matching element, and re-assign it to 'el'. Otherwise, create
// an element from the 'id', 'className' and 'tagName' properties.
_ensureElement: function() {
  if (!this.el) {
    var attrs = _.extend({}, _.result(this, 'attributes'));
    if (this.id) attrs.id = _.result(this, 'id');
    if (this.className) attrs['class'] = _.result(this, 'className');
    this.setElement(this._createElement(_.result(this, 'tagName')));
    this._setAttributes(attrs);
  } else {
    this.setElement(_.result(this, 'el'));
  }
},

// Set attributes from a hash on this view's element.  Exposed for
...
```

#### <a name="apidoc.element.backbone.View.prototype._ensureElement"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>_ensureElement ()](#apidoc.element.backbone.View.prototype._ensureElement)
- description and source-code
```javascript
_ensureElement = function () {
  if (!this.el) {
    var attrs = _.extend({}, _.result(this, 'attributes'));
    if (this.id) attrs.id = _.result(this, 'id');
    if (this.className) attrs['class'] = _.result(this, 'className');
    this.setElement(this._createElement(_.result(this, 'tagName')));
    this._setAttributes(attrs);
  } else {
    this.setElement(_.result(this, 'el'));
  }
}
```
- example usage
```shell
...
// react to specific changes in the state of your models.

// Creating a Backbone.View creates its initial element outside of the DOM,
// if an existing element is not provided...
var View = Backbone.View = function(options) {
  this.cid = _.uniqueId('view');
  _.extend(this, _.pick(options, viewOptions));
  this._ensureElement();
  this.initialize.apply(this, arguments);
};

// Cached regex to split keys for 'delegate'.
var delegateEventSplitter = /^(\S+)\s*(.*)$/;

// List of view options to be set as properties.
...
```

#### <a name="apidoc.element.backbone.View.prototype._removeElement"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>_removeElement ()](#apidoc.element.backbone.View.prototype._removeElement)
- description and source-code
```javascript
_removeElement = function () {
  this.$el.remove();
}
```
- example usage
```shell
...
render: function() {
  return this;
},

// Remove this view by taking the element out of the DOM, and removing any
// applicable Backbone.Events listeners.
remove: function() {
  this._removeElement();
  this.stopListening();
  return this;
},

// Remove this view's element from the document and all event listeners
// attached to it. Exposed for subclasses using an alternative DOM
// manipulation API.
...
```

#### <a name="apidoc.element.backbone.View.prototype._setAttributes"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>_setAttributes (attributes)](#apidoc.element.backbone.View.prototype._setAttributes)
- description and source-code
```javascript
_setAttributes = function (attributes) {
  this.$el.attr(attributes);
}
```
- example usage
```shell
...
// an element from the 'id', 'className' and 'tagName' properties.
_ensureElement: function() {
  if (!this.el) {
    var attrs = _.extend({}, _.result(this, 'attributes'));
    if (this.id) attrs.id = _.result(this, 'id');
    if (this.className) attrs['class'] = _.result(this, 'className');
    this.setElement(this._createElement(_.result(this, 'tagName')));
    this._setAttributes(attrs);
  } else {
    this.setElement(_.result(this, 'el'));
  }
},

// Set attributes from a hash on this view's element.  Exposed for
// subclasses using an alternative DOM manipulation API.
...
```

#### <a name="apidoc.element.backbone.View.prototype._setElement"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>_setElement (el)](#apidoc.element.backbone.View.prototype._setElement)
- description and source-code
```javascript
_setElement = function (el) {
  this.$el = el instanceof Backbone.$ ? el : Backbone.$(el);
  this.el = this.$el[0];
}
```
- example usage
```shell
...
  this.$el.remove();
},

// Change the view's element ('this.el' property) and re-delegate the
// view's events on the new element.
setElement: function(element) {
  this.undelegateEvents();
  this._setElement(element);
  this.delegateEvents();
  return this;
},

// Creates the 'this.el' and 'this.$el' references for this view using the
// given 'el'. 'el' can be a CSS selector or an HTML string, a jQuery
// context or an element. Subclasses can override this to utilize an
...
```

#### <a name="apidoc.element.backbone.View.prototype.bind"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>bind (name, callback, context)](#apidoc.element.backbone.View.prototype.bind)
- description and source-code
```javascript
bind = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...

// Bind an event to only be triggered a single time. After the first time
// the callback is invoked, its listener will be removed. If multiple events
// are passed in using the space-separated syntax, the handler will fire
// once for each event, not once for a combination of all events.
Events.once = function(name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
...
```

#### <a name="apidoc.element.backbone.View.prototype.delegate"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>delegate (eventName, selector, listener)](#apidoc.element.backbone.View.prototype.delegate)
- description and source-code
```javascript
delegate = function (eventName, selector, listener) {
  this.$el.on(eventName + '.delegateEvents' + this.cid, selector, listener);
  return this;
}
```
- example usage
```shell
...
  if (!events) return this;
  this.undelegateEvents();
  for (var key in events) {
    var method = events[key];
    if (!_.isFunction(method)) method = this[method];
    if (!method) continue;
    var match = key.match(delegateEventSplitter);
    this.delegate(match[1], match[2], _.bind(method, this));
  }
  return this;
},

// Add a single event listener to the view's element (or a child element
// using 'selector'). This only works for delegate-able events: not 'focus',
// 'blur', and not 'change', 'submit', and 'reset' in Internet Explorer.
...
```

#### <a name="apidoc.element.backbone.View.prototype.delegateEvents"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>delegateEvents (events)](#apidoc.element.backbone.View.prototype.delegateEvents)
- description and source-code
```javascript
delegateEvents = function (events) {
  events || (events = _.result(this, 'events'));
  if (!events) return this;
  this.undelegateEvents();
  for (var key in events) {
    var method = events[key];
    if (!_.isFunction(method)) method = this[method];
    if (!method) continue;
    var match = key.match(delegateEventSplitter);
    this.delegate(match[1], match[2], _.bind(method, this));
  }
  return this;
}
```
- example usage
```shell
...
},

// Change the view's element ('this.el' property) and re-delegate the
// view's events on the new element.
setElement: function(element) {
  this.undelegateEvents();
  this._setElement(element);
  this.delegateEvents();
  return this;
},

// Creates the 'this.el' and 'this.$el' references for this view using the
// given 'el'. 'el' can be a CSS selector or an HTML string, a jQuery
// context or an element. Subclasses can override this to utilize an
// alternative DOM manipulation API and are only required to set the
...
```

#### <a name="apidoc.element.backbone.View.prototype.initialize"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>initialize ()](#apidoc.element.backbone.View.prototype.initialize)
- description and source-code
```javascript
initialize = function (){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.View.prototype.listenTo"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>listenTo (obj, name, callback)](#apidoc.element.backbone.View.prototype.listenTo)
- description and source-code
```javascript
listenTo = function (obj, name, callback) {
  if (!obj) return this;
  var id = obj._listenId || (obj._listenId = _.uniqueId('l'));
  var listeningTo = this._listeningTo || (this._listeningTo = {});
  var listening = listeningTo[id];

  // This object is not listening to any other events on 'obj' yet.
  // Setup the necessary references to track the listening callbacks.
  if (!listening) {
    var thisId = this._listenId || (this._listenId = _.uniqueId('l'));
    listening = listeningTo[id] = {obj: obj, objId: id, id: thisId, listeningTo: listeningTo, count: 0};
  }

  // Bind callbacks on obj, and keep track of them on listening.
  internalOn(obj, name, callback, this, listening);
  return this;
}
```
- example usage
```shell
...
  return this.on(events, callback, context);
};

// Inversion-of-control versions of 'once'.
Events.listenToOnce = function(obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
...
```

#### <a name="apidoc.element.backbone.View.prototype.listenToOnce"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>listenToOnce (obj, name, callback)](#apidoc.element.backbone.View.prototype.listenToOnce)
- description and source-code
```javascript
listenToOnce = function (obj, name, callback) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.stopListening, this, obj));
  return this.listenTo(obj, events);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.View.prototype.off"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>off (name, callback, context)](#apidoc.element.backbone.View.prototype.off)
- description and source-code
```javascript
off = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
...
  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
};

// The reducing API that removes a callback from the 'events' object.
var offApi = function(events, name, callback, options) {
...
```

#### <a name="apidoc.element.backbone.View.prototype.on"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>on (name, callback, context)](#apidoc.element.backbone.View.prototype.on)
- description and source-code
```javascript
on = function (name, callback, context) {
  return internalOn(this, name, callback, context);
}
```
- example usage
```shell
...
// A module that can be mixed in to *any object* in order to provide it with
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;
...
```

#### <a name="apidoc.element.backbone.View.prototype.once"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>once (name, callback, context)](#apidoc.element.backbone.View.prototype.once)
- description and source-code
```javascript
once = function (name, callback, context) {
  // Map the event into a '{event: once}' object.
  var events = eventsApi(onceMap, {}, name, callback, _.bind(this.off, this));
  if (typeof name === 'string' && context == null) callback = void 0;
  return this.on(events, callback, context);
}
```
- example usage
```shell
...
  return this.listenTo(obj, events);
};

// Reduces the event callbacks into a map of '{event: onceWrapper}'.
// 'offer' unbinds the 'onceWrapper' after it has been called.
var onceMap = function(map, name, callback, offer) {
  if (callback) {
    var once = map[name] = _.once(function() {
      offer(name, once);
      callback.apply(this, arguments);
    });
    once._callback = callback;
  }
  return map;
};
...
```

#### <a name="apidoc.element.backbone.View.prototype.remove"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>remove ()](#apidoc.element.backbone.View.prototype.remove)
- description and source-code
```javascript
remove = function () {
  this._removeElement();
  this.stopListening();
  return this;
}
```
- example usage
```shell
...
push: function(model, options) {
  return this.add(model, _.extend({at: this.length}, options));
},

// Remove a model from the end of the collection.
pop: function(options) {
  var model = this.at(this.length - 1);
  return this.remove(model, options);
},

// Add a model to the beginning of the collection.
unshift: function(model, options) {
  return this.add(model, _.extend({at: 0}, options));
},
...
```

#### <a name="apidoc.element.backbone.View.prototype.render"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>render ()](#apidoc.element.backbone.View.prototype.render)
- description and source-code
```javascript
render = function () {
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.View.prototype.setElement"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>setElement (element)](#apidoc.element.backbone.View.prototype.setElement)
- description and source-code
```javascript
setElement = function (element) {
  this.undelegateEvents();
  this._setElement(element);
  this.delegateEvents();
  return this;
}
```
- example usage
```shell
...
// matching element, and re-assign it to 'el'. Otherwise, create
// an element from the 'id', 'className' and 'tagName' properties.
_ensureElement: function() {
  if (!this.el) {
    var attrs = _.extend({}, _.result(this, 'attributes'));
    if (this.id) attrs.id = _.result(this, 'id');
    if (this.className) attrs['class'] = _.result(this, 'className');
    this.setElement(this._createElement(_.result(this, 'tagName')));
    this._setAttributes(attrs);
  } else {
    this.setElement(_.result(this, 'el'));
  }
},

// Set attributes from a hash on this view's element.  Exposed for
...
```

#### <a name="apidoc.element.backbone.View.prototype.stopListening"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>stopListening (obj, name, callback)](#apidoc.element.backbone.View.prototype.stopListening)
- description and source-code
```javascript
stopListening = function (obj, name, callback) {
  var listeningTo = this._listeningTo;
  if (!listeningTo) return this;

  var ids = obj ? [obj._listenId] : _.keys(listeningTo);

  for (var i = 0; i < ids.length; i++) {
    var listening = listeningTo[ids[i]];

    // If listening doesn't exist, this object is not currently
    // listening to obj. Break out early.
    if (!listening) break;

    listening.obj.off(name, callback, this);
  }

  return this;
}
```
- example usage
```shell
...
    destroy: function(options) {
options = options ? _.clone(options) : {};
var model = this;
var success = options.success;
var wait = options.wait;

var destroy = function() {
  model.stopListening();
  model.trigger('destroy', model, model.collection, options);
};

options.success = function(resp) {
  if (wait) destroy();
  if (success) success.call(options.context, model, resp, options);
  if (!model.isNew()) model.trigger('sync', model, resp, options);
...
```

#### <a name="apidoc.element.backbone.View.prototype.trigger"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>trigger (name)](#apidoc.element.backbone.View.prototype.trigger)
- description and source-code
```javascript
trigger = function (name) {
  if (!this._events) return this;

  var length = Math.max(0, arguments.length - 1);
  var args = Array(length);
  for (var i = 0; i < length; i++) args[i] = arguments[i + 1];

  eventsApi(triggerApi, this._events, name, void 0, args);
  return this;
}
```
- example usage
```shell
...
// a custom event channel. You may bind a callback to an event with 'on' or
// remove with 'off'; 'trigger'-ing an event fires all callbacks in
// succession.
//
//     var object = {};
//     _.extend(object, Backbone.Events);
//     object.on('expand', function(){ alert('expanded'); });
//     object.trigger('expand');
//
var Events = Backbone.Events = {};

// Regular expression used to split event strings.
var eventSplitter = /\s+/;

// Iterates over the standard 'event, callback' (as well as the fancy multiple
...
```

#### <a name="apidoc.element.backbone.View.prototype.unbind"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>unbind (name, callback, context)](#apidoc.element.backbone.View.prototype.unbind)
- description and source-code
```javascript
unbind = function (name, callback, context) {
  if (!this._events) return this;
  this._events = eventsApi(offApi, this._events, name, callback, {
    context: context,
    listeners: this._listeners
  });
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.View.prototype.undelegate"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>undelegate (eventName, selector, listener)](#apidoc.element.backbone.View.prototype.undelegate)
- description and source-code
```javascript
undelegate = function (eventName, selector, listener) {
  this.$el.off(eventName + '.delegateEvents' + this.cid, selector, listener);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.backbone.View.prototype.undelegateEvents"></a>[function <span class="apidocSignatureSpan">backbone.View.prototype.</span>undelegateEvents ()](#apidoc.element.backbone.View.prototype.undelegateEvents)
- description and source-code
```javascript
undelegateEvents = function () {
  if (this.$el) this.$el.off('.delegateEvents' + this.cid);
  return this;
}
```
- example usage
```shell
...
_removeElement: function() {
  this.$el.remove();
},

// Change the view's element ('this.el' property) and re-delegate the
// view's events on the new element.
setElement: function(element) {
  this.undelegateEvents();
  this._setElement(element);
  this.delegateEvents();
  return this;
},

// Creates the 'this.el' and 'this.$el' references for this view using the
// given 'el'. 'el' can be a CSS selector or an HTML string, a jQuery
...
```



# <a name="apidoc.module.backbone.history"></a>[module backbone.history](#apidoc.module.backbone.history)

#### <a name="apidoc.element.backbone.history.checkUrl"></a>[function <span class="apidocSignatureSpan">backbone.history.</span>checkUrl ()](#apidoc.element.backbone.history.checkUrl)
- description and source-code
```javascript
checkUrl = function () { [native code] }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
