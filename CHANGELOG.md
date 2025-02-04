<a name="v1.19.0"></a>
### v1.19.0 (2019-06-25)


#### Features

* **hal client**
  * update from pact-ruby	 ([f8b3432](/../../commit/f8b3432))

* update pact with broker for scenario where version does not exist	 ([27b744f](/../../commit/27b744f))


#### Bug Fixes

* **create webhook**
  * pass in token from command line	 ([9d3170e](/../../commit/9d3170e))

* correct pact merge error message	 ([5ebe808](/../../commit/5ebe808))


<a name="v1.18.0"></a>
### v1.18.0 (2019-03-05)


#### Features

* remove 'no data' message when there are no rows.	 ([b0246a2](/../../commit/b0246a2))
* allow for broker token to be used	 ([3266bc1](/../../commit/3266bc1))
* add broker token to cli	 ([e342c29](/../../commit/e342c29))


<a name="v1.17.0"></a>
### v1.17.0 (2018-11-15)


#### Features

* update HAL client from pact codebase	 ([ed77fe0](/../../commit/ed77fe0))


<a name="v1.16.0"></a>
### v1.16.0 (2018-07-09)


#### Features

* add retries to can-i-deploy to allow the command to wait for missing results to arrive	 ([e44f88d](/../../commit/e44f88d))


<a name="v1.15.1"></a>
### v1.15.1 (2018-06-28)


#### Bug Fixes

* declare dependency on rake in gemspec	 ([b24bbcd](/../../commit/b24bbcd))


<a name="v1.15.0"></a>
### v1.15.0 (2018-06-22)


#### Features

* allow webhooks with optional consumer and provider to be created using the create-webhooks CLI	 ([c6763b0](/../../commit/c6763b0))
* update expectation of error response	 ([d45244f](/../../commit/d45244f))
* add create-webhook to CLI	 ([e1ec885](/../../commit/e1ec885))
* add title, name and title_or_name methods to Link	 ([dc24caa](/../../commit/dc24caa))
* add http debug logging for create environment call	 ([5f31fcb](/../../commit/5f31fcb))
* add hal client	 ([4d93bf9](/../../commit/4d93bf9))
* update pacts relation name in retrieve pacts query	 ([7d965bf](/../../commit/7d965bf))


#### Bug Fixes

* correctly escape expanded URL links	 ([d6dbce8](/../../commit/d6dbce8))
* correct accept headers for requests to the pact broker	 ([415d9d5](/../../commit/415d9d5))


<a name="v1.14.1"></a>
### v1.14.1 (2018-04-11)


#### Bug Fixes

* use SSL_CERT_FILE and SSL_CERT_DIR environment variables for https connections	 ([e4e7a15](/../../commit/e4e7a15))


<a name="v1.14.0"></a>
### v1.14.0 (2018-01-25)


#### Features

* **describe-version**
  * allow retrieving latest pacticipant version	 ([7679f61](/../../commit/7679f61))

* update help text for can-i-deploy	 ([7d3f3e1](/../../commit/7d3f3e1))
* add example showing how to use can-i-deploy and describe-version as a verification webhook endpoint	 ([ec83387](/../../commit/ec83387))

* **cli**
  * add describe-version	 ([6e12478](/../../commit/6e12478))
  * output HTTP request and response debugging when verbose mode enabled	 ([f487714](/../../commit/f487714))


<a name="v1.13.0"></a>
### v1.13.0 (2017-11-09)


#### Features

* **can-i-deploy**
  * allow pacticipant version to be checked against latest tagged versions of all the other pacticipants	 ([7f10e13](/../../commit/7f10e13))


#### Bug Fixes

* **publish**
  * accept pact file paths using windows separator	 ([5ee9dd7](/../../commit/5ee9dd7))


<a name="v1.12.0"></a>
### v1.12.0 (2017-11-06)


#### Features

* **publish**
  * expose tag_with_git_branch in rake publication task	 ([f28d9ad](/../../commit/f28d9ad))

* **can-i-deploy**
  * shorten header names in text output	 ([89d5a04](/../../commit/89d5a04))
  * support invocation with only one pacticipant/version provided	 ([3d799cc](/../../commit/3d799cc))


<a name="v1.11.0"></a>
### v1.11.0 (2017-11-01)


#### Features

* **can-i-deploy**
  * add --latest option to command line	 ([c7f012d](/../../commit/c7f012d))

* allow broker base url, username and password to be set by environment variables	 ([3516103](/../../commit/3516103))

