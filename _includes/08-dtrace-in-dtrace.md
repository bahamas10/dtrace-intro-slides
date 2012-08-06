Concepts in DTrace
==================

    syscall::open:entry
    /execname == "bash"/
    {
        printf("Open syscall fired by pid %d\n", pid);
    }

---

And this is what it looks like in DTrace
