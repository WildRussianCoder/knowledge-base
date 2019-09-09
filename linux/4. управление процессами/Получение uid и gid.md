# Получение uid и gid

    #include <unistd.h>
    #include <sys/types.h>
    
    uid_t getuid();
    gid_t getgid();

Они не могу привести к неудаче. Аналогично эти два вызова возвращают действительные идентификаторы пользователя и группы соответственно:

    #include <unistd.h>
    #include <sys/types.h>
    
    uid_t geteuid();
    gid_t getegid();
    
Они также не могут привести к сбою.