* **cli**
  * add one line of backtrace to error output	 ([c2ede03](/../../commit/c2ede03))

* **create-version-tag**
  * add CLI to tag a pacticipant version	 ([c62d9b8](/../../commit/c62d9b8))


<a name="v1.10.0"></a>
### v1.10.0 (2017-10-31)


#### Features

* **can-i-deploy**
  * print out matrix summary 'reason'	 ([aa25e16](/../../commit/aa25e16))


<a name="v1.9.0"></a>
### v1.9.0 (2017-10-30)


#### Features

* **cli**
  * add option to --tag-with-git-branch when publishing pacts	 ([484d5b8](/../../commit/484d5b8))

* **can-i-deploy**
  * raise error when no --version is supplied for a --pacticipant	 ([0f3bfea](/../../commit/0f3bfea))
  * change --name to --pacticipant	 ([d5d23bc](/../../commit/d5d23bc))
  * include full response body in json output	 ([216bfdc](/../../commit/216bfdc))
  * use array of query params for matrix	 ([314e2e2](/../../commit/314e2e2))

* **what-can-i-deploy**
  * add success param to matrix query	 ([40adb2e](/../../commit/40adb2e))

* handle hash of errors in response	 ([fff32c2](/../../commit/fff32c2))
* change query params for matrix to use pacticipant[]=? and version[]=?	 ([003e305](/../../commit/003e305))


#### Bug Fixes

* **can-i-deploy**
  * correct provider name in text output	 ([bfd0882](/../../commit/bfd0882))


<a name="v1.8.0"></a>
### v1.8.0 (2017-10-19)

#### Features

* renamed `pact-publish` command to `pact-broker publish`	 ([ed7d23a](/../../commit/ed7d23a))

#### Bug Fixes

* **pact-publish**
  * ensure process exits with a status 1 when error is raised	 ([800f5cd](/../../commit/800f5cd))

<a name="v1.7.0"></a>
### v1.7.0 (2017-10-19)


#### Features

* **can-i-deploy**
  * change cli to use --name and --version options instead of bespoke version selector format	 ([15e8131](/../../commit/15e8131))
  * puts output to stdout for both success and failure scenarios so that JSON output can be parsed by capturing stdout	 ([6db595a](/../../commit/6db595a))
  * remove dates from table output and add success status	 ([5dc9484](/../../commit/5dc9484))
  * add --output option allowing table or json to be specified	 ([57fa24e](/../../commit/57fa24e))

* changed name of verification date field	 ([962b7d1](/../../commit/962b7d1))
* output table of verification results when present	 ([9220703](/../../commit/9220703))
* add 'pact-broker can-i-deploy' executable	 ([ca68c54](/../../commit/ca68c54))


<a name="v1.6.0"></a>
### v1.6.0 (2017-10-01)

#### BREAKING CHANGES

* **cli**
  * change cli option names to match pact-provider-verifier	 ([0682662](/../../commit/0682662))

<a name="v1.5.0"></a>
### v1.5.0 (2017-09-28)

#### Features

* **cli**
  * add command line tool to publish pacts   ([d031b98](/../../commit/d031b98))

* **publish pacts**
  * merge pact files with same consumer/provider before publishing   ([1c039a0](/../../commit/1c039a0))

<a name="v1.4.0"></a>
### v1.4.0 (2017-09-07)

#### Features

* **tagging**
  * url escape tag names	 ([8335978](/../../commit/8335978))
  * allow multiple tags to be specified for a version	 ([5f862fe](/../../commit/5f862fe))

#### v1.3.0 (2017-07-03)
* 138a042 - feat(tag): Added tag to PublicationTask (Beth Skurrie, Mon Jul 3 11:45:24 2017 +1000)

#### 1.2.0 (2016-11-23)
* 08e6025 - Fixed broken spec - expected hal+json (Bethany Skurrie, Wed Nov 23 09:20:39 2016 +1100)
* ec4b7d7 - Added Travis badge. (Beth Skurrie, Wed Nov 23 09:16:10 2016 +1100)
* ff133f2 - Adding appraisals and updating test matrix (Bethany Skurrie, Wed Nov 23 09:10:40 2016 +1100)
* e79eec6 - Add hal+json to list of accepted content types (Steve Pletcher, Wed Sep 21 10:27:20 2016 -0400)
* 314f059 - add the option to retrieve all the latest (tagged) pacts for a provider (Olga Vasylchenko, Mon Nov 21 15:01:09 2016 +0100)

#### 1.1.0 (2016-08-19)
* b5ea1b3 - Add support for publishing pacts via patch request (Steve Pletcher, Fri Aug 5 11:16:18 2016 -0400)

