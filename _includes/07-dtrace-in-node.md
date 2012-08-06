Concepts in Node
================

    syscall.on('open', function(pid, execname) {
      if (execname === 'bash') {
        console.log('Open syscall fired by pid %d', pid);
      }
    });

---

This is what a DTrace script would look like in node...
