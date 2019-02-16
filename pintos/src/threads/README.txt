I added the following lines of code to the following files.


File modified:
    Changes made


tests/threads/Make.tests:
    alarm-mega alarm-multiple alarm-simultaneous alarm-priority alarm-zero		\

tests/threads/Rubric.alarm:
    4   alarm-mega

tests/threads/tests.c:
    {"alarm-mega", test_alarm_mega},

tests/threads/tests.h:
    extern test_func test_alarm_mega;

tests/threads/alarm-wait.c:
    void
    test_alarm_mega (void)
    {
        test_sleep (5, 70);
    }

