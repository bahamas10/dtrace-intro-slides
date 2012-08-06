Concepts in DTrace
==================

    syscall::open:entry                                 | Probe
    /execname == "bash"/                                | Predicate
    {                                                   | Actions
        printf("Open syscall fired by pid %d\n", pid);  | Actions
    }                                                   | Actions

---

Fields explained

* Probe is the event to hook into
* Predicate is a conditional to test before running any `Actions`
* Actions are code to execute when an event is matched
