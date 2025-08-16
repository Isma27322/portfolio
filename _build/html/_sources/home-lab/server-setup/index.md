# The Server Build

### Choosing the Brains
* How I chose the brains for my server, for my first home lab I used some old laptops I was gifted from my brother

### The Setup Process
* For my newest server install(ubuntu 24.04 LTS), I had to install it twice. This was mostly because the default formatting creates an LVM group (often used with servers that have more than one disk), and I found it didn't use the entire 500GB SSD.
* To get around the disk issue I had to do the custom storage layout to make it exactly the way I needed with the disk, swap, and the boot partitions

### Locking it Down
* Even though it is a local server with not much access from the public internet. It is still good to lock it down these are the steps I took to do that:
    1. Not allowing root login over ssh
        * Is actually a default thing with the new ubuntu servers.
    2. Requing a ssh key to login over ssh and not allowing passwords
    3. Changing the default ssh port from the default 22
