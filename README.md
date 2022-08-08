# mytextinfolder
List file lines matched a specific regural expression (or simple string) in a folder.

It's just a simple script to search for specific parts of a source code.

## Usage
`mytextinfolder <folder> <regex or simple string>`

### Example
`mytextinfolder /var/www/html/ '\(mysqli_connect\|new mysqli\)'`

And you will see all mysqli connections. ;)

## Installation
- You can either [download](https://github.com/tamas646/mytextinfolder/raw/main/mytextinfolder_1.1.0_all.deb) and install the deb package or use the source code and setup it yourself.

- If you wish, you can install it from my apt repository too:

  ```sh
  sudo echo "deb [signed-by=/usr/share/keyrings/ptamas-pub.gpg] http://apt.ptamas.hu/main/ ./" > /etc/apt/sources.list.d/apt.ptamas.list
  wget -qO - https://apt.ptamas.hu/ptamas-pub.gpg | gpg --dearmor | sudo tee /usr/share/keyrings/ptamas-pub.gpg > /dev/null
  apt update && apt install mytextinfolder
  ```
