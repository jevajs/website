[zua]: https://github.com/thatziv
[logo]: https://raw.githubusercontent.com/jevajs/jeva-screen/master/main.png
# Server Starter Closing Immediately After Startup.
![logo][logo]

 Written by [Zua][zua]
 > In the video *How to Make a FiveM Server*, we have to create a [batch file](https://en.wikipedia.org/wiki/Batch_file). In this batch file we have to use your computer's directory. Some individuals have a problem with this due to their directories having spaces in them.

 1. A good work-around to this is just to move the server folder to another drive or folder **without a space in it**. Then edit the `starter.bat` to the according directory you moved it to. 
    * Before:
    ```shell
        cd /d C:\Users\Zavaar Shah\Desktop\server\cfx-server-data-master
        C:\Users\Zavaar Shah\Desktop\server\run.cmd +exec server.cfg
    ```
    * After:
    ```shell
        cd /d C:\server\cfx-server-data-master
        C:\server\run.cmd +exec server.cfg
    ```
 