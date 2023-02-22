<p>$tpi is our custom command-line interface that should help you interact with Turing Pi V2. It is still a work in progress and new features should be available as soon as possible. It is also open source, and the guide on where to find it and how you can contribute to it will be in our advance section.</p>
<p>$tpi is pre-installed on BMC and you can simply invoke it by:</p>
<pre># tpi -h<br>Usage: tpi [host] &lt;options...&gt;<br>Options: <br>        -p, --power (on off status) Power management <br>        -u, --usb (host device status) USB mode,Must be used with the node command<br>        -n, --node (1 2 3 4) USB selected node<br>        -r, --resetsw reset switch<br>        -U, --uart uart opt get or set<br>        -C, --cmd uart set cmd<br>        -F, --upgrade upgrade fw<br>        -f, --flash todo<br>        -h, --help usage<br>example: <br>        $ tpi -p on //power on<br>        $ tpi -p off //power off<br>        $ tpi -u host -n 1 //USB uses host mode to connect to Node1<br>        $ tpi --uart=get -n 1 //get node1 uart info<br>        $ tpi --uart=set -n 1 --cmd=ls//set node1 uart cmd<br>        $ tpi --upgrade=/mnt/sdcard/xxxx.swu //upgrade fw<br>        $ tpi -r //reset switch</pre>
<p> </p>