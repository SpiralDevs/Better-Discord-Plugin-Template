# Better-Discord-Plugin-Template

<details><summary>Template Code</summary>
  
```js
/**
 * @name PluginName //no spaces in this field
 * @description Plugin description goes here
 * @version 1.0.0 //current plugin version
 * @author YOURNAME //use discord name excluding the # + the numbers
 * @authorId 707771493441994843 //your discord id
 * @authorLink https://github.com/SpiralGaming //the link to your github or replit (something along those lines)
 * @website https://google.com
 * @source https://google.com //teh github or repl
 * @updateUrl https://google.com
 */

// config
const config = {
    info: {
        name: "Plugin Name", //allows spaces
        id: "PluginName", //doesn't allow spaces
        description: "Plugin description.",
        version: "1.0.0", 
        author: "Spiral",
        updateUrl: "https://google.com", //the link 
    },
    changelog: [
        {
            title: "Plugin Name",
            items: ["Changes made to plugin..."]
        }
    ]
}


	module.exports = class TimeViewer { 
	  //gets author's name
	  getName () {return config.info.name;}
		//gets author
	  getAuthor () {return config.info.author;}
		//gets plugin version
	  getVersion () {return config.info.version;}
		//gets plugin description
	  getDescription () {return config.info.description;}
	
		//
	  load() { 
			console.log("Plugin loaded successfully..."); 
		}
	
	  start() {
	  	BdApi.alert("This is an alert title.", `This is an alert description. This is an alert, this one will show when the plugin is turned on in discord.`); //gives a popup in discord 
			console.log("Plugin started successfully...");
	  }
	
	  stop() {
	  	BdApi.alert("This is an alert title.", `This is an alert description. This is an alert, this one will show when the plugin is turned off in discord.`); //gives a popup in discord 
			console.log("Plugin stopped successfully...");
	  }
	}
  ```
  </details>
  
  [Download Template](#)
