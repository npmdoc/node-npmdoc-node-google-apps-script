# api documentation for  [node-google-apps-script (v1.1.5)](https://github.com/danthareja/node-google-apps-script)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-google-apps-script.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-google-apps-script) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-google-apps-script.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-google-apps-script)
#### The easiest way to develop Google Apps Script projects

[![NPM](https://nodei.co/npm/node-google-apps-script.png?downloads=true)](https://www.npmjs.com/package/node-google-apps-script)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-google-apps-script/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-google-apps-script_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-google-apps-script/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-google-apps-script/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-google-apps-script/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dan Thareja",
        "url": "danthareja@gmail.com"
    },
    "bin": {
        "gapps": "./bin/gapps"
    },
    "bugs": {
        "url": "https://github.com/danthareja/node-google-apps-script/issues"
    },
    "dependencies": {
        "bluebird": "^2.9.30",
        "colors": "^1.0.3",
        "commander": "^2.7.1",
        "googleapis": "^2.0.5",
        "lodash": "^3.9.3",
        "mkdirp": "^0.5.1",
        "node-dir": "^0.1.6",
        "request": "^2.54.0"
    },
    "description": "The easiest way to develop Google Apps Script projects",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "f51f265def17fe8eacbdf545c01f00526da28780",
        "tarball": "https://registry.npmjs.org/node-google-apps-script/-/node-google-apps-script-1.1.5.tgz"
    },
    "gitHead": "e8150010a36cd4368df0192bc47a27c4dbb15bcf",
    "homepage": "https://github.com/danthareja/node-google-apps-script",
    "keywords": [
        "google",
        "apps",
        "script",
        "drive",
        "github",
        "source",
        "version",
        "control",
        "import",
        "export",
        "download",
        "upload",
        "push",
        "clone"
    ],
    "license": "MIT",
    "main": "index",
    "maintainers": [
        {
            "name": "danthareja",
            "email": "danthareja@gmail.com"
        }
    ],
    "name": "node-google-apps-script",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/danthareja/node-google-apps-script.git"
    },
    "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "version": "1.1.5"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-google-apps-script](#apidoc.module.node-google-apps-script)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.</span>auth (clientSecretPath, withWebserver)](#apidoc.element.node-google-apps-script.auth)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.</span>init (fileId, options)](#apidoc.element.node-google-apps-script.init)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.</span>upload ()](#apidoc.element.node-google-apps-script.upload)
1.  object <span class="apidocSignatureSpan">node-google-apps-script.</span>defaults
1.  object <span class="apidocSignatureSpan">node-google-apps-script.</span>manifestor
1.  object <span class="apidocSignatureSpan">node-google-apps-script.</span>util

#### [module node-google-apps-script.manifestor](#apidoc.module.node-google-apps-script.manifestor)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.manifestor.</span>build (externalFiles)](#apidoc.element.node-google-apps-script.manifestor.build)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.manifestor.</span>get ()](#apidoc.element.node-google-apps-script.manifestor.get)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.manifestor.</span>getExternalFiles (fileId)](#apidoc.element.node-google-apps-script.manifestor.getExternalFiles)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.manifestor.</span>set (config)](#apidoc.element.node-google-apps-script.manifestor.set)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.manifestor.</span>throwIfConfig ()](#apidoc.element.node-google-apps-script.manifestor.throwIfConfig)

