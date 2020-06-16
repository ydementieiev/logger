# Logger

It's a Simple Logger, just connect file to your project.


### How to use

* Create global logger in your file.
```
 CREATE_LOGGERPTR_GLOBAL(logger_ptr, "Your logger name", "Path to your file or file name");
```
* Add autotrace to the start of your function.
```
 LOG_AUTO_TRACE(logger_ptr, "Your function name");
```
* Use one of the proposed log level.
```
 LOG_INFO(logger_ptr, "Your log message.", std::string, int, ...);
 LOG_DEBUG(logger_ptr, "Your log message.", std::string, int, ...);
 LOG_ERROR(logger_ptr, "Your log message.", std::string, int, ...);
```

### Note

Logs save to -> log.txt file in your binary directory.