#### 1.0.3 (2016-06-27)

* 04bd518 - Clarify that pact_broker-client will only work with ruby >= 2.0 (Sergei Matheson, Mon Jun 27 11:17:57 2016 +1000)

#### 1.0.2 (2016-06-20)

* 4637978 - Warn on overwritting (Taiki Ono, Mon Jun 6 14:50:37 2016 +0900)

#### 1.0.1 (2016-04-29)

* 72c099b - Add release instructions (Sergei Matheson, Fri Apr 29 11:54:01 2016 +1000)
* 12f0054 - :headers is duplicated and overwritten (Taiki Ono, Tue Mar 15 21:46:23 2016 +0900)
* e9251f7 - Commit pact files (Taiki Ono, Tue Mar 15 21:30:15 2016 +0900)
* 0278731 - Loosen content type header expectation (Taiki Ono, Tue Mar 15 21:26:03 2016 +0900)
* fff1838 - Remove `Gemfile.lock` and do not check-in (Taiki Ono, Sun Mar 13 21:49:36 2016 +0900)
* 48c1434 - Add Travis CI setting not to test with ruby1.9 (Taiki Ono, Sun Mar 13 21:17:11 2016 +0900)
* 0365b94 - Updated to RSpec 3 syntax (Beth, Mon Oct 19 08:54:48 2015 +1100)

#### 1.0.0 (2014-10-09)

* 2c08da2 - added pact_broker_basic_auth options to publish task (lifei zhou, Fri Feb 27 21:33:09 2015 +1100)
* 1b84a54 - Updated pact-version rel name (Beth, Mon Dec 22 11:30:57 2014 +1100)
* 04c1e4e - Updated link rels (Beth, Thu Dec 11 14:32:27 2014 +1100)
* d1b2cad - Correcting pact publish message (Beth Skurrie, Mon Aug 25 07:15:57 2014 +1000)
* 6b1d147 - Added backwards compatibility for pact broker publish response (Beth Skurrie, Sun Aug 24 17:50:16 2014 +1000)
* 8c8aa89 - Added location of latest pact to output of pact:publish (Beth Skurrie, Sun Aug 24 17:43:02 2014 +1000)
* e6b56d0 - Added retries for pact publishing (Beth Skurrie, Sun Aug 24 16:55:10 2014 +1000)
* 27c00e5 - Disabled pacticipant version interactions, not needed yet. (Beth Skurrie, Sat May 17 17:57:33 2014 +1000)
* cfefdc4 - Changed path from /pact to /pacts (Beth Skurrie, Sat May 17 15:58:32 2014 +1000)

#### 0.0.6 (2014-03-24)

* 2ad5f7d - Updated method of tagging versions (bethesque, Sat Mar 22 16:54:37 2014 +1100)
* b74128f - Added 'latest' pact url to pact representation in the 'latest pacts' response (bethesque, Sat Mar 22 09:04:31 2014 +1100)

#### 0.0.5 (2014-01-03)

* 194183c - Removing debugger for Travis CI (bethesque, Fri Jan 3 12:45:07 2014 +1100)
* b42aba9 - Changed 'last' to 'latest' (bethesque, Tue Nov 19 09:30:12 2013 +1100)
* 30d63b7 - Changed name to title in list pacticipants response (bethesque, Mon Nov 18 09:37:11 2013 +1100)

#### 0.0.4 (2013-11-15)

* cf33479 - Merge branch 'master' of github.com:bethesque/pact_broker-client (Beth, 20 hours ago)
* 01087ae - Fixed problem where PublicationTask block was evaluated at load time, instead of run time. (Beth, 20 hours ago)
* 2073234 - Updating to use example.org as the base URL (Beth, 2 days ago)
* 07073de - Updating latest pact URL (Beth, 2 days ago)

#### 0.0.3 (2013-11-13)

* a3488bd - Fixing application/json+hal to application/hal+json (Beth, 2 days ago)
* 0fa89ef - Updating content type to match new Webmachine implementation. Removing redundant repository_url interaction. (Beth, 2 days ago)
* 9e1539e - Redoing the URLs yet again (Beth, 3 days ago)
* 9067b83 - Working on list latest pacts (Beth, 3 days ago)
* 3ba218a - Specifying pact/latest response (Beth, 6 days ago)
* b746f23 - Changing to new /pacts/latest URL format (Beth, 6 days ago)
* 39f52cf - Working on expected 'pacts/latest' response (Beth, 6 days ago)
