Node.js is <s>hard</s> easy
===========================

    var http = require('http'),
        util = require('util');

    http.createServer(function(req,res) {
      console.log('incoming.');
      res.end(JSON.stringify(
      {
        'message': 'OK',
        'url':     util.format('is %s', req.url)
      }
      ));
    }).listen(80,'0.0.0.0');

---

Now you can start to make sense of this...
