# on_exit()

SunOS 4 определяет собственный эквивалент `atexit()`, библиотека `glibc` в Linux поддерживает его:

    #include <stdlib.h>
    
    int on_exit(void (*function)(int, void*), void* args);
    
Последняя версия Solaris уже не поддерживает эту функцию. Вместо нее необходимо использовать стандартно компилируемую `atexit()`.

