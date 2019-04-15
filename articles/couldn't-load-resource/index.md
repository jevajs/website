[zua]: https://github.com/thatziv
[logo]: https://raw.githubusercontent.com/jevajs/jeva-screen/master/main.png
# Couldn't load resource
 ![logo][logo]

 Written by [Zua][zua]
 > In almost every video, we create resources for the server. Most viewers expirience the issue of `couldn't load <resourcename>`. Here's how to fix that.
 > # FiveM - How to Fix Couldn't Load Resource - YouTube ![YouTube](https://s.ytimg.com/yts/img/favicon-vfl8qSV2F.ico)
 > [![FiveM - How to Fix Couldn't Load Resource](http://img.youtube.com/vi/cPJzei0cPFU/0.jpg)](http://www.youtube.com/watch?v=cPJzei0cPFU) 
  - *Make sure to watch this video as it's a visual fix.*
## Diagnosis
 1. Open up the resource's folder
 2. Check the root of the resource's folder to see if the `__resource.lua` is present. 
  - If the `__resource.lua` is not present, create one and follow the syntax of a proper `__resource.lua`.
  **Make sure it is called `__resource.lua` and not `__resources.lua`**
 3. Open the `__resource.lua`, and make sure you followed the **correct** syntax.
  *  ```lua
        -- This example can be found here at https://docs.fivem.net/scripting-reference/resource-manifest/resource-manifest/#example
        resource_manifest_version '44febabe-d386-4d18-afbe-5e627f4af937'

        client_scripts {
            'client.lua',
            'client_two.lua'
        }

        server_script 'server.lua'

        -- extra data can be used as well
        my_data 'one' { two = 42 }
        my_data 'three' { four = 69 }

        -- due to Lua syntax, the following works too:
        my_data('nine')({ninety = "nein"})
    ```
 4. Restart your server and connect!
