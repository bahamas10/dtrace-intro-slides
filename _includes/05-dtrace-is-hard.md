DTrace is hard
===============

    syscall::write:entry{self->ts=timestamp;}syscall::write:return/self->ts/{this->lat=timestamp-self->ts;trace(this->lat);self->ts=0;}

---

If you know DTrace, you recognize this as a simple invocation


but if you don't... it's as hard to read as Node.js
