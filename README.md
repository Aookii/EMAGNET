# EMAGNET v3.4.2

### Before you using emagnet, please remember that with great power comes great responsibility. 

## <p align="center">![Screenshot](https://i.ibb.co/3B5GS6X/68747470733a2f2f6e72312e6e752f656d61676e65742f70726576696577732f656d61676e65745f6f6c646d6f76692e676966.gif)

| Current Version    | News                            | Tested On                          |
| :----------------- | :-------------------------------- | :----------------------------------|
| `3.4.2`            |  Support for scraping via API has been added    | Linux/MacOS/OpenWRT/Windows/Android                               |
| `3.4.1`            |  Support for SSH Tunnel/Socks5 proxy    | Linux/MacOS/OpenWRT/Windows/Android                               |
| `3.4`              |  Full support on android devices, no root required    | Linux/MacOS/OpenWRT/Windows/Android                               |

<a href="https://github.com/wuseman/EMAGNET"><img src="https://img.shields.io/github/languages/top/wuseman/emagnet.svg?color=magenta&label=Bash%2FShell"></a><a href="https://github.com/wuseman/EMAGNET/issues?q=is%3Aissue+is%3Aclosed">
<img src="https://img.shields.io/github/issues-closed/wuseman/emagnet.svg?color=light&label=Closed%20Issues"></a>
 <a href="https://github.com/wuseman/EMAGNET/issues"><img src="https://img.shields.io/github/issues-raw/wuseman/emagnet.svg?color=orange&label=Open%20Issues"></a><img src="https://img.shields.io/github/last-commit/wuseman/emagnet.svg?color=darkmagenta&label=Latest%20Commit"><a href="https://twitter.com/wuseman1">
 <img src="https://img.shields.io/website/https/nr1.nu.svg?down_color=darkred&down_message=DOWN&label=Nr1.nu%2Femagnet&up_message=UP"><img src="https://img.shields.io/github/license/wuseman/emagnet.svg?color=blue&label=License"></a></a></a>
</a>
</p>


### Latest Update: 

Once again it's boring news. 

Pastebin really working hard for block Emagnet and all users that using emagnet, they closed/removed 20+ accounts that was used for scrape and monitor pastebin.

It's not possible to buy pro accounts anymore since they "sold out" all PRO accounts so from now it's not possible to use emagnet beta neither since they closed over 20+ accounts that was used to scrape pastebin, emagnet works fine still but you wont be able to get all pastes anymore due to all limits they added last 2 months so for now they blocked emagnet and it out of my control, really.

![Screenshot](https://nr1.nu/f/gjojs.png)

PRO users: You will be able to scrape pastebin with your added ip on pastebin  even if you wont pay next bill so don't buy another month of PRO account, for be able to scrape pastebin from your IP you just need to use curl with mozilla useragent and also include the cookie from _ga and cf_clearance. For not use static _ga and cf values use |shuffle -n1 for randomize the values. 

Here is an example how you can scrape pastebin again without pay for another month of PRO account:

    curl -Ls 'https://scrape.pastebin.com/api_scraping.php' -H 'User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:68.0) Gecko/20100101 Firefox/68.0' -H 'Cookie: _ga=GAx.x.xxxxxxxxxx.xxxxxxxxx0; cf_clearance=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx-xxxxxxxxxxx-x-xxxxxxxx-xxx'|grep -i full_url|awk -F'"' '{print $4}'|sed 's/.com/.com\/raw/g' 

As you can see I got no PRO account on this IP, but I am able to scrape Pastebin so remove your card from this place :-) 

