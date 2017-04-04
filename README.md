# api documentation for  [letsencrypt (v2.1.8)](https://github.com/Daplie/node-letsencrypt#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-letsencrypt.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-letsencrypt) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-letsencrypt.svg)](https://travis-ci.org/npmdoc/node-npmdoc-letsencrypt)
#### Let's Encrypt for node.js on npm

[![NPM](https://nodei.co/npm/letsencrypt.png?downloads=true)](https://www.npmjs.com/package/letsencrypt)

[![apidoc](https://npmdoc.github.io/node-npmdoc-letsencrypt/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-letsencrypt_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-letsencrypt/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-letsencrypt/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-letsencrypt/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "AJ ONeal",
        "email": "coolaj86@gmail.com",
        "url": "https://coolaj86.com/"
    },
    "bugs": {
        "url": "https://github.com/Daplie/node-letsencrypt/issues"
    },
    "dependencies": {
        "asn1js": "^1.2.12",
        "bluebird": "^3.0.6",
        "certpem": "^1.0.0",
        "homedir": "^0.6.0",
        "le-acme-core": "^2.0.5",
        "le-challenge-fs": "^2.0.2",
        "le-challenge-sni": "^2.0.0",
        "le-sni-auto": "^2.1.0",
        "le-store-certbot": "^2.0.3",
        "localhost.daplie.com-certificates": "^1.2.3",
        "node.extend": "^1.1.5",
        "pkijs": "^1.3.27",
        "rsa-compat": "^1.2.1"
    },
    "deprecated": "letsencrypt has been renamed to greenlock. Please find it at npm greenlock",
    "description": "Let's Encrypt for node.js on npm",
    "devDependencies": {
        "request": "^2.75.0"
    },
    "directories": {},
    "dist": {
        "shasum": "981ae1415b9fb372ae15f1156d5d32b7dcc78bdd",
        "tarball": "https://registry.npmjs.org/letsencrypt/-/letsencrypt-2.1.8.tgz"
    },
    "gitHead": "acf8a487de507ca46bf7bca6fbde390afbd500fc",
    "homepage": "https://github.com/Daplie/node-letsencrypt#readme",
    "keywords": [
        "letsencrypt",
        "letsencrypt.org",
        "le",
        "Let's Encrypt",
        "lejs",
        "le.js",
        "acme",
        "node",
        "nodejs",
        "node.js",
        "client"
    ],
    "license": "(MIT OR Apache-2.0)",
    "main": "index.js",
    "maintainers": [
        {
            "name": "coolaj86",
            "email": "coolaj86@gmail.com"
        },
        {
            "name": "insightfuls",
            "email": "insightful_schmidt@yahoo.com.au"
        },
        {
            "name": "michielbdejong",
            "email": "michiel@unhosted.org"
        }
    ],
    "name": "letsencrypt",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/Daplie/node-letsencrypt.git"
    },
    "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "version": "2.1.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module letsencrypt](#apidoc.module.letsencrypt)
1.  [function <span class="apidocSignatureSpan">letsencrypt.</span>_undefine (le)](#apidoc.element.letsencrypt._undefine)
1.  [function <span class="apidocSignatureSpan">letsencrypt.</span>create (le)](#apidoc.element.letsencrypt.create)
1.  number <span class="apidocSignatureSpan">letsencrypt.</span>rsaKeySize
1.  object <span class="apidocSignatureSpan">letsencrypt.</span>LE
1.  object <span class="apidocSignatureSpan">letsencrypt.</span>_undefined
1.  object <span class="apidocSignatureSpan">letsencrypt.</span>challengeTypes
1.  object <span class="apidocSignatureSpan">letsencrypt.</span>core
1.  object <span class="apidocSignatureSpan">letsencrypt.</span>defaults
1.  object <span class="apidocSignatureSpan">letsencrypt.</span>middleware
1.  object <span class="apidocSignatureSpan">letsencrypt.</span>utils
1.  string <span class="apidocSignatureSpan">letsencrypt.</span>acmeChallengePrefix
1.  string <span class="apidocSignatureSpan">letsencrypt.</span>challengeType
1.  string <span class="apidocSignatureSpan">letsencrypt.</span>productionServerUrl
1.  string <span class="apidocSignatureSpan">letsencrypt.</span>stagingServerUrl

#### [module letsencrypt.core](#apidoc.module.letsencrypt.core)
1.  [function <span class="apidocSignatureSpan">letsencrypt.core.</span>create (le)](#apidoc.element.letsencrypt.core.create)

#### [module letsencrypt.middleware](#apidoc.module.letsencrypt.middleware)
1.  [function <span class="apidocSignatureSpan">letsencrypt.middleware.</span>create (le)](#apidoc.element.letsencrypt.middleware.create)

#### [module letsencrypt.utils](#apidoc.module.letsencrypt.utils)
1.  [function <span class="apidocSignatureSpan">letsencrypt.utils.</span>attachCertInfo (results)](#apidoc.element.letsencrypt.utils.attachCertInfo)
1.  [function <span class="apidocSignatureSpan">letsencrypt.utils.</span>isValidDomain (domain)](#apidoc.element.letsencrypt.utils.isValidDomain)
1.  [function <span class="apidocSignatureSpan">letsencrypt.utils.</span>merge ()](#apidoc.element.letsencrypt.utils.merge)
1.  [function <span class="apidocSignatureSpan">letsencrypt.utils.</span>testEmail (email)](#apidoc.element.letsencrypt.utils.testEmail)
1.  [function <span class="apidocSignatureSpan">letsencrypt.utils.</span>tplCopy (copy)](#apidoc.element.letsencrypt.utils.tplCopy)



# <a name="apidoc.module.letsencrypt"></a>[module letsencrypt](#apidoc.module.letsencrypt)

#### <a name="apidoc.element.letsencrypt._undefine"></a>[function <span class="apidocSignatureSpan">letsencrypt.</span>_undefine (le)](#apidoc.element.letsencrypt._undefine)
- description and source-code
```javascript
_undefine = function (le) {
  Object.keys(LE._undefined).forEach(function (key) {
    if (!(key in le)) {
      le[key] = u;
    }
  });

  return le;
}
```
- example usage
```shell
...
      le.challenges['dns-01'] = require('le-challenge-dns').create({ debug: le.debug });
    } catch(e) {
      // not yet implemented
    }
  }
}

le = LE._undefine(le);
le.acmeChallengePrefix = LE.acmeChallengePrefix;
le.rsaKeySize = le.rsaKeySize || LE.rsaKeySize;
le.challengeType = le.challengeType || LE.challengeType;
le._ipc = ipc;
le.agreeToTerms = le.agreeToTerms || function (args, agreeCb) {
  agreeCb(new Error("'agreeToTerms' was not supplied to LE and 'agreeTos' was not supplied to LE.register"));
};
...
```

#### <a name="apidoc.element.letsencrypt.create"></a>[function <span class="apidocSignatureSpan">letsencrypt.</span>create (le)](#apidoc.element.letsencrypt.create)
- description and source-code
```javascript
create = function (le) {
  var PromiseA = require('bluebird');

  le.acme = le.acme || ACME.create({ debug: le.debug });
  le.store = le.store || require('le-store-certbot').create({ debug: le.debug });
  le.core = require('./lib/core');
  var log = le.log || _log;

  if (!le.challenges) {
    le.challenges = {};
  }
  if (!le.challenges['http-01']) {
    le.challenges['http-01'] = require('le-challenge-fs').create({ debug: le.debug });
  }
  if (!le.challenges['tls-sni-01']) {
    le.challenges['tls-sni-01'] = require('le-challenge-sni').create({ debug: le.debug });
  }
  if (!le.challenges['dns-01']) {
    try {
      le.challenges['dns-01'] = require('le-challenge-ddns').create({ debug: le.debug });
    } catch(e) {
      try {
        le.challenges['dns-01'] = require('le-challenge-dns').create({ debug: le.debug });
      } catch(e) {
        // not yet implemented
      }
    }
  }

  le = LE._undefine(le);
  le.acmeChallengePrefix = LE.acmeChallengePrefix;
  le.rsaKeySize = le.rsaKeySize || LE.rsaKeySize;
  le.challengeType = le.challengeType || LE.challengeType;
  le._ipc = ipc;
  le.agreeToTerms = le.agreeToTerms || function (args, agreeCb) {
    agreeCb(new Error("'agreeToTerms' was not supplied to LE and 'agreeTos' was not supplied to LE.register"));
  };

  if (!le.renewWithin) { le.renewWithin = 7 * DAY; }
  // renewBy has a default in le-sni-auto

  if (!le.server) {
    throw new Error("opts.server must be set to 'staging' or a production url, such as LE.productionServerUrl'");
  }
  if ('staging' === le.server) {
    le.server = LE.stagingServerUrl;
  }
  else if ('production' === le.server) {
    le.server = LE.productionServerUrl;
  }

  if (le.acme.create) {
    le.acme = le.acme.create(le);
  }
  le.acme = PromiseA.promisifyAll(le.acme);
  le._acmeOpts = le.acme.getOptions();
  Object.keys(le._acmeOpts).forEach(function (key) {
    if (!(key in le)) {
      le[key] = le._acmeOpts[key];
    }
  });

  if (le.store.create) {
    le.store = le.store.create(le);
  }
  le.store = PromiseA.promisifyAll(le.store);
  le.store.accounts = PromiseA.promisifyAll(le.store.accounts);
  le.store.certificates = PromiseA.promisifyAll(le.store.certificates);
  le._storeOpts = le.store.getOptions();
  Object.keys(le._storeOpts).forEach(function (key) {
    if (!(key in le)) {
      le[key] = le._storeOpts[key];
    }
  });


  //
  // Backwards compat for <= v2.1.7
  //
  if (le.challenge) {
    console.warn("Deprecated use of le.challenge. Use le.challenges['" + LE.challengeType + "'] instead.");
    le.challenges[le.challengeType] = le.challenge;
  }

  LE.challengeTypes.forEach(function (challengeType) {
    var challenger = le.challenges[challengeType];

    if (!challenger) {
      return;
    }

    if (challenger.create) {
      challenger = le.challenges[challengeType] = challenger.create(le);
    }
    challenger = le.challenges[challengeType] = PromiseA.promisifyAll(challenger);
    le['_challengeOpts_' + challengeType] = challenger.getOptions();
    Object.keys(le['_challengeOpts_' + challengeType]).forEach(function (key) {
      if (!(key in le)) {
        le[key] = le['_challengeOpts_' + challengeType][key];
      }
    });

    // TODO wrap these here and now with tplCopy?
    if (!challenger.set || 5 !== challenger.set.length) {
      throw new Error("le.challenges[" + challengeType + "].set receives the wrong number of arguments."
        + " You must define setChallenge as function (opts, domain, token, keyAuthorization, cb) { }");
    }
    if (challenger.get && 4 !== challenger.get.length) {
      throw new Error("le.challenges[" + challengeType + "].get receives the wrong number of arguments."
        + " You must define getChallenge as function (opts, domain, token, cb) { }");
    }
    if (!challenger.remove || 4 !== challenger.remove.length) {
      throw new Error("le.challenges[" + challengeType + "].remove receives the wrong number of arguments."
        + " You must define removeChallenge as function (opts, domain, token, cb) { }");
    }
    if (!challenger.loopback || 5 !== challenger.loopback.length) ...
```
- example usage
```shell
...

### Overly Simplified Example

Against my better judgement I'm providing a terribly oversimplified example
of how to use this library:

'''javascript
var le = require('letsencrypt').create({ server: 'staging' });

var opts = {
domains: ['example.com'], email: 'user@email.com', agreeTos: true
};

le.register(opts).then(function (certs) {
console.log(certs);
...
```



# <a name="apidoc.module.letsencrypt.core"></a>[module letsencrypt.core](#apidoc.module.letsencrypt.core)

#### <a name="apidoc.element.letsencrypt.core.create"></a>[function <span class="apidocSignatureSpan">letsencrypt.core.</span>create (le)](#apidoc.element.letsencrypt.core.create)
- description and source-code
```javascript
create = function (le) {
  var PromiseA = require('bluebird');
  var utils = require('./utils');
  var RSA = PromiseA.promisifyAll(require('rsa-compat').RSA);
  var log = le.log || _log; // allow custom log

  var core = {
    //
    // Helpers
    //
    getAcmeUrlsAsync: function (args) {
      var now = Date.now();

      // TODO check response header on request for cache time
      if ((now - le._ipc.acmeUrlsUpdatedAt) < 10 * 60 * 1000) {
        return PromiseA.resolve(le._ipc.acmeUrls);
      }

      return le.acme.getAcmeUrlsAsync(args.server).then(function (data) {
        le._ipc.acmeUrlsUpdatedAt = Date.now();
        le._ipc.acmeUrls = data;

        return le._ipc.acmeUrls;
      });
    }


    //
    // The Main Enchilada
    //

    //
    // Accounts
    //
  , accounts: {
      // Accounts
      registerAsync: function (args) {
        var err;
        var copy = utils.merge(args, le);
        var disagreeTos;
        args = utils.tplCopy(copy);

        disagreeTos = (!args.agreeTos && 'undefined' !== typeof args.agreeTos);
        if (!args.email || disagreeTos || (parseInt(args.rsaKeySize, 10) < 2048)) {
          err = new Error(
            "In order to register an account both 'email' and 'agreeTos' must be present"
              + " and 'rsaKeySize' must be 2048 or greater."
          );
          err.code = 'E_ARGS';
          return PromiseA.reject(err);
        }

        return utils.testEmail(args.email).then(function () {
          var keypairOpts = { public: true, pem: true };

          var promise = le.store.accounts.checkKeypairAsync(args).then(function (keypair) {
            if (keypair) {
              return RSA.import(keypair);
            }

            if (args.accountKeypair) {
              return le.store.accounts.setKeypairAsync(args, RSA.import(args.accountKeypair));
            }

            return RSA.generateKeypairAsync(args.rsaKeySize, 65537, keypairOpts).then(function (keypair) {
              keypair.privateKeyPem = RSA.exportPrivatePem(keypair);
              keypair.publicKeyPem = RSA.exportPublicPem(keypair);
              keypair.privateKeyJwk = RSA.exportPrivateJwk(keypair);
              return le.store.accounts.setKeypairAsync(args, keypair);
            });
          });

          return promise.then(function (keypair) {
            // Note: the ACME urls are always fetched fresh on purpose
            // TODO is this the right place for this?
            return core.getAcmeUrlsAsync(args).then(function (urls) {
              args._acmeUrls = urls;

              return le.acme.registerNewAccountAsync({
                email: args.email
              , newRegUrl: args._acmeUrls.newReg
              , agreeToTerms: function (tosUrl, agreeCb) {
                  if (true === args.agreeTos || tosUrl === args.agreeTos || tosUrl === le.agreeToTerms) {
                    agreeCb(null, tosUrl);
                    return;
                  }

                  // args.email = email;      // already there
                  // args.domains = domains   // already there
                  args.tosUrl = tosUrl;
                  le.agreeToTerms(args, agreeCb);
                }
              , accountKeypair: keypair

              , debug: le.debug || args.debug
              }).then(function (receipt) {
                var reg = {
                  keypair: keypair
                , receipt: receipt
                , email: args.email
                };

                // TODO move templating of arguments to right here?
                return le.store.accounts.setAsync(args, reg).then(function (account) {
                  // should now have account.id and account.accountId
                  args.account = account;
                  args.accountId = account.id;
                  return account;
                });
              });
            });
          });
        });
      }

      // Accounts
    , getAsync: function (args) {
        return core.accounts.checkAsync(args).then(function (account) {
          if (account) {
            return account;
          } else { ...
```
- example usage
```shell
...

### Overly Simplified Example

Against my better judgement I'm providing a terribly oversimplified example
of how to use this library:

'''javascript
var le = require('letsencrypt').create({ server: 'staging' });

var opts = {
domains: ['example.com'], email: 'user@email.com', agreeTos: true
};

le.register(opts).then(function (certs) {
console.log(certs);
...
```



# <a name="apidoc.module.letsencrypt.middleware"></a>[module letsencrypt.middleware](#apidoc.module.letsencrypt.middleware)

#### <a name="apidoc.element.letsencrypt.middleware.create"></a>[function <span class="apidocSignatureSpan">letsencrypt.middleware.</span>create (le)](#apidoc.element.letsencrypt.middleware.create)
- description and source-code
```javascript
create = function (le) {
  if (!le.challenges['http-01'] || !le.challenges['http-01'].get) {
    throw new Error("middleware requires challenge plugin with get method");
  }
  var log = le.log || _log;

  log(le.debug, "created middleware");
  return function (_app) {
    if (_app && 'function' !== typeof _app) {
      throw new Error("use le.middleware() or le.middleware(function (req, res) {})");
    }
    var prefix = le.acmeChallengePrefix || '/.well-known/acme-challenge/';

    return function (req, res, next) {
      if (0 !== req.url.indexOf(prefix)) {
        log(le.debug, "no match, skipping middleware");
        if ('function' === typeof _app) {
          _app(req, res, next);
        }
        else if ('function' === typeof next) {
          next();
        }
        else {
          res.statusCode = 500;
          res.end("[500] Developer Error: app.use('/', le.middleware()) or le.middleware(app)");
        }
        return;
      }

      log(le.debug, "this must be tinder, 'cuz it's a match!");

      var token = req.url.slice(prefix.length);
      var hostname = req.hostname || (req.headers.host || '').toLowerCase().replace(/:.*/, '');

      log(le.debug, "hostname", hostname, "token", token);

      var copy = utils.merge({ domains: [ hostname ] }, le);
      copy = utils.tplCopy(copy);

      // TODO tpl copy?
      // TODO need to restore challengeType
      le.challenges['http-01'].get(copy, hostname, token, function (err, secret) {
        if (err || !token) {
          res.statusCode = 404;
          res.setHeader('Content-Type', 'application/json; charset=utf-8');
          res.end('{ "error": { "message": "Error: These aren\'t the tokens you\'re looking for. Move along." } }');
          return;
        }

        res.setHeader('Content-Type', 'text/plain; charset=utf-8');
        res.end(secret);
      });
    };
  };
}
```
- example usage
```shell
...

### Overly Simplified Example

Against my better judgement I'm providing a terribly oversimplified example
of how to use this library:

'''javascript
var le = require('letsencrypt').create({ server: 'staging' });

var opts = {
domains: ['example.com'], email: 'user@email.com', agreeTos: true
};

le.register(opts).then(function (certs) {
console.log(certs);
...
```



# <a name="apidoc.module.letsencrypt.utils"></a>[module letsencrypt.utils](#apidoc.module.letsencrypt.utils)

#### <a name="apidoc.element.letsencrypt.utils.attachCertInfo"></a>[function <span class="apidocSignatureSpan">letsencrypt.utils.</span>attachCertInfo (results)](#apidoc.element.letsencrypt.utils.attachCertInfo)
- description and source-code
```javascript
attachCertInfo = function (results) {
  // XXX Note: Parsing the certificate info comes at a great cost (~500kb)
  var getCertInfo = require('certpem').info;
  var certInfo = getCertInfo(results.cert);

  // subject, altnames, issuedAt, expiresAt
  Object.keys(certInfo).forEach(function (key) {
    results[key] = certInfo[key];
  });

  return results;
}
```
- example usage
```shell
...
  var copy = utils.merge(args, le);
  utils.tplCopy(copy);

  // returns pems
  return le.store.certificates.checkAsync(copy).then(function (cert) {
    if (cert) {
      log(args.debug, 'checkAsync found existing certificates');
      return utils.attachCertInfo(cert);
    }

    log(args.debug, 'checkAsync failed to find certificates');
    return null;
  });
}
// Certificates
...
```

#### <a name="apidoc.element.letsencrypt.utils.isValidDomain"></a>[function <span class="apidocSignatureSpan">letsencrypt.utils.</span>isValidDomain (domain)](#apidoc.element.letsencrypt.utils.isValidDomain)
- description and source-code
```javascript
isValidDomain = function (domain) {
  if (re.test(domain)) {
    return domain;
  }

  domain = punycode.toASCII(domain);

  if (re.test(domain)) {
    return domain;
  }

  return '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.letsencrypt.utils.merge"></a>[function <span class="apidocSignatureSpan">letsencrypt.utils.</span>merge ()](#apidoc.element.letsencrypt.utils.merge)
- description and source-code
```javascript
merge = function () {
  var allDefaults = Array.prototype.slice.apply(arguments);
  var args = allDefaults.shift();
  var copy = {};

  allDefaults.forEach(function (defaults) {
    Object.keys(defaults).forEach(function (key) {
      copy[key] = defaults[key];
    });
  });

  Object.keys(args).forEach(function (key) {
    copy[key] = args[key];
  });

  return copy;
}
```
- example usage
```shell
...
  le.sni = le.sni || require('le-sni-auto');
  if (le.sni.create) {
    le.sni = le.sni.create(le);
  }
  le.httpsOptions.SNICallback = le.sni.sniCallback;
}
if (!le.httpsOptions.key || !le.httpsOptions.cert) {
  le.httpsOptions = require('localhost.daplie.com-certificates').merge(le.httpsOptions);
}
/*
le.sni = PromiseA.promisifyAll(le.sni);
le._sniOpts = le.sni.getOptions();
Object.keys(le._sniOpts).forEach(function (key) {
  if (!(key in le)) {
    le[key] = le._sniOpts[key];
...
```

#### <a name="apidoc.element.letsencrypt.utils.testEmail"></a>[function <span class="apidocSignatureSpan">letsencrypt.utils.</span>testEmail (email)](#apidoc.element.letsencrypt.utils.testEmail)
- description and source-code
```javascript
testEmail = function (email) {
  var parts = (email||'').split('@');
  var err;

  if (2 !== parts.length || !parts[0] || !parts[1]) {
    err = new Error("malformed email address '" + email + "'");
    err.code = 'E_EMAIL';
    return PromiseA.reject(err);
  }

  return dns.resolveMxAsync(parts[1]).then(function (records) {
    // records only returns when there is data
    if (!records.length) {
      throw new Error("sanity check fail: success, but no MX records returned");
    }
    return email;
  }, function (err) {
    if ('ENODATA' === err.code) {
      err = new Error("no MX records found for '" + parts[1] + "'");
      err.code = 'E_EMAIL';
      return PromiseA.reject(err);
    }
  });
}
```
- example usage
```shell
...
  "In order to register an account both 'email' and 'agreeTos' must be present"
    + " and 'rsaKeySize' must be 2048 or greater."
);
err.code = 'E_ARGS';
return PromiseA.reject(err);
        }

        return utils.testEmail(args.email).then(function () {
var keypairOpts = { public: true, pem: true };

var promise = le.store.accounts.checkKeypairAsync(args).then(function (keypair) {
  if (keypair) {
    return RSA.import(keypair);
  }
...
```

#### <a name="apidoc.element.letsencrypt.utils.tplCopy"></a>[function <span class="apidocSignatureSpan">letsencrypt.utils.</span>tplCopy (copy)](#apidoc.element.letsencrypt.utils.tplCopy)
- description and source-code
```javascript
tplCopy = function (copy) {
  var homedir = require('homedir')();
  var tplKeys;

  copy.hostnameGet = function (copy) {
    return (copy.domains || [])[0] || copy.domain;
  };

  Object.keys(copy).forEach(function (key) {
    var newName;
    if (!/Get$/.test(key)) {
      return;
    }

    newName = key.replace(/Get$/, '');
    copy[newName] = copy[newName] || copy[key](copy);
  });

  tplKeys = Object.keys(copy);
  tplKeys.sort(function (a, b) {
    return b.length - a.length;
  });

  tplKeys.forEach(function (key) {
    if ('string' !== typeof copy[key]) {
      return;
    }

    copy[key] = copy[key].replace(homeRe, homedir + path.sep);
  });

  tplKeys.forEach(function (key) {
    if ('string' !== typeof copy[key]) {
      return;
    }

    tplKeys.forEach(function (tplname) {
      if (!copy[tplname]) {
        // what can't be templated now may be templatable later
        return;
      }
      copy[key] = copy[key].replace(':' + tplname, copy[tplname]);
    });
  });

  return copy;
}
```
- example usage
```shell
...
    //
  , accounts: {
      // Accounts
      registerAsync: function (args) {
var err;
var copy = utils.merge(args, le);
var disagreeTos;
args = utils.tplCopy(copy);

disagreeTos = (!args.agreeTos && 'undefined' !== typeof args.agreeTos);
if (!args.email || disagreeTos || (parseInt(args.rsaKeySize, 10) < 2048)) {
  err = new Error(
    "In order to register an account both 'email' and 'agreeTos' must be present"
      + " and 'rsaKeySize' must be 2048 or greater."
  );
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
