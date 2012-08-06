Node.js is hard
===============

    var http=require('http'),util=require('util');http.createServer(function(req,res){console.log('incoming.');res.end(JSON.stringify({'message':'OK','url':util.format('is %s',req.url)}));}).listen(80,'0.0.0.0');

---

If you know Node.js, you can tell what this is doing...


but if you don't... forget about it
