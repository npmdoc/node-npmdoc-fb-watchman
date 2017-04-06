# api documentation for  [fb-watchman (v2.0.0)](https://facebook.github.io/watchman/)  [![npm package](https://img.shields.io/npm/v/npmdoc-fb-watchman.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fb-watchman) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fb-watchman.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fb-watchman)
#### Bindings for the Watchman file watching service

[![NPM](https://nodei.co/npm/fb-watchman.png?downloads=true)](https://www.npmjs.com/package/fb-watchman)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fb-watchman/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-fb-watchman_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fb-watchman/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fb-watchman/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fb-watchman/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Wez Furlong",
        "email": "wez@fb.com",
        "url": "http://wezfurlong.org"
    },
    "bugs": {
        "url": "https://github.com/facebook/watchman/issues"
    },
    "dependencies": {
        "bser": "^2.0.0"
    },
    "description": "Bindings for the Watchman file watching service",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "54e9abf7dfa2f26cd9b1636c588c1afc05de5d58",
        "tarball": "https://registry.npmjs.org/fb-watchman/-/fb-watchman-2.0.0.tgz"
    },
    "files": [
        "index.js"
    ],
    "homepage": "https://facebook.github.io/watchman/",
    "keywords": [
        "facebook",
        "watchman",
        "file",
        "watch",
        "watcher",
        "watching",
        "fs.watch",
        "fswatcher",
        "fs",
        "glob",
        "utility"
    ],
    "license": "Apache-2.0",
    "main": "index.js",
    "maintainers": [
        {
            "name": "wez",
            "email": "wez@wezfurlong.org"
        }
    ],
    "name": "fb-watchman",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/facebook/watchman.git"
    },
    "scripts": {},
    "version": "2.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module fb-watchman](#apidoc.module.fb-watchman)
