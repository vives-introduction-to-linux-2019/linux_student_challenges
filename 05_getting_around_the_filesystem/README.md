# Chapter 05 - Getting Around the FileSystem

## touch

What does `touch` actually do? Demonstrate using an example.

## Files and Directories

Note down all the instructions for solving the assignments below.

### Hello

1. Create a directory `projects` in your home directory.

2. Create a file called `my_name` inside of `projects` and add your full name inside of it using a text editor such as nano.

3. Output the content of the file using `cat`.

4. Create another file called `hello` with the content `Hello`.

5. Now execute the command `cat hello my_name`. Explain the output. What happens here ?

6. Create a subdirectory `hello` inside of `projects`. Move all te files we created to this `hello` directory. Can you do it in a single command?

7. Now create a `backup` directory inside `projects`. Now make a copy of the directory `hello` to the directory `backups`. If you did it correctly, you should now have a directory `hello` in `backups`.

### Chuck

1. Make a git clone of `https://github.com/BioBoost/chuck_norris_facts.git` inside of the directory `projects`.

2. Rename the directory to `facts_about_chuck_norris`.

3. All we need from this repo is the actual facts from the file `README.md`. Delete all other files and directories. Don't forget to remove the hidden `.git` directory.

4. Edit the `README.md` file and remove everything except the actual facts. Output the result using `cat`.

5. Make a backup of the directory `facts_about_chuck_norris` to `backups`.

### My Own Local Domain Name

1. Make a backup of the file `/etc/hosts` to the directory `~/projects/backups/domain` directory. Create the directories as needed.

2. Search the man pages for the use of `/etc/hosts`. Explain in your own words.

3. Edit the file `/etc/hosts` so we can ping the hostname `mymachine.dev`. Test it by using the `ping` command. Output the result here and the content of `/etc/hosts`.

### NodeJS

1. Install NodeJS by following the instructions on [https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-debian-10#installing-using-a-ppa](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-debian-10#installing-using-a-ppa).

2. Check if the installation completed successfully by issuing the command `node --version`. It should return `v12.13.0`.

3. Remove the bash script from your home directory.

4. Go back to your `projects` directory and create a directory `hello_api`.

5. Create a file called `index.js` inside of the directory `hello_api`.

6. Next install the `express` module by executing the command `npm install express` inside of the directory `hello_api`.

7. Now edit the file `index.js` using nano and place the following content in it:

```js
const express = require('express')
const app = express()
const port = 3000

app.get('/', (req, res) => res.send('Hello World from Nico!'))

app.listen(port, () => console.log(`Example app listening on port ${port}!`))
```

8. Replace my name with yours in the javascript code above.

9. Next we need to enable port forwarding on our virtual machine. Go to `Settings => Network => Adapter 1` and click `Advanced` and then `Port Forwarding`. Now add the rule:

```text
Name: NodeJS Hello API
Protocol: TCP
Host IP:
Host Port: 3000
Guest IP
Guest Port: 3000
```

10. Now open powershell in windows and determine the IP address of your virtual box host adapter using the command `ipconfig` (specific command on windows to determine ip address of network interfaces).

11. Now surf to this IP address using a browser. Don't forget to specify that port `3000` should be used.

12. What would you need to change to make it work using port `80`?
