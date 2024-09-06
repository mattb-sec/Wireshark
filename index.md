
# Introduction

With or without our knowledge and permission, the are thousands of packets of digital information being sent out and received every minute. That being said, it is important to keep in mind that not all information is transferred the same way. This brings forth the concept of protocols. CompTIA defines network protocols as “an established set of rules that determine how data is transmitted between different devices in the same network.” For instance, the Transmission Control Protocol (TCP) defines the way information is exchanged between senders and receivers (IBM) whereas the Address Resolution Protocol (ARP) is in charge of taking the name address of a machine and translating it into a usable address for a network (Techopedia). This lab is dedicated to capturing packets that use these protocols and analyzing both their function and role in a network. 

## Introducing and Installing Wireshark

The tool I will be using to capture packets in this lab is a free and open-source software known as Wireshark. The official website’s “about” page describes the program as “the world’s largest foremost and widely-used network protocol analyzer and views networks at microscopic levels” (Wireshark). The program is capable of capturing and deeply inspecting hundreds of protocols, capturing live network activity, allowing offline analysis, and reading live data from Ethernet connections. The program also has other uses such as detecting DoS attacks and grabbing passwords from passing File Transfer Protocol (FTP) packets. However, this lab is only concerned with surface-level analysis of basic internet traffic. Moreover, true to its reputation, this is an extremely popular piece of software and I have used it several times already for my other information systems classes. Nevertheless, the version I already had installed was due for an update, so I installed a fresh version of the program from Wireshark’s website. After launching it, I am taken to the program’s home page where I decide which network will be used for capturing.

## Explaining My Internet Connection and Illustrating My Network Architecture

Before I begin to capture network activity, it is important to first understand how my network is laid out. When my house was being built, all the network architecture has handled by AT&T. They had designed our connections such that only AT&T would be able to repair or modify them. Throughout my house are ethernet ports which join into two switches which connect to an AT&T U-verse router which is then connected to the house’s phone line. Additionally, the router connects to an AT&T Wireless Access Point (WAP).

In 2020, however, my family and I had noticed that our wired connections have been exceedingly bad for quite some time. The support technicians at AT&T had insisted that we had the fastest internet plan available, but only a few simple internet speed tests proved this to be a lie. Although our phone service was excellent, our internet connections were not. We eventually got fed up and opted to switch to Spectrum. However, my parents still wanted to keep AT&T for our phone service. The result was having a Spectrum modem and router crudely installed alongside the AT&T U-verse router and WAP. The Spectrum technicians stated that they could not do any more to modify the network due to the way AT&T had initially set it up. It works well, but the tradeoff was that all the ethernet ports in my house are now totally useless (and we have one of the ugliest network boxes you have ever seen). This was mostly fine since nothing except my computer really used ethernet anymore. Of course, I still wanted a wired connection and thankfully the network box is in my closet. My solution was to plug an ethernet cable into my desktop computer, run it across my room, and plug the other end into the Spectrum router. The router is then connected to the modem which is connected to the internet. The figure below shows an illustration of this:

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
