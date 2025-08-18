---
date_created: 2025-08-16
date_modified: 2025-08-18
---
# Content Areas || Opening Up Content

Opening up Content to new topics while keeping the Lossless content clean.

A "Content Area", is a cluster of topics, organizations, projects, initiatives, concepts, vocabulary, etc that become the shared knowledge and experience set of professionals in an industry, space, cause. 

In the [[concepts/Public Repository|Public Repository]], you will see folders that are Capitalized, these are the content areas we are building out together. As of August 2024, the areas are Blue-Economy, Health, and Finance. The folders that are not capitalized will be treated a little differently. Now, there's only one called "general"

The "general" folder serves two purposes:
1. a catch-all when content creators are unsure where something should go
2. a shared version of a document that can be accessed and rendered in any Content Area, so when a document might fall into multiple areas, or are not clearly limited to one area.

The Area folders and the general folder should have the same folder structure. To make it easier to quickly recognize and differentiate, domain folders should be Capitalized and general folders should be lowercase. 
## Domains expected:

**As of August 2025:**
1. Health (Healthcare, Public Health, HealthTech, Medicine)
2. Blue-Economy (Water, Sustainabilty & Innovation & Issues)
3. Finance

**Expected in the future:**
1. Economics & Prosperity
2. Education & EdTech
3. Energy
4. Computing & AI Infrastructure
5. AgTech & FoodTech
6. FinTech & RegTech

# Setting Expectations: Contributing requires some nerd-level setup

For people who have not done programming or worked their computer using the command line, which is most everybody, there is about 2 hours of setup work that requires being a bit confused and going into unfamiliar territory.  It's actually really easy, everyone says _after_ it's over. During, it feels like getting an unwanted lesson in teeth pulling. 

You will need to:
- Use a few features of the Operating System you probably did not even know exist. 
- Use the command line to type commands.
- Install a few systems-level programs and know how to start and stop them. 
- Create an account on GitHub.
- Understand a few basic concepts in Version Control systems. We use Git (so does 95% of programmers.)
# Getting Started

Download [GitHub Desktop](https://github.com/apps/desktop) unless you want to use the terminal and command line (which usually only hackers and geeks use the command line.)

### Getting Started with Obsidian
Download [Obsidian](https://obsidian.md)
Create a vault in obsidian called `my-tws`

# Starting the plug-ins every time

## Installing the nerdy stuff
- A [[Package Manager]], for Windows it's [[Tooling/Software Development/Programming Languages/Libraries/Chocolatey]], for Mac it's [[Tooling/Software Development/Developer Experience/Homebrew|Homebrew]], for Linux you should already have all this already. 
- [[Tooling/Software Development/Developer Experience/DevTools/Node.js|Node.js]] but through [[Node Version Manager]], so install the [[Node Version Manager]] first. 
- [[GitHub Desktop]]
- Using [[GitHub Desktop]], cloning our Obsidian Community Plugins Perplexed, Cite Wide, and Starter. 
### On Windows
#### Install Chocolatey, the Windows Package Manager
[[Tooling/Software Development/Programming Languages/Libraries/Chocolatey]] is a [[Package Manager]], which software that installs, updates, cleans up, and removes other software. Package Managers are typically used to install "infrastructure" like software that usually does not have a user interface, just performs different functions on your computer.  
1. Follow the [instructions to install Chocolatey](https://chocolatey.org/install)
2. **Open the "Command Line" application as an "administrator"** of your computer. To do this, search for Command Line in the windows launcher. Instead of just clicking or hitting enter, look for an option that says: "Open as administrator." If you don't see that option, left click or hit control or alt and it should reveal a few options, "Open as an administrator" should be among them. 
3. Install with `powershell.exe` or `cmd.exe`, following the instructions of one or the other.

#### Install Node Version Manager
Once [[Tooling/Software Development/Programming Languages/Libraries/Chocolatey]] is installed, you should be able to use the command line to very easily install Node Version Manager
```powershell
choco install nvm
```

## On windows 

```bash

```


#### If Node Version Manager doesn't go well
[https://nodejs.org/en/download/current](https://nodejs.org/en/download/current)



Go to our GitHub repository content-domains, with needs to be on your local computer only 

and clone it on your computer using GitHub desktop. 


### Install Node with Node Version Manager
```
nvm install 22
```

### Install pnpm
```powershell
choco install pnpm
```

# Cloning our Plugins
https://github.com/lossless-group/cite-wide.git
https://github.com/lossless-group/perplexed-plugin.git
https://github.com/lossless-group/obsidian-plugin-starter.git 

# Connecting our Plugins to your Obsidian Vault

On Windows, open the Command Prompt app as an Administrator and paste: 
```bash
mklink /J "C:\Users\97152\code\obsidian-plugins" "C:\Users\97152\OneDrive\Desktop\My TWF\.obsidian\plugins" 
```
 `C:\Users\97152\code\obsidian-plugins`

# Setting up our Plugins
Once the plugins Starter, Cite Wide, and Perplexed are in the right directory:
For ease of management, open [[PowerShell]] on Windows and [[Terminal]] on Mac. 

Navigate into the plugins directory (folder) using `cd` and `ls`

Now either create two more tabs in the same open PowerShell or Terminal, or open two more windows of them.  

In one, change directory into `cite-wide`
In another, change directory into `perplexed-plugin`
In the other, change directory into `obsidian-plugin-starter`

In each one, type `pnpm install`.  You should see a bunch of text explaining all the things it's installing and it will probably go pretty fast. 

# Get Going with Contributing

For ease of management, open [[PowerShell]] on Windows and [[Terminal]] on Mac. 

Navigate into the plugins directory (folder) using `cd` and `ls`

Now either create two more tabs in the same open PowerShell or Terminal, or open two more windows of them.  

In one, change directory into `cite-wide`
In another, change directory into `perplexed-plugin`
In the other, change directory into `obsidian-plugin-starter`

In each one, type `pnpm build` then wait until the build is successful. 
Then, type `pnpm dev`

Once all three plugins are "running" (the program is now made available to Obsidian), and the Plugins should work seamlessly. 

## For more on how to use or Plugins:
