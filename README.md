mruby-syslog
============

### To build:

Prerequisites:

    * mruby
    * libc

    activate GEMs in *build_config.rb*
    * conf.gem :git => 'https://github.com/iij/mruby-syslog.git', :branch => 'master'
    env ENABLE_GEMS=true ruby ./minirake

### To run the tests:

    env ENABLE_GEMS=true ruby ./minirake test


For example,

    Syslog.open("syslogtest")
    Syslog.log(Syslog::LOG_WARNING, "the sky is falling in %d seconds!", 100)
    Syslog.close


## License

Copyright (c) 2012 Internet Initiative Japan Inc.

Permission is hereby granted, free of charge, to any person obtaining a 
copy of this software and associated documentation files (the "Software"), 
to deal in the Software without restriction, including without limitation 
the rights to use, copy, modify, merge, publish, distribute, sublicense, 
and/or sell copies of the Software, and to permit persons to whom the 
Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in 
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
DEALINGS IN THE SOFTWARE.

