# |How do I download the source code?
Its right here in releases, as its not precompiled -->

# |What is it
A lightweight FastFetch/NeoFetch clone for the C# Operating System Development Kit Cosmos (https://github.com/CosmosOS/Cosmos)

# |How do I add it to my Cosmos OS?
Firstly, in your Kernel.cs, you must add this class anywhere as long as it is public and accessible to multiple files.

```
    public static class Global
        {
           public static string OS = "Your operating systems name, which will need to be specified both here and in ascii.cs when making your ascii art.";
           public static string OSversion = "Your operating systems version or version name";
           public static string DE = "The desktop environment your OS uses, or the TUI, or the command interpreter name, it doesn't matter what you choose - could be nothing at all";
           public static string user = your method of fetching your OS's username, if applicable;
           public static string hostname = "your OS's hostname, if applicable";
        }
```
Then, where ever you would like, drag and drop the unzipped CosFetch Folder into your project. After, add it to your command interpreter. The CosFetch application does not expect
any specific way of you doing this, so it is extremely versatile and should work on all terminals with minimal to no tinkering. And, you can remove or add bits to CosFetch.cs
as much as you would like! Everything works independently of each other, so you can remove everything but the OS name and OS version if you really wanted to, or make it only
display your ASCII art, or have a comprehensive list of everything about your OS. It's entirely up to you!

# |How do I add my ASCII art to CosFetch?
Simply go to ascii.cs, scroll to the bottom and edit this:

```
      if (Kernel.Global.OS == "Put your OS name here!")
	    {
	    Console.WriteLine("put your ascii art here")
	    }
```

For example, this is the Waterfall ASCII art in code:

```
           if (Kernel.Global.OS == "Waterfall")
            {
            Console.WriteLine(@" /\          /\  _______ ______ _____  ______      _      _      
 \ \        / /\/__   __/  ____/____ \|  ____/\   | |    | |     
  \ \  /\  / /  \  | |  | |__   ____) | |__ /  \  | |    | |     
   \ \/  \/ / /\ \ | |  |  __/ |  _  /|  __/ /\ \ | |    | |     
    \  /\  / /__\ \| |  | |____| | \ \| | / /__\ \| |____| |____ 
     \/  \/_/______\_|  |_____/|_|  \_\_|/_/______\______|______|
                                                                 
                                                                 ");
            }
```

# |Screenshots
![image](https://github.com/user-attachments/assets/df3201b6-82f2-47d3-abf7-812de28f7181)
This is an example of it running on my own Operating System Called Cosmix.