![Screenshot](https://nr1.nu/f/yvggy.png)
![Screenshot](https://nr1.nu/f/jddfi.png)

### About: 

Emagnet is a very powerful tool for it's purpose wich is to capture  email addresses and passwords from leaked databases uploaded on pastebin. It's almost impossible to find leaked passwords when they are out of list on pastebin.com. Either they have been deleted by pastebin's techs or the uploads is just one in the crowd. To be honest it's easier to find a needle in a haystack then find outdated uploads on pastebin with the data we want to collect. 

#### BBC NEWS: ["Pastebin: Running the site where hackers publicise their attacks"](https://www.bbc.com/news/technology-17524822) 

- Emagnet is No.1 tool for fetch these leaks from pastebin

### Emagnet Beta

Use beta version for be updated - ![Emagnet Beta - v4.0](https://github.com/wuseman/EMAGNET/tree/emagnet/beta) 

### Getting Started

    git clone https://github.com/wuseman/emagnet
    chmod +x emagnet/emagnet.sh
    bash emagnet/emagnet.sh --emagnet
  
### Sit back and relax and Emagnet will do the rest, watch the video below, this is for real!	

![Screenshot](.preview/emagnet-latest.gif)

### ... So how does this work? See the video below exactly line by line how it works: 

* Left side is how you see things - Right side is what actually going on:

![Screenshot](.preview/emagnet2-debug.gif)

### System Requirements

- Bash     - Find more info about _bash_ [here](https://www.gnu.org/software/bash/)
- Wget     - Find more info about _wget_ [here](https://www.gnu.org/software/wget/)
- Curl     - Find more info about _curl_ [here](https://github.com/curl/curl)

### Wiki Sections:

- [About](https://github.com/wuseman/EMAGNET/wiki/ABOUT) - 
_How everything started._
- [Previews](https://github.com/wuseman/EMAGNET/wiki/PREVIEWS) - 
_Previews can be found here._
- [Configurations-&-Installation](https://github.com/wuseman/EMAGNET/wiki/Configurations-&-Installation) - 
_Get started with spotify brute forcing - How emagnet will work with your openvpn files._
- [Regex - Tips For Search](https://github.com/wuseman/EMAGNET/wiki/Searching-&-Regex) - How To Find your facebook credenticals, if it has been leaked._
- [Leaked Databases](https://github.com/wuseman/EMAGNET/wiki/Leaked-Databases) - Various Public Leaks

## Changelog

[Versions changelog](CHANGELOG.md).

## Authors: 

* **wuseman <wuseman@nr1.nu\>** 

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE.md](LICENSE.md) file for details

### Contact

  If you have problems, questions, ideas or suggestions please contact me on *_wuseman@nr1.nu_  - For faster contact visit freenode irc network or the webchat and type '/msg wuseman hi!' in the input bar and I will reply you ASAP I will see the message.
  
  Enter Freenodes network via your own client 'chat.freenode.com:+6697 or use their new web client [here](https://webchat.freenode.net/)

### Notice

Attacking different kinds of accounts via emagnet that you have not been granted or allowed to attack is strictly prohibited and it breaks the law. The punishment is hard and you can even get into prison in some countries just for trying to attack for intrusion. With this said, it's *important* that all users is aware of this and when you have cloned or downloaded it's fully up to every user to take responsibility over their own actions. wuseman cannot be held responsible for the actions of any user, all users using Emagnet on their own responsibility. 

Developer: "All my previews where a brute force attack has been done is under controlling forms with 100% fully permissions by the owners. If you have any questions about this then you are welcome to contact me or the owner."

### Haters Gonna Hate

If you are one of these who dislikes _EMAGNET_ and believe the program has been developed for a reason that would break the law then I am not interested in taking part of your opinions, keep them for _yourself_! Emagnet does **NOT** leak any data at all either to the developer(s) or anyone else. No statistics at all to track any user so if you want to contact me for ask who it might was who downloaded emagnet a specific date is completely useless since i really have no idea, and to be honest I don't care.

Feel free to read the history about emagnet [here](https://github.com/wuseman/EMAGNET/wiki/About) and how everything started about this project.

#### Development of emagnet is active and is updated frequently, please use the latest version if you report issues/bugs.

### Greetings: 

_m1st_ that deliver legit leaks for us daily.

And to all ppl that is trying to sell public leaks and steal the real hackers job, f*ck you! This is one reason why I started this project, I hope this project will get widely spreaded so you will earn 0.00$ on your re-edited malware shit!

Cheers!

### Feel free to send donations if you want to support the development of the emagnet

      BTC Address: 1MJ3JATUjfRUSoBdrbRHEC5XX1zgH72uKj

### Emagnet is a private project since 2015 and was released in June @ 2018, to be continued. 