#### [module node-google-apps-script.util](#apidoc.module.node-google-apps-script.util)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.util.</span>getFileExtension (file)](#apidoc.element.node-google-apps-script.util.getFileExtension)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.util.</span>getFileType (file)](#apidoc.element.node-google-apps-script.util.getFileType)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.util.</span>getFilesFromDisk (subdir)](#apidoc.element.node-google-apps-script.util.getFilesFromDisk)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.util.</span>hasFileOnDisk (filesOnDisk, file)](#apidoc.element.node-google-apps-script.util.hasFileOnDisk)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.util.</span>swapGStoJS (filename)](#apidoc.element.node-google-apps-script.util.swapGStoJS)
1.  [function <span class="apidocSignatureSpan">node-google-apps-script.util.</span>updateFileSource (existingFile, newFile)](#apidoc.element.node-google-apps-script.util.updateFileSource)



# <a name="apidoc.module.node-google-apps-script"></a>[module node-google-apps-script](#apidoc.module.node-google-apps-script)

#### <a name="apidoc.element.node-google-apps-script.auth"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.</span>auth (clientSecretPath, withWebserver)](#apidoc.element.node-google-apps-script.auth)
- description and source-code
```javascript
function auth(clientSecretPath, withWebserver) {
  return fs.lstatAsync(defaults.STORAGE_FILE)
    .then(function() {
      console.log(defaults.STORAGE_FILE + ' already exists. Remove it to re-authenticate node-google-apps-script');
      return Promise.resolve();
    })
    .catch(function(err) {
      if (!clientSecretPath) {
        throw defaults.STORAGE_FILE + ' does not exist yet. Specify a credential file with '--auth ~/Downloads/client_secret_abcd
.json'';
      }
      return performAuthenticationFlow(clientSecretPath, withWebserver);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-google-apps-script.init"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.</span>init (fileId, options)](#apidoc.element.node-google-apps-script.init)
- description and source-code
```javascript
function init(fileId, options) {
  var subdir = options.subdir || defaults.DEFAULT_SUBDIR;

  if(!fileIdIsValid(fileId)) {
    return;
  }

  var config = {
    path: subdir,
    fileId: fileId,
    key: options.key
  };

  var overwritePromise = options.overwrite ?
    Promise.resolve() :
    manifestor.throwIfConfig();

  return overwritePromise
    .then(function() {
      return manifestor.set(config);
    })
    .then(function() {
      return mkdirp(subdir);
    })
    .then(function(config) {
      return manifestor.getExternalFiles(fileId)
    })
    .map(function(file) {
      return writeExternalFile(file, subdir)
    })
    .catch(function(err) {
      console.log('Error running init command'.red);
      throw err;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-google-apps-script.upload"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.</span>upload ()](#apidoc.element.node-google-apps-script.upload)
- description and source-code
```javascript
function upload() {
  console.log('Pushing back up to Google Drive...');

  var fileId; // Hold in closure to avoid promise nesting

  return manifestor.get()
    .then(function(config) {
      fileId = config.fileId;
      return manifestor.getExternalFiles(fileId)
    })
    .then(function(externalFiles) {
      return manifestor.build(externalFiles);
    })
    .then(function(files) {
      return sendToGoogle(files, fileId);
    })
    .then(function() {
      console.log('The latest files were successfully uploaded to your Apps Script project.'.green);
    })
    .catch(function(err) {
      console.log('Upload failed.'.red);
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-google-apps-script.manifestor"></a>[module node-google-apps-script.manifestor](#apidoc.module.node-google-apps-script.manifestor)

#### <a name="apidoc.element.node-google-apps-script.manifestor.build"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.manifestor.</span>build (externalFiles)](#apidoc.element.node-google-apps-script.manifestor.build)
- description and source-code
```javascript
build = function (externalFiles) {
  return getConfig().get('path')
    .then(util.getFilesFromDisk)
    .then(function(files) {

      // for each manifest file, if it has an equivalent on disk, keep it
      // otherwise trash it
      var filesToUpload = _.filter(externalFiles, function(externalFile) {
        return util.hasFileOnDisk(files, externalFile);
      });

      _.each(files, function(file) {
        // Add new file or update existing record
        var manifestFile = getFileInManifest(filesToUpload, file);
        if (manifestFile === undefined) {
          // add
          filesToUpload.push({
            name: file.name,
            type: util.getFileType(file),
            source: file.content
          });

        } else {
          // update
          util.updateFileSource(manifestFile, file);
        }
      });

      return filesToUpload;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-google-apps-script.manifestor.get"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.manifestor.</span>get ()](#apidoc.element.node-google-apps-script.manifestor.get)
- description and source-code
```javascript
function getConfig() {
  return fs.readFileAsync(defaults.CONFIG_NAME)
    .then(JSON.parse)
    .catch(SyntaxError, function(err) {
      console.log('Error parsing config'.red);
      throw err;
    })
    .error(function(err) {
      console.log('Config does not exist'.red);
      throw err;
    });
}
```
- example usage
```shell
...

/**
  build generates a manifest to be uploaded to google drive
  @param externalFiles {Object} files in the cloud
  @return {Object} manifest
 */
var build = function(externalFiles) {
  return getConfig().get('path')
    .then(util.getFilesFromDisk)
    .then(function(files) {

// for each manifest file, if it has an equivalent on disk, keep it
// otherwise trash it
var filesToUpload = _.filter(externalFiles, function(externalFile) {
  return util.hasFileOnDisk(files, externalFile);
...
```

#### <a name="apidoc.element.node-google-apps-script.manifestor.getExternalFiles"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.manifestor.</span>getExternalFiles (fileId)](#apidoc.element.node-google-apps-script.manifestor.getExternalFiles)
- description and source-code
```javascript
function getExternalFiles(fileId) {
  return authenticate()
    .then(function(auth) {
      return getProjectFiles(fileId, auth);
    })
    .catch(function(err) {
      console.log('Script file ID not found. Please input an ID and try again.'.red);
      throw err;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-google-apps-script.manifestor.set"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.manifestor.</span>set (config)](#apidoc.element.node-google-apps-script.manifestor.set)
- description and source-code
```javascript
function setConfig(config) {
  return fs.writeFileAsync(defaults.CONFIG_NAME, JSON.stringify(config, "", 2))
    .then(function() {
      return config;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-google-apps-script.manifestor.throwIfConfig"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.manifestor.</span>throwIfConfig ()](#apidoc.element.node-google-apps-script.manifestor.throwIfConfig)
- description and source-code
```javascript
function throwIfConfig() {
  return fs.readFileAsync(defaults.CONFIG_NAME)
    .then(JSON.parse)
    .then(function() {
      throw 'Config already exists. Cowardly refusing to overwrite.';
    })
    .error(function() {
      // swallow error
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-google-apps-script.util"></a>[module node-google-apps-script.util](#apidoc.module.node-google-apps-script.util)

#### <a name="apidoc.element.node-google-apps-script.util.getFileExtension"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.util.</span>getFileExtension (file)](#apidoc.element.node-google-apps-script.util.getFileExtension)
- description and source-code
```javascript
function getFileExtension(file) {
  if (file.type === 'server_js') return '.js';
  if (file.type === 'html') return '.html';
  throw new Error('Unsupported file type found');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-google-apps-script.util.getFileType"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.util.</span>getFileType (file)](#apidoc.element.node-google-apps-script.util.getFileType)
- description and source-code
```javascript
function getFileType(file) {
  if (file.ext === '.js') return 'server_js';
  if (file.ext === '.gs') return 'server_js';
  if (file.ext === '.html') return 'html';
  throw new Error('Unsupported file type found. Google Apps Script only allows .js and .html');
}
```
- example usage
```shell
...
      _.each(files, function(file) {
// Add new file or update existing record
var manifestFile = getFileInManifest(filesToUpload, file);
if (manifestFile === undefined) {
  // add
  filesToUpload.push({
    name: file.name,
    type: util.getFileType(file),
    source: file.content
  });

} else {
  // update
  util.updateFileSource(manifestFile, file);
}
...
```

#### <a name="apidoc.element.node-google-apps-script.util.getFilesFromDisk"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.util.</span>getFilesFromDisk (subdir)](#apidoc.element.node-google-apps-script.util.getFilesFromDisk)
- description and source-code
```javascript
function getFilesFromDisk(subdir) {
  return new Promise(function(resolve, reject) {

    var filesOnDisk = [];

    // Only iterate through supported .js, .gs and .html files in dir
    dir.readFiles(subdir, { match: /.js$|.gs$|.html$/ },
      // Invoke this callback on each file
      function(err, content, filename, next) {
        if (err) return reject(err);

        // Parse file's absolute path and add its content to result object
        file = path.parse(filename);
        file.content = content;

        filesOnDisk.push(file);

        // Continue to next file
        next();
      },
      // finished callback.
      function(err) {
        if (err) return reject(err);
        resolve(filesOnDisk);
      });
  })
  .error(function() {
    // swallow ENOENT
    return [];
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-google-apps-script.util.hasFileOnDisk"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.util.</span>hasFileOnDisk (filesOnDisk, file)](#apidoc.element.node-google-apps-script.util.hasFileOnDisk)
- description and source-code
```javascript
function hasFileOnDisk(filesOnDisk, file) {
  return _.any(filesOnDisk, function(fileOnDisk) {
    var sameName = file.name === fileOnDisk.name;
    var sameType = file.type === getFileType(fileOnDisk);
    return sameName && sameType;
  });
}
```
- example usage
```shell
...
  return getConfig().get('path')
    .then(util.getFilesFromDisk)
    .then(function(files) {

// for each manifest file, if it has an equivalent on disk, keep it
// otherwise trash it
var filesToUpload = _.filter(externalFiles, function(externalFile) {
  return util.hasFileOnDisk(files, externalFile);
});

_.each(files, function(file) {
  // Add new file or update existing record
  var manifestFile = getFileInManifest(filesToUpload, file);
  if (manifestFile === undefined) {
    // add
...
```

#### <a name="apidoc.element.node-google-apps-script.util.swapGStoJS"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.util.</span>swapGStoJS (filename)](#apidoc.element.node-google-apps-script.util.swapGStoJS)
- description and source-code
```javascript
function swapGStoJS(filename) {
  if (filename.indexOf('.gs') === filename.length - 3) {
    return filename.substr(0, filename.lastIndexOf('.gs')) + '.js';
  }
  return filename;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-google-apps-script.util.updateFileSource"></a>[function <span class="apidocSignatureSpan">node-google-apps-script.util.</span>updateFileSource (existingFile, newFile)](#apidoc.element.node-google-apps-script.util.updateFileSource)
- description and source-code
```javascript
function updateFileSource(existingFile, newFile) {
  existingFile.source = newFile.content;
}
```
- example usage
```shell
...
            name: file.name,
            type: util.getFileType(file),
            source: file.content
          });

        } else {
          // update
          util.updateFileSource(manifestFile, file);
        }
      });

      return filesToUpload;
    });
};
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
