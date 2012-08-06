DTrace is <s>hard</s> easy
==========================

    syscall::write:entry
    {
        self->ts = timestamp;
    }

    syscall::write:return
    /self->ts/
    {
        this->lat = timestamp - self->ts;
        trace(this->lat);
        self->ts=0;
    }

---

It's not so bad
