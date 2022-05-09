# Lab Report 3 Week 6
## Streamlining ssh Configuration
Here, we will learn how configuration files can be used to make the process of logging into servers easier.

**Step 1:** Open up or create a <code> ~/.ssh/config </code> file.

- You can do this in any text editor.
- Make sure that it is in your ssh directory.

**Step 2:** Add the following lines into the file.
<code>

    Host ieng6
        HostName ieng6.ucsd.edu
        User cs15lsp22zzz (use your     username)
</code>
The file will look something like this:

![Image](file.png)


**Step 3:** Run the command <code> ssh ieng6 </code> 

Like this:

![Image](command.png)

Now, we can even try copying files into your account using *scp*!

![Image](terminal.png)