1.  [function <span class="apidocSignatureSpan">fb-watchman.</span>Client (options)](#apidoc.element.fb-watchman.Client)
1.  object <span class="apidocSignatureSpan">fb-watchman.</span>Client.prototype

#### [module fb-watchman.Client](#apidoc.module.fb-watchman.Client)
1.  [function <span class="apidocSignatureSpan">fb-watchman.</span>Client (options)](#apidoc.element.fb-watchman.Client.Client)
1.  [function <span class="apidocSignatureSpan">fb-watchman.Client.</span>super_ ()](#apidoc.element.fb-watchman.Client.super_)

#### [module fb-watchman.Client.prototype](#apidoc.module.fb-watchman.Client.prototype)
1.  [function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>_synthesizeCapabilityCheck ( resp, optional, required)](#apidoc.element.fb-watchman.Client.prototype._synthesizeCapabilityCheck)
1.  [function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>cancelCommands (why)](#apidoc.element.fb-watchman.Client.prototype.cancelCommands)
1.  [function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>capabilityCheck (caps, done)](#apidoc.element.fb-watchman.Client.prototype.capabilityCheck)
1.  [function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>command (args, done)](#apidoc.element.fb-watchman.Client.prototype.command)
1.  [function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>connect ()](#apidoc.element.fb-watchman.Client.prototype.connect)
1.  [function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>end ()](#apidoc.element.fb-watchman.Client.prototype.end)
1.  [function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>sendNextCommand ()](#apidoc.element.fb-watchman.Client.prototype.sendNextCommand)



# <a name="apidoc.module.fb-watchman"></a>[module fb-watchman](#apidoc.module.fb-watchman)

#### <a name="apidoc.element.fb-watchman.Client"></a>[function <span class="apidocSignatureSpan">fb-watchman.</span>Client (options)](#apidoc.element.fb-watchman.Client)
- description and source-code
```javascript
function Client(options) {
  var self = this;
  EE.call(this);

  this.watchmanBinaryPath = 'watchman';
  if (options && options.watchmanBinaryPath) {
    this.watchmanBinaryPath = options.watchmanBinaryPath.trim();
  };
  this.commands = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fb-watchman.Client"></a>[module fb-watchman.Client](#apidoc.module.fb-watchman.Client)

#### <a name="apidoc.element.fb-watchman.Client.Client"></a>[function <span class="apidocSignatureSpan">fb-watchman.</span>Client (options)](#apidoc.element.fb-watchman.Client.Client)
- description and source-code
```javascript
function Client(options) {
  var self = this;
  EE.call(this);

  this.watchmanBinaryPath = 'watchman';
  if (options && options.watchmanBinaryPath) {
    this.watchmanBinaryPath = options.watchmanBinaryPath.trim();
  };
  this.commands = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fb-watchman.Client.super_"></a>[function <span class="apidocSignatureSpan">fb-watchman.Client.</span>super_ ()](#apidoc.element.fb-watchman.Client.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fb-watchman.Client.prototype"></a>[module fb-watchman.Client.prototype](#apidoc.module.fb-watchman.Client.prototype)

#### <a name="apidoc.element.fb-watchman.Client.prototype._synthesizeCapabilityCheck"></a>[function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>_synthesizeCapabilityCheck ( resp, optional, required)](#apidoc.element.fb-watchman.Client.prototype._synthesizeCapabilityCheck)
- description and source-code
```javascript
_synthesizeCapabilityCheck = function ( resp, optional, required) {
  resp.capabilities = {}
  var version = resp.version;
  optional.forEach(function (name) {
    resp.capabilities[name] = have_cap(version, name);
  });
  required.forEach(function (name) {
    var have = have_cap(version, name);
    resp.capabilities[name] = have;
    if (!have) {
      resp.error = 'client required capability '' + name +
                   '' is not supported by this server';
    }
  });
  return resp;
}
```
- example usage
```shell
...
if (error) {
  done(error);
  return;
}
if (!('capabilities' in resp)) {
  // Server doesn't support capabilities, so we need to
  // synthesize the results based on the version
  resp = self._synthesizeCapabilityCheck(resp, optional, required);
  if (resp.error) {
    error = new Error(resp.error);
    error.watchmanResponse = resp;
    done(error);
    return;
  }
}
...
```

#### <a name="apidoc.element.fb-watchman.Client.prototype.cancelCommands"></a>[function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>cancelCommands (why)](#apidoc.element.fb-watchman.Client.prototype.cancelCommands)
- description and source-code
```javascript
cancelCommands = function (why) {
  var error = new Error(why);

  // Steal all pending commands before we start cancellation, in
  // case something decides to schedule more commands
  var cmds = this.commands;
  this.commands = [];

  if (this.currentCommand) {
    cmds.unshift(this.currentCommand);
    this.currentCommand = null;
  }

  // Synthesize an error condition for any commands that were queued
  cmds.forEach(function(cmd) {
    cmd.cb(error);
  });
}
```
- example usage
```shell
...
    if (self.bunser) {
      self.bunser.append(buf);
    }
  });
  self.socket.on('end', function() {
    self.socket = null;
    self.bunser = null;
    self.cancelCommands('The watchman connection was closed');
    self.emit('end');
  });
}

// triggers will export the sock path to the environment.
// If we're invoked in such a way, we can simply pick up the
// definition from the environment and avoid having to fork off
...
```

#### <a name="apidoc.element.fb-watchman.Client.prototype.capabilityCheck"></a>[function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>capabilityCheck (caps, done)](#apidoc.element.fb-watchman.Client.prototype.capabilityCheck)
- description and source-code
```javascript
capabilityCheck = function (caps, done) {
  var optional = caps.optional || [];
  var required = caps.required || [];
  var self = this;
  this.command(['version', {
      optional: optional,
      required: required
  }], function (error, resp) {
    if (error) {
      done(error);
      return;
    }
    if (!('capabilities' in resp)) {
      // Server doesn't support capabilities, so we need to
      // synthesize the results based on the version
      resp = self._synthesizeCapabilityCheck(resp, optional, required);
      if (resp.error) {
        error = new Error(resp.error);
        error.watchmanResponse = resp;
        done(error);
        return;
      }
    }
    done(null, resp);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fb-watchman.Client.prototype.command"></a>[function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>command (args, done)](#apidoc.element.fb-watchman.Client.prototype.command)
- description and source-code
```javascript
command = function (args, done) {
  done = done || function() {};

  // Queue up the command
  this.commands.push({cmd: args, cb: done});

  // Establish a connection if we don't already have one
  if (!this.socket) {
    if (!this.connecting) {
      this.connecting = true;
      this.connect();
      return;
    }
    return;
  }

  // If we're already connected and idle, try sending the command immediately
  this.sendNextCommand();
}
```
- example usage
```shell
...
return resp;
}

Client.prototype.capabilityCheck = function(caps, done) {
var optional = caps.optional || [];
var required = caps.required || [];
var self = this;
this.command(['version', {
    optional: optional,
    required: required
}], function (error, resp) {
  if (error) {
    done(error);
    return;
  }
...
```

#### <a name="apidoc.element.fb-watchman.Client.prototype.connect"></a>[function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>connect ()](#apidoc.element.fb-watchman.Client.prototype.connect)
- description and source-code
```javascript
connect = function () {
  var self = this;

  function makeSock(sockname) {
    // bunser will decode the watchman BSER protocol for us
    self.bunser = new bser.BunserBuf();
    // For each decoded line:
    self.bunser.on('value', function(obj) {
      // Figure out if this is a unliteral response or if it is the
      // response portion of a request-response sequence.  At the time
      // of writing, there are only two possible unilateral responses.
      var unilateral = false;
      for (var i = 0; i < unilateralTags.length; i++) {
        var tag = unilateralTags[i];
        if (tag in obj) {
          unilateral = tag;
        }
      }

      if (unilateral) {
        self.emit(unilateral, obj);
      } else if (self.currentCommand) {
        var cmd = self.currentCommand;
        self.currentCommand = null;
        if ('error' in obj) {
          var error = new Error(obj.error);
          error.watchmanResponse = obj;
          cmd.cb(error);
        } else {
          cmd.cb(null, obj);
        }
      }

      // See if we can dispatch the next queued command, if any
      self.sendNextCommand();
    });
    self.bunser.on('error', function(err) {
      self.emit('error', err);
    });

    self.socket = net.createConnection(sockname);
    self.socket.on('connect', function() {
      self.connecting = false;
      self.emit('connect');
      self.sendNextCommand();
    });
    self.socket.on('error', function(err) {
      self.connecting = false;
      self.emit('error', err);
    });
    self.socket.on('data', function(buf) {
      if (self.bunser) {
        self.bunser.append(buf);
      }
    });
    self.socket.on('end', function() {
      self.socket = null;
      self.bunser = null;
      self.cancelCommands('The watchman connection was closed');
      self.emit('end');
    });
  }

  // triggers will export the sock path to the environment.
  // If we're invoked in such a way, we can simply pick up the
  // definition from the environment and avoid having to fork off
  // a process to figure it out
  if (process.env.WATCHMAN_SOCK) {
    makeSock(process.env.WATCHMAN_SOCK);
    return;
  }

  // We need to ask the client binary where to find it.
  // This will cause the service to start for us if it isn't
  // already running.
  var args = ['--no-pretty', 'get-sockname'];

  // We use the more elaborate spawn rather than exec because there
  // are some error cases on Windows where process spawning can hang.
  // It is desirable to pipe stderr directly to stderr live so that
  // we can discover the problem.
  var proc = null;
  var spawnFailed = false;

  function spawnError(error) {
    if (spawnFailed) {
      // For ENOENT, proc 'close' will also trigger with a negative code,
      // let's suppress that second error.
      return;
    }
    spawnFailed = true;
    if (error.errno === 'EACCES') {
      error.message = 'The Watchman CLI is installed but cannot ' +
                      'be spawned because of a permission problem';
    } else if (error.errno === 'ENOENT') {
      error.message = 'Watchman was not found in PATH.  See ' +
          'https://facebook.github.io/watchman/docs/install.html ' +
          'for installation instructions';
    }
    console.error('Watchman: ', error.message);
    self.emit('error', error);
  }

  try {
    proc = childProcess.spawn(this.watchmanBinaryPath, args, {
      stdio: ['ignore', 'pipe', 'pipe']
    });
  } catch (error) {
    spawnError(error);
    return;
  }

  var stdout = [];
  var stderr = [];
  proc.stdout.on('data', function(data) {
    stdout.push(data);
  });
  proc.stderr.on('data', function(data) {
    data = data.toString('utf8');
    stderr.push(data);
    console.error(data);
  });
  proc.on('error', function(error) {
    spawnError(error);
  });

  proc.on('close', function (code, signal) {
    if (code !== 0) {
      spawnError(new Error(
          self.watchmanBinaryPath + ' ' + args.join(' ') +
          ' returned with exit code=' + code + ', signal=' +
          signal + ', stderr= ' + stderr.join('')));
      return;
    }
    try { ...
```
- example usage
```shell
...
// Queue up the command
this.commands.push({cmd: args, cb: done});

// Establish a connection if we don't already have one
if (!this.socket) {
  if (!this.connecting) {
    this.connecting = true;
    this.connect();
    return;
  }
  return;
}

// If we're already connected and idle, try sending the command immediately
this.sendNextCommand();
...
```

#### <a name="apidoc.element.fb-watchman.Client.prototype.end"></a>[function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>end ()](#apidoc.element.fb-watchman.Client.prototype.end)
- description and source-code
```javascript
end = function () {
  this.cancelCommands('The client was ended');
  if (this.socket) {
    this.socket.end();
    this.socket = null;
  }
  this.bunser = null;
}
```
- example usage
```shell
...
  });
}

// Close the connection to the service
Client.prototype.end = function() {
  this.cancelCommands('The client was ended');
  if (this.socket) {
    this.socket.end();
    this.socket = null;
  }
  this.bunser = null;
}
...
```

#### <a name="apidoc.element.fb-watchman.Client.prototype.sendNextCommand"></a>[function <span class="apidocSignatureSpan">fb-watchman.Client.prototype.</span>sendNextCommand ()](#apidoc.element.fb-watchman.Client.prototype.sendNextCommand)
- description and source-code
```javascript
sendNextCommand = function () {
  if (this.currentCommand) {
    // There's a command pending response, don't send this new one yet
    return;
  }

  this.currentCommand = this.commands.shift();
  if (!this.currentCommand) {
    // No further commands are queued
    return;
  }

  this.socket.write(bser.dumpToBuffer(this.currentCommand.cmd));
}
```
- example usage
```shell
...
      cmd.cb(error);
    } else {
      cmd.cb(null, obj);
    }
  }

  // See if we can dispatch the next queued command, if any
  self.sendNextCommand();
});
self.bunser.on('error', function(err) {
  self.emit('error', err);
});

self.socket = net.createConnection(sockname);
self.socket.on('connect', function() {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
