# sync()

Дедовский системный вызов `sync()` не оптимален для решения описываемых задач, зато гараздо более универсален. Этот вызов обеспечивает синхронизацию всех буферов, имеющихся на диске:

    #include <unistd.h>

    void syns();

    