# Project 7 - WordPress Pen Testing

Time spent: **10** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pen Testing Report

### 1. Unauthenticated Stored Cross-Site Scripting: 


- [ ] Summary: 
  - Vulnerability types: Unauthenticated Stored Cross-Site Scripting URLS:
  - Tested in version: 4.1.0
  - Fixed in version: WordPress 4.1.2 
- [ ] GIF Walkthrough: 
- [ ] ![ezgif com-gif-maker(1)](https://user-images.githubusercontent.com/88115439/199626407-a8eaa02b-f821-4c29-b3a2-3410e719db14.gif)
- [ ] Steps to recreate: create a post and then test my inject Cross-Site Scripting (basic script tags) into the comment section. To find the vunerbility I used WPSCAN.
- [ ] Affected source code:
  - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
  
- https://wpscan.com/vulnerability/604b553d-5492-4f8c-af7a-db7169780032     
 - https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3438

 - https://wordpress.org/news/2015/04/wordpress-4-1-2/
 - https://cedricvb.be/post/wordpress-stored-xss-vulnerability-4-1-2/
  
### 2. Username Enumeration

- [ ] Summary: 
  - Vulnerability types: Username Enumeration
  - Tested in version: 4.1.0
  - Fixed in version: 4.1.28
- [ ] GIF Walkthrough: 
![](ezgif.com-gif-maker(1)%20copy.gif)![ezgif com-gif-maker(1) copy](https://user-images.githubusercontent.com/88115439/199633008-0fad5351-9d96-4c55-9ccb-ca676a62cc28.gif)

![](ezgif.com-gif-maker(1)%20copy.gif)
- [ ] Steps to recreate: First did a wpscan on the site to find username enumerations. With this I than created two files usernames and passwords which contained the username found and sample passwords. 
- [ ] Affected source code:
  - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)

### 3. Password Enumeration

- [ ] Summary: 
  - Vulnerability types: Password Enumeration
  - Tested in version: 4.1.0
  - Fixed in version: 4.1.28
- [ ] GIF Walkthrough: ![](Screen%20Shot%202022-11-02%20at%207.54.02%20PM.png)
![](ezgif.com-gif-maker(1)%20copy%202.gif)![ezgif com-gif-maker(1) copy 2](https://user-images.githubusercontent.com/88115439/199632990-90e397ae-92b7-4b70-8cec-d91903f21bfe.gif)

![Screen Shot 2022-11-02 at 7 54 02 PM](https://user-images.githubusercontent.com/88115439/199632896-7a3d7131-2bcc-4f20-ace8-1d3b2c325596.png)

- [ ] Steps to recreate: After getting the resultes back from the first scan I then did another scan for the password which came back with the correct passkey. 
- [ ] Affected source code:
  - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)


## Assets

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with  ...
https://ezgif.com/ 
<!-- Recommended GIF Tools:
[Kap](https://getkap.co/) for macOS
[ScreenToGif](https://www.screentogif.com/) for Windows
[peek](https://github.com/phw/peek) for Linux. -->

## Notes

Challenges encountered while doing the work

I had a hard time setting up docker and really understanding how it works. But through this Pen Testing activity I was able to practice multiple brectching techniques to get in. 


## License

    Copyright [2022] [Ezekiel Faulknor]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
