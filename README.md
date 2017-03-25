# api documentation for  [cron (v1.2.1)](https://github.com/ncb000gt/node-cron#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cron.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cron)
#### Cron jobs for your node

[![NPM](https://nodei.co/npm/cron.png?downloads=true)](https://www.npmjs.com/package/cron)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cron/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-cron_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cron/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-cron/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Nick Campbell",
        "email": "nicholas.j.campbell@gmail.com",
        "url": "http://github.com/ncb000gt"
    },
    "bugs": {
        "url": "http://github.com/ncb000gt/node-cron/issues"
    },
    "contributors": [
        {
            "name": "Romain Beauxis",
            "email": "toots@rastageeks.org",
            "url": "https://github.com/toots"
        },
        {
            "name": "James Padolsey",
            "url": "https://github.com/jamespadolsey"
        },
        {
            "name": "Finn Herpich",
            "email": "fh@three-heads.de",
            "url": "https://github.com/ErrorProne"
        },
        {
            "name": "Clifton Cunningham",
            "email": "clifton.cunningham@gmail.com",
            "url": "https://github.com/cliftonc"
        },
        {
            "name": "Eric Abouaf",
            "email": "eric.abouaf@gmail.com",
            "url": "https://github.com/neyric"
        },
        {
            "name": "humanchimp",
            "email": "morphcham@gmail.com",
            "url": "https://github.com/humanchimp"
        },
        {
            "name": "Craig Condon",
            "email": "craig@spiceapps.com",
            "url": "https://github.com/spiceapps"
        },
        {
            "name": "Dan Bear",
            "email": "daniel@hulu.com",
            "url": "https://github.com/danhbear"
        },
        {
            "name": "Vadim Baryshev",
            "email": "vadimbaryshev@gmail.com",
            "url": "https://github.com/baryshev"
        },
        {
            "name": "Leandro Ferrari",
            "email": "lfthomaz@gmail.com",
            "url": "https://github.com/lfthomaz"
        },
        {
            "name": "Gregg Zigler",
            "email": "greggzigler@gmail.com",
            "url": "https://github.com/greggzigler"
        },
        {
            "name": "Jordan Abderrachid",
            "email": "jabderrachid@gmail.com",
            "url": "https://github.com/jordanabderrachid"
        }
    ],
    "dependencies": {
        "moment-timezone": "^0.5.x"
    },
    "description": "Cron jobs for your node",
    "devDependencies": {
        "chai": "~3.4.0",
        "mocha": "~2.3.3",
        "sinon": "~1.12.x"
    },
    "directories": {},
    "dist": {
        "shasum": "3a86c09b41b8f261ac863a7cc85ea4735857eab2",
        "tarball": "https://registry.npmjs.org/cron/-/cron-1.2.1.tgz"
    },
    "gitHead": "c81322184d77a9c97e4eab51371a198c2750ea51",
    "homepage": "https://github.com/ncb000gt/node-cron#readme",
    "license": "MIT",
    "main": "lib/cron",
    "maintainers": [
        {
            "name": "ncb000gt",
            "email": "nicholas.j.campbell@gmail.com"
        }
    ],
    "name": "cron",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/ncb000gt/node-cron.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "1.2.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module cron](#apidoc.module.cron)
1.  [function <span class="apidocSignatureSpan">cron.</span>CronJob (cronTime, onTick, onComplete, startNow, timeZone, context, runOnInit)](#apidoc.element.cron.CronJob)
1.  [function <span class="apidocSignatureSpan">cron.</span>CronTime (source, zone)](#apidoc.element.cron.CronTime)
1.  [function <span class="apidocSignatureSpan">cron.</span>job (cronTime, onTick, onComplete)](#apidoc.element.cron.job)
1.  [function <span class="apidocSignatureSpan">cron.</span>sendAt (cronTime)](#apidoc.element.cron.sendAt)
1.  [function <span class="apidocSignatureSpan">cron.</span>time (cronTime, timeZone)](#apidoc.element.cron.time)
1.  [function <span class="apidocSignatureSpan">cron.</span>timeout (cronTime)](#apidoc.element.cron.timeout)
1.  object <span class="apidocSignatureSpan">cron.</span>CronJob.prototype
1.  object <span class="apidocSignatureSpan">cron.</span>CronTime.prototype

#### [module cron.CronJob](#apidoc.module.cron.CronJob)
1.  [function <span class="apidocSignatureSpan">cron.</span>CronJob (cronTime, onTick, onComplete, startNow, timeZone, context, runOnInit)](#apidoc.element.cron.CronJob.CronJob)

#### [module cron.CronJob.prototype](#apidoc.module.cron.CronJob.prototype)
1.  [function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>addCallback (callback)](#apidoc.element.cron.CronJob.prototype.addCallback)
1.  [function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>fireOnTick ()](#apidoc.element.cron.CronJob.prototype.fireOnTick)
1.  [function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>lastDate ()](#apidoc.element.cron.CronJob.prototype.lastDate)
1.  [function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>nextDate ()](#apidoc.element.cron.CronJob.prototype.nextDate)
1.  [function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>nextDates (i)](#apidoc.element.cron.CronJob.prototype.nextDates)
1.  [function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>setTime (time)](#apidoc.element.cron.CronJob.prototype.setTime)
1.  [function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>start ()](#apidoc.element.cron.CronJob.prototype.start)
1.  [function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>stop ()](#apidoc.element.cron.CronJob.prototype.stop)

#### [module cron.CronTime](#apidoc.module.cron.CronTime)
1.  [function <span class="apidocSignatureSpan">cron.</span>CronTime (source, zone)](#apidoc.element.cron.CronTime.CronTime)
1.  object <span class="apidocSignatureSpan">cron.CronTime.</span>aliases
1.  object <span class="apidocSignatureSpan">cron.CronTime.</span>constraints
1.  object <span class="apidocSignatureSpan">cron.CronTime.</span>monthConstraints
1.  object <span class="apidocSignatureSpan">cron.CronTime.</span>parseDefaults

#### [module cron.CronTime.prototype](#apidoc.module.cron.CronTime.prototype)
1.  [function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_findDST (date)](#apidoc.element.cron.CronTime.prototype._findDST)
1.  [function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_getNextDateFrom (start)](#apidoc.element.cron.CronTime.prototype._getNextDateFrom)
1.  [function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_hasAll (type)](#apidoc.element.cron.CronTime.prototype._hasAll)
1.  [function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_parse ()](#apidoc.element.cron.CronTime.prototype._parse)
1.  [function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_parseField (field, type, constraints)](#apidoc.element.cron.CronTime.prototype._parseField)
1.  [function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_verifyParse ()](#apidoc.element.cron.CronTime.prototype._verifyParse)
1.  [function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_wcOrAll (type)](#apidoc.element.cron.CronTime.prototype._wcOrAll)
1.  [function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>getTimeout ()](#apidoc.element.cron.CronTime.prototype.getTimeout)
1.  [function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>sendAt (i)](#apidoc.element.cron.CronTime.prototype.sendAt)
1.  [function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>toJSON ()](#apidoc.element.cron.CronTime.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>toString ()](#apidoc.element.cron.CronTime.prototype.toString)



# <a name="apidoc.module.cron"></a>[module cron](#apidoc.module.cron)

#### <a name="apidoc.element.cron.CronJob"></a>[function <span class="apidocSignatureSpan">cron.</span>CronJob (cronTime, onTick, onComplete, startNow, timeZone, context, runOnInit)](#apidoc.element.cron.CronJob)
- description and source-code
```javascript
function CronJob(cronTime, onTick, onComplete, startNow, timeZone, context, runOnInit) {
	var _cronTime = cronTime;
	if (typeof cronTime != 'string' && arguments.length == 1) {
		//crontime is an object...
		onTick = cronTime.onTick;
		onComplete = cronTime.onComplete;
		context = cronTime.context;
		startNow = cronTime.start || cronTime.startNow || cronTime.startJob;
		timeZone = cronTime.timeZone;
		runOnInit = cronTime.runOnInit;
		_cronTime = cronTime.cronTime;
	}

	this.context = (context || this);
	this._callbacks = [];
	this.onComplete = command2function(onComplete);
	this.cronTime = new CronTime(_cronTime, timeZone);

	addCallback.call(this, command2function(onTick));

	if (runOnInit) fireOnTick.call(this);
	if (startNow) start.call(this);

	return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronTime"></a>[function <span class="apidocSignatureSpan">cron.</span>CronTime (source, zone)](#apidoc.element.cron.CronTime)
- description and source-code
```javascript
function CronTime(source, zone) {
	this.source = source;

	if (zone) {
		if (moment.tz.names().indexOf(zone) === -1) {
			throw new Error('Invalid timezone.');
		}

		this.zone = zone;
	}

	var that = this;
	timeUnits.map(function(timeUnit){
		that[timeUnit] = {};
	});

	if (this.source instanceof Date) {
		this.source = moment(this.source);
		this.realDate = true;
	} else {
		this._parse();
		this._verifyParse();
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.job"></a>[function <span class="apidocSignatureSpan">cron.</span>job (cronTime, onTick, onComplete)](#apidoc.element.cron.job)
- description and source-code
```javascript
job = function (cronTime, onTick, onComplete) {
	return new CronJob(cronTime, onTick, onComplete);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.sendAt"></a>[function <span class="apidocSignatureSpan">cron.</span>sendAt (cronTime)](#apidoc.element.cron.sendAt)
- description and source-code
```javascript
sendAt = function (cronTime) {
	return exports.time(cronTime).sendAt();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.time"></a>[function <span class="apidocSignatureSpan">cron.</span>time (cronTime, timeZone)](#apidoc.element.cron.time)
- description and source-code
```javascript
time = function (cronTime, timeZone) {
	return new CronTime(cronTime, timeZone);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.timeout"></a>[function <span class="apidocSignatureSpan">cron.</span>timeout (cronTime)](#apidoc.element.cron.timeout)
- description and source-code
```javascript
timeout = function (cronTime) {
	return exports.time(cronTime).getTimeout();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cron.CronJob"></a>[module cron.CronJob](#apidoc.module.cron.CronJob)

#### <a name="apidoc.element.cron.CronJob.CronJob"></a>[function <span class="apidocSignatureSpan">cron.</span>CronJob (cronTime, onTick, onComplete, startNow, timeZone, context, runOnInit)](#apidoc.element.cron.CronJob.CronJob)
- description and source-code
```javascript
function CronJob(cronTime, onTick, onComplete, startNow, timeZone, context, runOnInit) {
	var _cronTime = cronTime;
	if (typeof cronTime != 'string' && arguments.length == 1) {
		//crontime is an object...
		onTick = cronTime.onTick;
		onComplete = cronTime.onComplete;
		context = cronTime.context;
		startNow = cronTime.start || cronTime.startNow || cronTime.startJob;
		timeZone = cronTime.timeZone;
		runOnInit = cronTime.runOnInit;
		_cronTime = cronTime.cronTime;
	}

	this.context = (context || this);
	this._callbacks = [];
	this.onComplete = command2function(onComplete);
	this.cronTime = new CronTime(_cronTime, timeZone);

	addCallback.call(this, command2function(onTick));

	if (runOnInit) fireOnTick.call(this);
	if (startNow) start.call(this);

	return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cron.CronJob.prototype"></a>[module cron.CronJob.prototype](#apidoc.module.cron.CronJob.prototype)

#### <a name="apidoc.element.cron.CronJob.prototype.addCallback"></a>[function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>addCallback (callback)](#apidoc.element.cron.CronJob.prototype.addCallback)
- description and source-code
```javascript
addCallback = function (callback) {
	if (typeof callback == 'function') this._callbacks.push(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronJob.prototype.fireOnTick"></a>[function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>fireOnTick ()](#apidoc.element.cron.CronJob.prototype.fireOnTick)
- description and source-code
```javascript
fireOnTick = function () {
	for (var i = (this._callbacks.length - 1); i >= 0; i--)
		this._callbacks[i].call(this.context, this.onComplete);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronJob.prototype.lastDate"></a>[function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>lastDate ()](#apidoc.element.cron.CronJob.prototype.lastDate)
- description and source-code
```javascript
lastDate = function (){
	return this.lastExecution;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronJob.prototype.nextDate"></a>[function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>nextDate ()](#apidoc.element.cron.CronJob.prototype.nextDate)
- description and source-code
```javascript
nextDate = function () {
	return this.cronTime.sendAt();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronJob.prototype.nextDates"></a>[function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>nextDates (i)](#apidoc.element.cron.CronJob.prototype.nextDates)
- description and source-code
```javascript
nextDates = function (i) {
	return this.cronTime.sendAt(i);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronJob.prototype.setTime"></a>[function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>setTime (time)](#apidoc.element.cron.CronJob.prototype.setTime)
- description and source-code
```javascript
setTime = function (time) {
	if (!(time instanceof CronTime)) throw new Error('\'time\' must be an instance of CronTime.');
	this.stop();
	this.cronTime = time;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronJob.prototype.start"></a>[function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>start ()](#apidoc.element.cron.CronJob.prototype.start)
- description and source-code
```javascript
start = function () {
	if (this.running) return;

	var MAXDELAY = 2147483647; // The maximum number of milliseconds setTimeout will wait.
	var self = this;
	var timeout = this.cronTime.getTimeout();
	var remaining = 0;
	var startTime;

	if (this.cronTime.realDate) this.runOnce = true;

	function _setTimeout(timeout) {
		startTime = Date.now();
		self._timeout = setTimeout(callbackWrapper, timeout);
	}

	// The callback wrapper checks if it needs to sleep another period or not
	// and does the real callback logic when it's time.

	function callbackWrapper() {
		var diff = startTime + timeout - Date.now();

		if (diff > 0) {
			var newTimeout = self.cronTime.getTimeout();

			if (newTimeout > diff) {
				newTimeout = diff;
			}

			remaining += newTimeout;
		}

		// If there is sleep time remaining, calculate how long and go to sleep
		// again. This processing might make us miss the deadline by a few ms
		// times the number of sleep sessions. Given a MAXDELAY of almost a
		// month, this should be no issue.

		self.lastExecution = new Date();
		if (remaining) {
			if (remaining > MAXDELAY) {
				remaining -= MAXDELAY;
				timeout = MAXDELAY;
			} else {
				timeout = remaining;
				remaining = 0;
			}

			_setTimeout(timeout);
		} else {

			// We have arrived at the correct point in time.

			self.running = false;

			//start before calling back so the callbacks have the ability to stop the cron job
			if (!(self.runOnce)) self.start();

			self.fireOnTick();
			//for (var i = (self._callbacks.length - 1); i >= 0; i--)
				//self._callbacks[i].call(self.context, self.onComplete);
		}
	}

	if (timeout >= 0) {
		this.running = true;

		// Don't try to sleep more than MAXDELAY ms at a time.

		if (timeout > MAXDELAY) {
			remaining = timeout - MAXDELAY;
			timeout = MAXDELAY;
		}

		_setTimeout(timeout);
	} else {
		this.stop();
	}
}
```
- example usage
```shell
...
     * at 11:30:00 AM. It does not run on Saturday
     * or Sunday.
     */
  },
  start: false,
  timeZone: 'America/Los_Angeles'
});
job.start();
'''


How to check if a cron pattern is valid:
==========

'''javascript
...
```

#### <a name="apidoc.element.cron.CronJob.prototype.stop"></a>[function <span class="apidocSignatureSpan">cron.CronJob.prototype.</span>stop ()](#apidoc.element.cron.CronJob.prototype.stop)
- description and source-code
```javascript
stop = function () {
	if (this._timeout)
		clearTimeout(this._timeout);
	this.running = false;
	if (typeof this.onComplete == 'function') this.onComplete();
}
```
- example usage
```shell
...

* 'constructor(cronTime, onTick, onComplete, start, timezone, context, runOnInit)' - Of note, the first parameter here can be a
JSON object that has the below names and associated types (see examples above).
  * 'cronTime' - [REQUIRED] - The time to fire off your job. This can be in the form of cron syntax or a JS [Date](https://developer
.mozilla.org/en/JavaScript/Reference/Global_Objects/Date) object.
  * 'onTick' - [REQUIRED] - The function to fire at the specified time.
  * 'onComplete' - [OPTIONAL] - A function that will fire when the job is complete, when it is stopped.
  * 'start' - [OPTIONAL] - Specifies whether to start the job just before exiting the constructor. By default this is set to false
. If left at default you will need to call 'job.start()' in order to start the job (assuming 'job' is the variable you set the cronjob
 to). This does not immediately fire your 'onTick' function, it just gives you more control over the behavior of your jobs.
  * 'timeZone' - [OPTIONAL] - Specify the timezone for the execution. This will modify the actual time relative to your timezone
. If the timezone is invalid, an error is thrown.
  * 'context' - [OPTIONAL] - The context within which to execute the onTick method. This defaults to the cronjob itself allowing
 you to call 'this.stop()'. However, if you change this you'll have access to the functions and values within your context object
.
  * 'runOnInit' - [OPTIONAL] - This will immediately fire your 'onTick' function as soon as the requisit initialization has happened
. This option is set to 'false' by default for backwards compatability.
* 'start' - Runs your job.
* 'stop' - Stops your job.

'CronTime'

* 'constructor(time)'
...
```



# <a name="apidoc.module.cron.CronTime"></a>[module cron.CronTime](#apidoc.module.cron.CronTime)

#### <a name="apidoc.element.cron.CronTime.CronTime"></a>[function <span class="apidocSignatureSpan">cron.</span>CronTime (source, zone)](#apidoc.element.cron.CronTime.CronTime)
- description and source-code
```javascript
function CronTime(source, zone) {
	this.source = source;

	if (zone) {
		if (moment.tz.names().indexOf(zone) === -1) {
			throw new Error('Invalid timezone.');
		}

		this.zone = zone;
	}

	var that = this;
	timeUnits.map(function(timeUnit){
		that[timeUnit] = {};
	});

	if (this.source instanceof Date) {
		this.source = moment(this.source);
		this.realDate = true;
	} else {
		this._parse();
		this._verifyParse();
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cron.CronTime.prototype"></a>[module cron.CronTime.prototype](#apidoc.module.cron.CronTime.prototype)

#### <a name="apidoc.element.cron.CronTime.prototype._findDST"></a>[function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_findDST (date)](#apidoc.element.cron.CronTime.prototype._findDST)
- description and source-code
```javascript
_findDST = function (date) {
		var newDate = moment(date);
		while (newDate <= date)
			newDate.add(1, 's');

		return newDate;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronTime.prototype._getNextDateFrom"></a>[function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_getNextDateFrom (start)](#apidoc.element.cron.CronTime.prototype._getNextDateFrom)
- description and source-code
```javascript
_getNextDateFrom = function (start) {
		var date = moment(start);
		if (date.toString() == 'Invalid date') {
			console.log('ERROR: You specified an invalid date.');
			return date;
		}
		if (this.realDate && start < new Date())
			console.log('WARNING: Date in past. Will never be fired.');
		if (this.realDate) return date;

		//sanity check
		while (true) {
			var diff = date - start,
				origDate = new Date(date);

			if (!(date.month() in this.month)) {
				date.add(1, 'M');
				date.date(1);
				date.hours(0);
				date.minutes(0);
				date.seconds(0);
				continue;
			}

			if (!(date.date() in this.dayOfMonth)) {
				date.add(1, 'd');
				date.hours(0);
				date.minutes(0);
				date.seconds(0);
				continue;
			}

			if (!(date.day() in this.dayOfWeek)) {
				date.add(1, 'd');
				date.hours(0);
				date.minutes(0);
				date.seconds(0);
				if (date <= origDate) {
					date = this._findDST(origDate);
				}
				continue;
			}

			if (!(date.hours() in this.hour)) {
				origDate = moment(date);
				date.hours(date.hours() == 23 && diff > 86400000 ? 0 : date.hours() + 1);
				date.minutes(0);
				date.seconds(0);
				if (date <= origDate) {
					date = this._findDST(origDate);
				}
				continue;
			}

			if (!(date.minutes() in this.minute)) {
				origDate = moment(date);
				date.minutes(date.minutes() == 59 && diff > 60 * 60 * 1000 ? 0 : date.minutes() + 1);
				date.seconds(0);
				if (date <= origDate) {
					date = this._findDST(origDate);
				}
				continue;
			}

			if (!(date.seconds() in this.second)) {
				origDate = moment(date);
				date.seconds(date.seconds() == 59 && diff > 60 * 1000 ? 0 : date.seconds() + 1);
				if (date <= origDate) {
					date = this._findDST(origDate);
				}
				continue;
			}

			break;
		}

		return date;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronTime.prototype._hasAll"></a>[function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_hasAll (type)](#apidoc.element.cron.CronTime.prototype._hasAll)
- description and source-code
```javascript
_hasAll = function (type) {
		var constrain = CronTime.constraints[timeUnits.indexOf(type)];

		for (var i = constrain[0], n = constrain[1]; i < n; i++) {
			if (!(i in this[type])) return false;
		}

		return true;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronTime.prototype._parse"></a>[function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_parse ()](#apidoc.element.cron.CronTime.prototype._parse)
- description and source-code
```javascript
_parse = function () {
		var aliases = CronTime.aliases,
		source = this.source.replace(/[a-z]{1,3}/ig, function(alias) {
			alias = alias.toLowerCase();

			if (alias in aliases) {
				return aliases[alias];
			}

			throw new Error('Unknown alias: ' + alias);
		}),
		split = source.replace(/^\s\s*|\s\s*$/g, '').split(/\s+/),
		cur, i = 0,
		len = timeUnits.length;

		for (; i < timeUnits.length; i++) {
			// If the split source string doesn't contain all digits,
			// assume defaults for first n missing digits.
			// This adds support for 5-digit standard cron syntax
			cur = split[i - (len - split.length)] || CronTime.parseDefaults[i];
			this._parseField(cur, timeUnits[i], CronTime.constraints[i]);
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronTime.prototype._parseField"></a>[function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_parseField (field, type, constraints)](#apidoc.element.cron.CronTime.prototype._parseField)
- description and source-code
```javascript
_parseField = function (field, type, constraints) {
		var rangePattern = /^(\d+)(?:-(\d+))?(?:\/(\d+))?$/g,
		typeObj = this[type],
		pointer,
		low = constraints[0],
		high = constraints[1];

		// * is a shortcut to [lower-upper] range
		field = field.replace(/\*/g, low + '-' + high);

		//commas separate information, so split based on those
		var allRanges = field.split(',');

		for (var i = 0; i < allRanges.length; i++) {
			if (allRanges[i].match(rangePattern)) {
				allRanges[i].replace(rangePattern, function($0, lower, upper, step) {
					step = parseInt(step) || 1;
					// Positive integer higher than constraints[0]
					lower = Math.min(Math.max(low, ~~Math.abs(lower)), high);

					// Positive integer lower than constraints[1]
					upper = upper ? Math.min(high, ~~Math.abs(upper)) : lower;

					// Count from the lower barrier to the upper
					pointer = lower;

					do {
						typeObj[pointer] = true
						pointer += step;
					} while (pointer <= upper);
				});
			} else {
				throw new Error('Field (' + field + ') cannot be parsed');
			}
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronTime.prototype._verifyParse"></a>[function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_verifyParse ()](#apidoc.element.cron.CronTime.prototype._verifyParse)
- description and source-code
```javascript
_verifyParse = function () {
		var months = Object.keys(this.month);
		for (var i = 0; i < months.length; i++) {
			var m = months[i];
			var con = CronTime.monthConstraints[parseInt(m, 10)];
			var ok = false;
			var dsom = Object.keys(this.dayOfMonth);
			for (var j = 0; j < dsom.length; j++) {
				var dom = dsom[j];
				if (dom <= con)
					ok = true;
			}

			if (!ok) {
				console.warn('Month \'' + m + '\' is limited to \'' + con + '\' days.');
			}
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronTime.prototype._wcOrAll"></a>[function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>_wcOrAll (type)](#apidoc.element.cron.CronTime.prototype._wcOrAll)
- description and source-code
```javascript
_wcOrAll = function (type) {
		if (this._hasAll(type)) return '*';

		var all = [];
		for (var time in this[type]) {
			all.push(time);
		}

		return all.join(',');
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronTime.prototype.getTimeout"></a>[function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>getTimeout ()](#apidoc.element.cron.CronTime.prototype.getTimeout)
- description and source-code
```javascript
getTimeout = function () {
		return Math.max(-1, this.sendAt() - moment());
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronTime.prototype.sendAt"></a>[function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>sendAt (i)](#apidoc.element.cron.CronTime.prototype.sendAt)
- description and source-code
```javascript
sendAt = function (i) {
		var date = this.realDate ? this.source : moment();
		// Set the timezone if given (http://momentjs.com/timezone/docs/#/using-timezones/parsing-in-zone/)
		if (this.zone)
			date = date.tz(this.zone);

		if (this.realDate)
			return date;

		//add 1 second so next time isn't now (can cause timeout to be 0 or negative number)
		var now = new Date();
		var targetSecond = date.seconds();
		var diff = Math.abs(targetSecond - now.getSeconds())
		// there was a problem when 'date' is 1424777177999 and 'now' is 1424777178000
		// 1 ms diff but this is another second...
		if ( diff == 0 || (diff == 1 && now.getMilliseconds() <= date.milliseconds() ) ) {
			//console.log('add 1 second?');
			date = date.add(1, 's');
		}

		//If the i argument is not given, return the next send time
		if(isNaN(i) || i < 0){
			date = this._getNextDateFrom(date);
			return date;
		}
		//Else return the next i send times
		else{
			var dates = [];
			for(;i>0;i--){
				date = this._getNextDateFrom(date);
				dates.push(moment(date));
				if(i>1) date.add(1,'s');
			}
			return dates;
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronTime.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>toJSON ()](#apidoc.element.cron.CronTime.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
		var self = this;
		return timeUnits.map(function(timeName){
			return self._wcOrAll(timeName);
		});
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cron.CronTime.prototype.toString"></a>[function <span class="apidocSignatureSpan">cron.CronTime.prototype.</span>toString ()](#apidoc.element.cron.CronTime.prototype.toString)
- description and source-code
```javascript
toString = function () {
		return this.toJSON().join(' ');
	}
```
- example usage
```shell
...




var Job = require('./lib/cron').CronJob;

new Job('*/2 * * * * *', function() {
  console.log(new Date().toString()); }
).start();
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
